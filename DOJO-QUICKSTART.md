# dojo quickstart guide

## Setup

### Objectives: 
- Give a professional assessment in a straight forward, modern, presentation format
- Efficiently record & report on assessment results
- TODO: Persistantly store results in one place
 - while not a current function this will be a future need  

### Assumptions: 
- Running from MacBook
- Displaying browser on a large screen
- Recording scores on the laptop directly

### Pre-reqs: 
- Nodejs (Tested with Node 6.2)
- git
- Chrome 

### Let's get started on the cli.
- Download & Install [node](https://nodejs.org/en/) 
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
- If you want to clear the current results, click the resest button at the bottom of the sheet.
- When you want to refresh the Radar Chart, click "export phase report"
- When you want to refresh the Bar Chart, click "export question report"

### When you're done...  Save as PDF.
- goto http://localhost:8000/index.html?print-pdf#/
- click cmd+p on Mac (cntrl+cmd+p on win)
- open in pdf preview & save report pages


