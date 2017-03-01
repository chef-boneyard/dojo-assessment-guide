<!--
#
# Copyright:: Copyright (c) 2012-2016 Chef Software, Inc.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#
-->
## Working with People

1. Coding Practices


## Coding Practices

1. Developers follow code inspection standards (rubocop, foodcritic, etc.)
2. Code reviews are performed and results are shared with developers
3. Every change is reviewed by at least two people with relevant skill and contextual knowledge
4. Software and automation components are shared and co-developed
5. Any potential contributor to a project can find its code and documentation with minimal assistance
6. Regularly scheduled automation demos occur
7. The codebase is almost always in a releasable state

Note:
Q2. results are shared (because w/o it, it's meaningless)  
Q3. person who wrote it plus one other (pair or mob programming is ok). At chef we have 2 people in addition to the writer.  
Q4. No Brents - Do you have that one person who you have to call to get the particular piece deployed.  
How many peieces of technology does only one person know about?  
Q6. Why what you did matters (what you did is clever, but why did you do it?)  Encourages collaboration. Practice speaking and presenting to business.  
Keeps you from spending 5 months building something that no one but you cares/knows about



## Working with Machines

1. Version Control
1. Chef Local Development
1. Continuous Integration
1. Chef Code Deployment
1. Application Deployment
1. Continuous Delivery
1. Virtualization as a Service
1. Full-Stack Automation
1. Compliance Automation
1. Sustaining Operations Culture


## Version Control

1. All source code is stored in a version control system (VCS)
2. All infrastructure and deployment code is stored in VCS

Note:
Scope of access, may include security, compliance, testing, operations.  
For example, all of your cookbooks are in VCS, but you have to create data_bags by hand.  


## Chef Local Development

1. Developers provision their own isolated VMs as needed
1. Developers use Chef development tools (ChefDK, Vagrant, etc)
1. Developers download code dependencies in a friction-free manner
1. Developers run unit tests (ChefSpec) locally
1. Developers run complaince checks (InSpec) locally
1. Developers use Test Kitchen to verify that cookbooks work as intended


## Continuous Integration

1. All projects use a CI service
1. CI job templates exist for each type of software project (Chef cookbook, Java app servers, Node.js app, etc.)
1. CI jobs lint projects
1. CI jobs unit test projects
1. CI jobs integration test projects
1. CI jobs execute functional tests against projects
1. CI jobs verify complaince of projects

Note:
Intergration (as it applies to applications) - old school java - have db layer. Java code calls DB directly w/o api, so you're testing that functionaltiy. Ex: create record. (create throw away db, and throw away data, or pretend to write something)  
Functional (as it applies to applications) - has to do with how the system is expected to be used. From the perspective of the end user (or if a service, does the API behave as expected)  


## Chef Code Deployment

1. CI jobs upload cookbooks to a Chef server
1. Cookbook updates are only uploaded via CI
1. All non-cookbook Chef policy (environments, roles, data bags, etc.) is only uploaded via CI
1. CI jobs pin dependencies so that they cannot be modified in later deployments
1. CI jobs assign a set of cookbook versions to a Chef environment
1. Cookbook deployments are automated
1. Cookbook deployment automation manages the sequence of deployments


## Application Deployment

1. Applications are deployed without manual intervention
1. Applications follow a clear promotion path (e.g., Dev -> QA -> Staging -> Production)
1. Application deployment automation manages the sequence of deployments (e.g.: Database schema first, then app servers)
1. CI jobs automatically update, pin, and test runtime dependencies of applications
1. Application deployment automation performs parallel, rolling, and/or canary deployments
1. Deployments are run during the business day without causing negative user experiences

Note:
Approval of a deployment is not considered manual intervention.
Q5. Can you deploy automatically with minimal impact/downtime.  
Paralles is also known as Blue/Green
Rolling - 7 nodes in LB, pull one out, deploy, verify, put it back, repeat.  
Canary - deploy this thing to x% of my nodes (eg: Netflix - first to 1 node, then 1%, then x%, then everywhere.)


## Continuous Delivery

1. All validation and deployments are executed in a pipeline that goes from source control all the way to production
2. Small batches of work flow through the pipeline
3. Changes are released weekly, if not more frequently
4. Changes that pass validation are automatically released to production

Note:
Q4 is the "Continuous Deployment" vs. "Continuous Delivery" clarifying question


## Virtualizaton as a Service

1. All servers are provisioned via APIs
1. Resources are provisioned in a friction-free manner
1. System images are built via an automated process
1. System images are built from scratch or from a well known, trusted origin
1. System images are built in a pipeline
1. System images are frequently updated


## Compliance Automation

1. Compliance policies are expressed in code
2. Compliance is checked automatically
3. Compliance automation removes non-compliant nodes from production upon detection
4. Nodes are destroyed beyond a certain age (e.g. 30 days)

Note:
Q4. Ex: Ooyala uses spot instances, so they get nuked randomly. (or whenever new EC2 base image comes out)  
Capital one - 60 day auto destroy policy  
Nike - 7 days auto destroy  
Poodle got auto fixed in prod while PMs were debating what to do due to 7-day auto destroy policy.  


## Sustaining Operations Culture

1. Automated services stress the production system (e.g. Chaos Monkey)
2. Prodution alerts first notify those who wrote the code
3. Operations, Security, Network, Automation, Testing, and Compliance experts provide developer-friendly tools and coaching to enable development teams

Note:
"Secretly the 5th culture slide"  
Big tech - silicone valley giants, Facebook/Google/Netflix/etc... their best practices are here to inspire best practices  
Q1. stress lab would be considered partially implemented  
Q2. you build it, you run it  
- if you have NOC that's a failure (speak about why)
