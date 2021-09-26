# Description
This project is for generating salary slips of employees using Uipath REFramework.

## Input data
Input data will be retrieved from Input Sheet which will have different details of employees like employee name, ID, basic pay, HRA, loss of pay days etc. This input sheet will be saved in dispatcher project.

## High level process flow
* Dispatcher to read input sheet and upload data to queue.
* Performer to get queue data and perform following activities.
    * Perform validations on input data regarding data type and allowed characters.
    * Calculate different salary components like Provident Fund, TDS, Net salary.
    * Update salary components in salary slip template and convert it to pdf.
    * Send report in end state mentioning number of application exceptions, business exceptions and successful transactions.
