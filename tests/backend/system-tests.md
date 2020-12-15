| Test ID | Scenario Group | Decription | Test Steps | Expected Output | Factors | Metrics | Remarks |
| :-      | :-             | :-         | :-         | :-              | :-      | :-      | :-      |
| SYS01 | Flight filter (Origin and Destination) | Check the flights data displayed with all the required filter inputs | 1. Select origin of the flight in the filter<br>2. Select destination of the flight in the filter<br>3. Click the search button | Flight data of all airlines should appear in a table | Correctness | Direct,<br>Internal| |
| SYS02 | Flight filter (Origin and Destination) | Check the flights data displayed without all the required filter inputs | 1. Click the search button | None of the flights data are displayed | Correctness | Direct,<br>Internal | |
| SYS03 | Flight filter (Airline) | Check the data for different type of delays in percentage with certain airline selected in the filter | 1. Select origin of the flight in the filter<br>2. Select destination of the flight in the filter<br>3.Select an airline<br>4. Click the search button | Data for different type of delays in percentage for the chosen airline should appear as a pie chart | Correctness | Direct,<br>Internal | |
| SYS04 | Flight filter (Airline) | Check the data for different type of delays in percentage without certain airline selected in the filter | 1. Select origin of the flight in the filter<br>2. Select destination of the flight in the filter<br>3. Click the search button | No pie chart displayed below the filter | Correctness | Direct,<br>Internal || 
| SYS05 | Flight filter (Airline) | Check the data for comparison between average delays in minutes for certain airline and all the airlines for each delay type with certain airline selected in the filter | 1. Select origin of the flight in the filter<br>2. Select destination of the flight in the filter<br>3.Select an airline<br>4. Click the search button | data for comparison between average delays in minutes for certain airline and all the airlines for each delay type should appear as a bar graph | Correctness| Direct,<br>Internal ||
| SYS06 | Flight filter (Airline) | Check the data for comparison between average delays in minutes for certain airline and all the airlines for each delay type without certain airline selected in the filter | 1. Select origin of the flight in the filter<br>2. Select destination of the flight in the filter<br>3. Click the search button | No bar graph displayed below the filter | Correctness | Direct,<br>Internal ||   
| SYS07 | Flight filter (Range of Dates) | Check the flight data displayed with certain range of dates selected in the filter | 1. Select origin of the flight in the filter<br>2. Select destination of the flight in the filter<br>3. Select the range for years<br>4. Select the month<br>5. Select the day<br>6. Click the search button | Only flight data within the range of dates specified should appear | Correctness | Direct,<br>Internal ||
| SYS08 | Airline table (Sorting rows) | Sort each row of the airlines in the table according to the column chosen | 1. Select origin of the flight in the filter<br>2. Select destination of the flight in the filter<br>3. Click the search button<br>4. Click on the header of each column<br>5. Double click on the header of each column | 1. Click once on the header of each column sort the row of airlines in ascending order<br>2. Double click on the header of each column sort the row of airlines in descending order | Correctness | Direct,<br>Internal ||
| SYS09 | Airline table (Pie chart and bar graph) | Check the data for different type of delays in percentage by clicking certain airline in the table | 1. Select origin of the flight in the filter<br>2. Select destination of the flight in the filter<br>3. Click the search button <br>4. Click one of the airline in the table | Data for different type of delays in percentage for the chosen airline should appear as a pie chart | Correctness | Direct,<br>Internal || 
| SYS10 | Airline table (Pie chart and bar graph) | Check the data for comparison between average delays in minutes for certain airline and all the airlines for each delay type by clicking certain airline in the table | 1. Select origin of the flight in the filter<br>2. Select destination of the flight in the filter<br>3. Click the search button <br>4. Click one of the airline in the table | Data for comparison between average delays in minutes for certain airline and all the airlines for each delay type should appear as a bar graph | Correctness | Direct,<br>Internal ||
|