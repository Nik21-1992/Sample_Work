# Power BI Formulas Documentation

## Measures
Attrition = SUMX('HR data',IF('HR data'[Attrition]="Yes",1,0))

Attrition Rate = DIVIDE('Calculated Measures'[Attrition],'Calculated Measures'[Total Employees])*100

average age = AVERAGE('HR data'[Age])

Current Working = 'Calculated Measures'[Total Employees] - 'Calculated Measures'[Attrition]

Total Employees = COUNTROWS('HR data')
