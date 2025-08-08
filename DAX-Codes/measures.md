### DAX Measures Used in Dashboard

```DAX
Total Employees = DISTINCTCOUNT(Employee[EmployeeID])

Attrition Count = COUNTROWS(FILTER(Employee, Employee[Attrition] = "Yes"))

Attrition Rate = DIVIDE([Attrition Count], [Total Employees], 0)

Average Salary = AVERAGE(Employee[Salary])

Average Age = AVERAGE(Employee[Age])

Years at Company = AVERAGE(Employee[YearsAtCompany])
```