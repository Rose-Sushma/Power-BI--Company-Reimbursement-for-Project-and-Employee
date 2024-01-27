# Power-BI--Company-Reimbursement-for-Project-and-Employee

Below were the instructions follwed and 

1. Import the data and opened the Power Query
2. The expense type column has some spelling and punctuation errors, correct them
3. Project names are not uniform, make it uniform.
3. The Currency column has some missing values, based on the amount, create a new custom column.
Condition: amount >= 1000, = INR; amount < 1000, = USD; else = EURO
Formula: (if [Currency] = null and [Amount] >= 1000 then "INR" else if [Currency] = null and [Amount] < 1000 then "USD" else [Currency] )
4. Normalize the amount column into INR based on the currency column.
5. Create a measure to calculate the sum of reimbursed amount in INR.
6. Use the calculate function and check the total reimbursed amount for Project_B
7. Create a measure to check the count of declined requests.
8. Create a slicer visual for the Project and employee
9. Create a bar chart for employees and reimbursement amount.
10. Create a pie chart for Project vs reimbursement amount
