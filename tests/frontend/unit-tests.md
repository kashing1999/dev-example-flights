## unit tests:
<br /> 


| TestID | Scenario Group | Description | Test Steps | Expected Output | Factors | Metrics| Remarks |
|--------|----------------|-------------|------------|-----------------|---------|--------|--------|
| FE01 | Initial Display | Should show initial display correctly | 1. Open the browser window | Dropdown bars are empty | Correctness | Direct,Internal | - |
| FE02 | Dropdown Bar | Test if Origin bar can be replaced with chosen airport | 1. Select the origin airport | Display chosen origin | Correctness | Direct,Internal | - |
| FE03 | Dropdown Bar | Test if Destination bar can be replaced with chosen airport | 1. Select the destination airport | Display chosen destination | Correctness | Direct,Internal | - |
| FE04 | Dropdown Bar | Test if Airline bar can be  replaced with chosen airline | 1. Select the airline | Display chosen airline | Correctness | Direct,Internal | - |
| FE06 | Dropdown Bar | Test if From bar can be replaced with year between 1990 - 2019 | 1. Hardcode years in FlightsFilter.js <br>2. Select the starting year from browser | Display chosen year | Correctness | Direct,Internal | Boundary Value Analysis |
| FE07 | Dropdown Bar | Test if To bar can be replaced with year between 1990 - 2019 | 1. Hardcode years in FlightsFilter.js <br>2. Select the ending year from browser | Display chosen year | Correctness | Direct,Internal | Boundary Value Analysis |
| FE08 | Dropdown Bar | Test if Month bar can be replaced with any month in January until December | 1. Hardcode months in FlightsFilter.js <br>2. Select the month from browser | Display chosen month | Correctness | Direct,Internal | Boundary Value Analysis |
| FE09 | Dropdown Bar | Test if Day bar can be replaced with any number from 1 until 31 | 1. Hardcode days in FlightsFilter.js <br>2. Select the day from browser | Display chosen day | Correctness | Direct,Internal | Boundary Value Analysis |
| FE09 | Dropdown Bar | Should return to initial when x is clicked on the bar | 1. Click x in the dropdown bar | Bar returns to empty | Correctness | Direct,Internal | - |
| FE10 | Table | Los Angeles International Airport and Chicago O'Hare International Airport should <br>display American Airlines, Spirit Air Lines, United Airlines Inc. Spirit Air Lines,<br> Alaska Airlines Inc, Frontlier Airlines Inc, Virgin America | 1. Hardcode airlines in AirlinesFlightsInfo.js <br>2. Set origin as Los Angeles International Airport <br>and destination as Chicago O'Hare International Airport | Table display airlines | Correctness<br> Integrity | Direct,Internal | - |
| FE11 | Pie Chart | Pie chart represents carrier, late aircraft, NAS, security, weather and other  | 1. Set through AirlineFlightsInfo.js<br>2. Choose airline | Pie Chart display the airlines delay in percentage | Correctness<br> Integrity | Direct,Internal | - |
| FE12 | Bar Graph | Bar graph shows the target and average of carrier, late aircraft, NAS, security, weather and other | 1. Set through AirlineFlightsInfo.js<br>2. Choose airline | Bar graph display the airlines delay | Correctness<br> Integrity | Direct,Internal | - |
| FE13 |User Interaction|Testing origin and destination airport|1. Select the origin airport<br />2. Select the dstination airport|Data will be filtered according to input values|Correctness| Direct,Internal | - |
| FE14 |User Interaction|Leaving origin and destination airport as null|1. Leave origin airport as empty<br />2. Leave destination airport as empty|No table displayed.|Correctness| Direct,Internal | - |
| FE15 |User Interaction|Viewing the month drop down |1. Click on the drop down to view the list of months|List of months from January to December should appear.|Correctness| Direct,Internal | - |
| FE16 |User Interaction|Viewing the year drop down list|1. Click on the drop down list to view|List of years from 1990 to 2019 should be viewable.|Correctness| Direct,Internal | - |
| FE17 |User Interaction|Sorting function|1. Click on the table heading once to sort according to it.<br >2.Click on it a second time to display the results in descending order.|Results are displayed according to the canceled percentage in decending order by default. Users is abe to change it by clicking on required table heading.|Correctness<br />Flexibility| Direct,Internal | - |




