## unit tests:
<br /> 


| TestID | Scenario Group | Description | Test Steps | Expected Output | Result | Factors | Metrics| Remarks |
|--------|----------------|------------|------------|-----------------|--------|---------|--------|--------|
| FE01 | Initial Display | Should show initial display correctly | 1. Open the browser window | Fields are empty | Success | Correctness | Direct,Internal | - |
| FE02 | Dropdown Bar | Test if Origin bar can be replaced with chosen airport | 1. Select the origin airport | Display chosen origin | Success | Correctness | Direct,Internal | - |
| FE03 | Dropdown Bar | Test if Destination bar can be replaced with chosen airport | 1. Select the destination airport | Display chosen destination | Success  | Correctness | Direct,Internal | - |
| FE04 | Dropdown Bar | Test if Airline bar can be  replaced with chosen airline | 1. Select the airline | Display chosen airline | Success  | Correctness | Direct,Internal | - |
| FE06 | Dropdown Bar | Test if From bar can be replaced with year between 1990 - 2019 | 1. Hardcode years in FlightsFilter.js <br>2. Select the starting year from browser | Display chosen year | Success  | Correctness | Direct,Internal | Boundary Value Analysis |
| FE07 | Dropdown Bar | Test if To bar can be replaced with year between 1990 - 2019 | 1. Hardcode years in FlightsFilter.js <br>2. Select the ending year from browser | Display chosen year | Success | Correctness | Direct,Internal | Boundary Value Analysis |
| FE08 | Dropdown Bar | Test if Month bar can be replaced with any month in January until December | 1. Hardcode months in FlightsFilter.js <br>2. Select the month from browser | Display chosen month | Success | Correctness | Direct,Internal | Boundary Value Analysis |
| FE09 | Dropdown Bar | Test if Day bar can be replaced with any number from 1 until 31 | 1. Hardcode days in FlightsFilter.js <br>2. Select the day from browser | Display chosen day | Success | Correctness | Direct,Internal | Boundary Value Analysis |
| FE09 | Dropdown Bar | Should return to initial when x is clicked on the bar | 1. Click x in the dropdown bar | Fields returns to empty | Success | Correctness | Direct,Internal | - |
| FE10 | Search Button | Should display table, piechart and bar graph | 1. Choose origin, destination and airlines<br> 2. Click the search button   | Display table, piechart, and bar graph | Success | Correctness | Direct,Internal | - |
| FE11 | Table | Los Angeles International Airport and Chicago O'Hare International Airport should display American Airlines,<br> Spirit Air Lines, United Airlines Inc. Spirit Air Lines,<br> Alaska Airlines Inc, Frontlier Airlines Inc, Virgin America | 1. Set through AirlinesFlightsInfo.js <br>2. Set origin as Los Angeles International Airport and destination as Chicago <br>O'Hare International Airport | Table display airlines | Success | Correctness<br> Integrity | Direct,Internal | - |
| FE12 | Pie Chart | Pie chart represents carrier, late aircraft, NAS, security, weather and other  | 1. Set through AirlineFlightsInfo.js<br>2. Choose airline | Pie Chart display the airlines delay in percentage | Success | Correctness<br> Integrity | Direct,Internal | - |
| FE13 | Bar Graph | Bar graph shows the target and average of carrier, late aircraft, NAS, security, weather and other | 1. Set through AirlineFlightsInfo.js<br>2. Choose airline | Bar graph display the airlines delay | Success | Correctness<br> Integrity | Direct,Internal | - |
| FE14 |User Interaction|Testing origin and destination airport|1. Select the origin airport<br />2. Select the destination airport|Data will be filtered according to input values| Success |Correctness| Direct,Internal | - |
| FE15 |User Interaction|Viewing the day drop down |1. Click on the drop down to view list|List of days from 1 to 31 should be viewable| Success |Correctness| Direct,Internal | Boundary Value Analysis |
| FE16 |User Interaction|Viewing the month drop down |1. Click on the drop down to view list|List of months from January to December should appear| Success |Correctness| Direct,Internal | Boundary Value Analysis |
| FE17 |User Interaction|Viewing the year drop down |1. Click on the drop down to view list|List of years from 1990 to 2019 should be viewable| Success |Correctness| Direct,Internal | Boundary Value Analysis |
| FE18 |User Interaction|Sorting function|1. Click on the table heading once to sort according to it.<br >2.Click on it a second time to display the results in descending order.|Results are displayed according to the canceled <br>percentage in decending order by default. Users is able to change it by clicking on required table heading| Success |Correctness<br />Flexibility| Direct,Internal | - |




