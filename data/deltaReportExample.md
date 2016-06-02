## | Organizational Success Factors |  |    Strategic Objectives   |     Tactical Objectives   
1 | The organization's leadership team recognizes IT as a competitive advantage | 1 | _______________________ | _______________________
1 | Clearly defined business champions lead change | 1 | _______________________ | _______________________
1 | Clearly defined technical champions lead change | 1 | _______________________ | _______________________
1 | There is a clear understanding of why the business is undertaking a technology transformation | 1 | _______________________ | _______________________
## | Organizational Culture (Westrum) |  |    Strategic Objectives   |     Tactical Objectives   
1 | Information is actively sought | 1 | _______________________ | _______________________
1 | Responsibilities and risks are shared | 1 | _______________________ | _______________________
1 | Cross-functional collaboration is encouraged and rewarded | 1 | _______________________ | _______________________
1 | New ideas and innovations are welcomed | 1 | _______________________ | _______________________
1 | Failure leads to inquiry | 1 | _______________________ | _______________________
## | Data-Driven Decision Making |  |    Strategic Objectives   |     Tactical Objectives   
1 | The organization's goals are visible to all of its members | 1 | _______________________ | _______________________
1 | Data is collected and used to make decisions | 1 | _______________________ | _______________________
1 | Cost and utilization are monitored | 1 | _______________________ | _______________________
1 | Monitoring data from pre-production environments is used to make release decisions | 1 | _______________________ | _______________________
1 | Monitoring provides business performance information | 1 | _______________________ | _______________________
## | Coding Practices |  |    Strategic Objectives   |     Tactical Objectives   
1 | Every change is reviewed by at least two people with relevant skill and contextual knowledge | 1 | _______________________ | _______________________
## | Working with Machines |  |    Strategic Objectives   |     Tactical Objectives   
## | Version Control |  |    Strategic Objectives   |     Tactical Objectives   
1 | Code documentation is easy to write and is viewable by all with VCS access | 1 | _______________________ | _______________________
## | Chef Local Development |  |    Strategic Objectives   |     Tactical Objectives   
1 | Developers provision their own isolated VMs as needed | 1 | _______________________ | _______________________
1 | Developers use VM images that closely resemble production systems | 1 | _______________________ | _______________________
1 | Developers use Chef development tools (ChefDK, Vagrant, etc) | 1 | _______________________ | _______________________
1 | Chef development workstation setup is automated | 1 | _______________________ | _______________________
1 | Developers download code dependencies in a friction-free manner | 1 | _______________________ | _______________________
1 | Developers run unit tests (ChefSpec) locally | 1 | _______________________ | _______________________
1 | Developers run complaince checks (InSpec) locally | 1 | _______________________ | _______________________
## | Continuous Integration |  |    Strategic Objectives   |     Tactical Objectives   
1 | The CI service automatically tests new branches | 1 | _______________________ | _______________________
1 | CI job templates exist for each type of software project (Chef cookbook, Java app servers, Node.js app, etc.) | 1 | _______________________ | _______________________
1 | CI jobs execute functional tests against projects | 1 | _______________________ | _______________________
1 | CI jobs verify complaince of projects | 1 | _______________________ | _______________________
1 | CI makes the quality of the code base highly visible | 1 | _______________________ | _______________________
1 | CI confirms that versions are unique | 1 | _______________________ | _______________________
1 | CI jobs automatically update dependencies | 1 | _______________________ | _______________________
1 | CI jobs use monitoring to assess each change's effect on system health | 1 | _______________________ | _______________________
## | Chef Code Deployment |  |    Strategic Objectives   |     Tactical Objectives   
1 | CI jobs upload cookbooks to a Chef server | 1 | _______________________ | _______________________
1 | All non-cookbook Chef policy (environments, roles, data bags, etc.) is only uploaded via CI | 1 | _______________________ | _______________________
1 | CI jobs pin dependencies so that they cannot be modified in later deployments | 1 | _______________________ | _______________________
1 | CI jobs assign a set of cookbook versions to a Chef environment | 1 | _______________________ | _______________________
## | Application Deployment |  |    Strategic Objectives   |     Tactical Objectives   
1 | Applications are deployed without manual intervention | 1 | _______________________ | _______________________
1 | Applications follow a clear promotion path (e.g., Dev -> QA -> Staging -> Production) | 1 | _______________________ | _______________________
1 | CI jobs automatically update, pin, and test runtime dependencies of applications | 1 | _______________________ | _______________________
1 | Deployments are run during the business day without causing negative user experiences | 1 | _______________________ | _______________________
## | Continuous Delivery |  |    Strategic Objectives   |     Tactical Objectives   
1 | Small batches of work flow through the pipeline | 1 | _______________________ | _______________________
1 | Changes are released weekly, if not more frequently | 1 | _______________________ | _______________________
## | Virtualizaton as a Service |  |    Strategic Objectives   |     Tactical Objectives   
1 | All servers are provisioned via APIs | 1 | _______________________ | _______________________
1 | The API is a generally accepted API such as EC2, Azure, OpenStack, vSphere, Docker | 1 | _______________________ | _______________________
1 | Access restrictions allow authorized users (e.g., developers and operations) to provision resources, and deny unauthorized users | 1 | _______________________ | _______________________
1 | Resources are provisioned in a friction-free manner | 1 | _______________________ | _______________________
1 | System images are built in a pipeline | 1 | _______________________ | _______________________
## | Full-Stack Automation |  |    Strategic Objectives   |     Tactical Objectives   
1 | The entire application is test provisioned and deployed in an alternate datacenter | 1 | _______________________ | _______________________
## | Compliance Automation |  |    Strategic Objectives   |     Tactical Objectives   
1 | Compliance policies are expressed in code | 1 | _______________________ | _______________________
1 | Compliance is checked automatically | 1 | _______________________ | _______________________
1 | Compliance automation removes non-compliant nodes from production upon detection | 1 | _______________________ | _______________________
## | Sustaining Operations Culture |  |    Strategic Objectives   |     Tactical Objectives   
1 | Prodution alerts first notify those who wrote the code | 1 | _______________________ | _______________________
1 | Operations, Security, Network, Automation, Testing, and Compliance experts provide developer-friendly tools and coaching to enable development teams | 1 | _______________________ | _______________________
