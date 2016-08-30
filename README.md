# dojo quickstart guide

### Objectives: 
- Give a professional assessment in a straight forward, modern, presentation format
- Efficiently record & report on assessment results
- TODO: Persistantly store results in one place
 - while not a current function this will be a future need  

## Setup

### Assumptions: 
- Running from MacBook
- Displaying browser on a large screen
- Recording scores on the laptop directly
- Office 365 (export buttons do not work with Excel 2011)

### Pre-reqs: 
- Nodejs (Tested with Node 6.2 & 6.3.0)
- git
- Chrome

### Let's get started on the cli.
- Download & Install [node](https://nodejs.org/en/) - (`brew install node`)
- `git clone https://github.com/chef-customers/dojo-assessment-guide`
- `cd dojo-assessment-guide`
- `npm install`
- `npm start`
- From Chrome: navigate to http://localhost:8080

## Runtime

### Using reveal.js
- Slides move left to right and top to bottom (Use keyboard arrow keys to move through the deck)
- To display speaker notes: click s

### Using Excel
- Open data/customer.xls
- Enable Macros
- Goto the assessment tab
- When you want to refresh the Radar Chart, click "export phase report". (On first use grant permissions.)
- When you want to refresh the Bar Chart, click "export question report". (On first use grant permissions.)
- If you want to clear the current results, click the reset button at the bottom of the sheet.

### When you're done...  Save as PDF.
- goto http://localhost:8000/index.html?print-pdf#/
- click cmd+p on Mac (cntrl+cmd+p on win)
- open in pdf preview & save report pages

## Suggestions for conducting the assesment.
- Conduct voting in the story sizing manner.
  - count down and have all participants vote at the same time (ready set go... Avoid using 1,2,3 as it mentally seeds a number)
- Copy scoring criteria to the whiteboard when scoring slide is reached.
- Define the scope for the assesement - team, project, product, org, etc..
  - Put scope on the whiteboard next to scoring criteria.
  - Remind participants as needed that all votes are done in the context of their scope
  - Make sure there is enough representation in the room for the chosen scope
- Throughout the assessement:
  - Remind participants, that this is not a grade, this is an assesement of their current state, and the state they can reach in 6 months.
  - Remind participants, that desired state is not the same as achieveable state.
  - Remind participants, that if the current state works for them, it's perfectly fine to have the same value currently, and as a 6 months goal. (even if it's a low number)
- Deadlocks
  - Set a voting limit to avoid deadlocks - for example max of 2 or 3 votes. If limit is reached, pick the lowest number.
  - In deadlocks on future state, ask participants to discuss what they can do to reach that state.
- In there are qustions about what a particular point may mean, start by allowing participants to decide what a particular question means in the context of their scope. Take node of the decision on the margins (it will not break the Excel).
  - If participants still have difficulties, provide examples.
- Make sure to take a break at least every 45 minutes.