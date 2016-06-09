<!--
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

<!-- .slide: data-background="images/shaolin-masters.jpg" -->
# Chef DOJO
## DevOps Journey Assessment

Note:
This is a speaker note for the first slide



# Agenda
1. The DevOps Journey
1. DOJO Mechanics
1. Working with People
1. Working with Machines



# The DevOps Journey
1. DevOps Journey Map
1. The Journey Phases
1. What You Get When We Are Done


# DevOps Journey Map
<!-- Insert revised Journey Map picture -->
![alt text](images/journey_map.png)


# The Journey Phases

Multiple phases can and should be worked on in parallel 

The earlier phases evolve significantly as the journey progresses

It's natural to skip or inconsistently implement certain phases, so be aware of problems this causes in the later phases

Note:
As you make progress in advanced areas, such as full-stack-automation, the scope of early phases, such as testing, expands
In order to show value quickly, you will sacrifice compeleteness. This is techical debt. Be aware that as you try to improve your system, you will need to go back and clean up. Revisiting is good!


### What You Get When We Are Done
<!-- Show a completed DOJO sample spider graph -->
<canvas data-chart="radar" data-chart-src="data/phase-report-example.csv" width="500" height="300">
<!--
{
"options": { "scale": { 
               "gridLines": { "color": "#FFF", "zeroLineColor": "#FFF" }, 
               "ticks": { "display": false }, 
               "pointLabels": { "fontSize": "16", "fontColor": "#FFF" }
             }
}            
}
-->
</canvas>


### What You Get When We Are Done
<!-- Show a completed DOJO sample spider graph -->
<canvas data-chart="horizontalBar" data-chart-src="data/question-report-example.csv" width="500" height="300">
<!-- 
{
"options": { 
  "responsive": true, 
  "scales": { 
    "xAxes": [{ "stacked": false }], "yAxes": [{ "stacked": true }]   
  },
  "label": { "fontColor": "#FFF" } 
}
}
-->
</canvas>


# DOJO Mechanics

1. Safety
1. Scoping
1. Goal Setting
1. Our Scale
1. Scoring


# Safety

This is a safe space. All of you should feel free to share openly and honestly without repercussions.

Note:
Make sure to get explicit support for this from the most senior person in the DOJO.


# Scoping

We focus on a service and the people who provide it.

1. Development
1. Operations
1. Management
1. Architecture
1. Testing
1. Security
1. Compliance
1. Release
1. Support


# Goal Setting

In this exercise, we want to assess your current state. After you have that, we want you to agree to a six month goal.


# Our Scale

#### <p style="text-align: left;">0   Not planned</p>
---
#### <p style="text-align: left;">1   Planned</p>
---
#### <p style="text-align: left;">2   Inconsistently implemented in some areas</p>
---
#### <p style="text-align: left;">3   Consistently implemented in some areas</p>
---
#### <p style="text-align: left;">4   Consistently implemented throughout the organization</p>


# Scoring

The sections of the DOJO each have a few statements. For each section, we will follow this process:

1. Individuals score each statement for current state
1. Group shares scores
1. Group discusses any differing scores
1. Consenus on scores
1. Repeat for the goal
