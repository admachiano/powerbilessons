## How to make sense of a spreadsheet with date columns going across the page



One of the most common scenarios for Power BI users is to have a request from someone in your own or another organziation who wants to see a financial spreadsheet in Power BI.



It is extremely common for financial spreadsheets to have a few columns that have some categorical data such as employees or products and then monthly columns that continue horizontally across the page.  The monthly columns contain amounts such as sales quantities or dollars for whichever month they fall under.



Even thought this structure is excellent for humans to read spreadsheets, it doesn't work very well in Power BI.  Power BI works much better when each column represents a different variable.  In this case the variables are whichever categorical information describes the quantities on each row (employee, product, etc.), the month (more precisely the date), and the amount (sales dollars or quantities) for each month.  When dealing with this kind of spreadsheet, the general strategy is to collapse the monthly columns and their amounts into two columns, regardless of how many monthly columns there may be.  One column will represent the month (date) variable and the other will represent the amount variable.



Open the Excel file named **Unpivot Sample1.xlsx**.  You will note this is a very basic spreadsheet with fourteen columns and 22 rows.  The Employee ID column is the categorical column, then 12 monthly columns, and finally, a total column.  The total column isn't important and will be disposed of in Power BI.  



Of the 22 rows, only the top row and the rows with Employee IDs and amounts are useful, the total row at the bottom will also be dropped in Power BI.



If you haven't already, save **Unpivot Sample1.xlsx** to your hard drive and open Power BI.  
