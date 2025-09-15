# Project Creation

## Calendar Dimension
* DAX Code to create a Calendar Dimension
* Modelling -> New Table
* And enter the code below 
```dax
Calendar = ADDCOLUMNS(
CALENDARAUTO(),
"Day", DAY([Date]),
"MonthNo", MONTH([Date]),
"MonthName", FORMAT([Date], "mmm"),
"MonthID", FORMAT([Date], "yyyymm"),
"Month", FORMAT([Date], "mmm-yy"),
"MonthStartDate", DATE(YEAR([Date]), MONTH([Date]), 1),
"MonthEndDate", EOMONTH([Date], 0),
"QuarterNo", QUARTER([Date]),
"Quarter", "Q" & QUARTER([Date]),
"Year", YEAR([Date])
)
```

## Ordering the calendar months on a chart in chronological order
* How to Custom Sort Power BI Bar Chart X Axis in a natural Month Order
* [Video Resource](https://www.youtube.com/watch?v=zF2xDm1Rvlg)


## Colors Used
* Red - #E60909  Symbol -  ⬇
* Green - #2EDA4B Symbol - ⬆
* Minor - Green - #0798A6
* Major - Brown - #775E0E
* Major - Red - #D32121

## Resources
* [Video](https://www.youtube.com/watch?v=aVrn8MSuIuI)
* [Icon Download](https://icons8.com/icons)
