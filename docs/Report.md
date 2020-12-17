# SQA Plan
## Purpose
The purpose of this plan is to specify how Software Quality Assuarance will be performed throughout the system. This plan will describe the SQA activities namely the process, methods, standards to be performed and the techniques used to perform those tasks. The plan provides the necessary framework to ensure a consistent approach to software quality assurance throughout the project life cycle. 

## Scope
The scope of this plan applies to all stages of the system testing. It defines the approach that will be used to assess the software to provide insight to the functionality and quality. Adherence to the plan will continue throughout as needed, based on the results of the tests.

## Objective
The SQA teams Objective is to ensure that the product does not deviate from the software specification. The team will analyse the quality of the system at any stage for functionality enhancement and error detecton.

## Roles and Responsibilities of SQA Team Member
|Student No.|Name|Roles|Responsibility|
|:-|:-|:-|:-|
|20127558|Tew Yu Jie|SQA Leader|Manage software quality assurance activities for the project|
|20129070|Lee Ka Shing|SQA Auditor|Perform SQA tasks, report to SQA leader the result of SQA review|
|20015829|Widanage Vinuri De Silva|SQA Auditor|Perform SQA tasks, report to SQA leader the result of SQA review|
|20012422|Nurul Hanna Mohd Azhar |SQA Auditor|Perform SQA tasks, report to SQA leader the result of SQA review|

## SQA Tasks
This section specifies the SQA tasks that are performed. The SQA activities performed relate to the testing of the system. Following are the activities planned:
1. Analysing and understanding the system
2. Identify the test activities to be performed and prepare a test environment for testing
3. Define guidelines for testing
4. Design tests according to the guideline specified in the [testing methodology](#testing-methodology) section of the document
5. Perform testing
6. Perform documentation of test results
   - Use the guideline specified in the [problem reporting and corrective actions](#problem-reporting-and-corrective-actions) section of the document to report any problems
7. Perform SQA reviews and audits

## Standards, Practices, Conventions, and Metrics
This section highlights the standards, practices, conventions, and metrics to be applied to measure the quality of the application.

### Document standards
The IEEE standards, with appropriate modifications, are used as guideline for documentation. The document describes the quality management plan that should be followed by the developers. Document needs to be well-written , spell checked and conforms to the conventions. In this document, MarkDown  is the preferred format for documentation, as it is easily version controlled and view on different platforms. Below is the template we use for test cases:
| Test ID | Scenario Group | Decription | Test Steps | Expected Output | Factors | Remarks |
| :-      | :-             | :-         | :-         | :-              | :-      | :-      |
|ID|Scenario|Desciption of test|Test steps performed|Output|SQA factors|Additional Remarks|

<br>
And below is the template for bug reports:

|Test Case ID|-|
|-|-|
|Test Scenario Group|-|
|Reporting member|-|
|Reporting date|-|
|Summary of bug|-|
|Expected result|-|
|Actual result|-|
|Screenshots|-|
|Priority of bug|-|
|Assigned to|-|
|Action to be taken|-|
|Result after action|-|
<br>

### Coding Standards
Coding standard gives a uniform appearance to the code even though it is written by different engineers. It helps in improving readability and maintainability of the code. The coding standards are as follows.
<br>
Python and JavaScript naming conventions is used throughout the code. The application contains multiple API projects where its either written using Phyton or JavaScript. Hence, naming conventions are followed respectively. The client, which communicates with the API, is written in JavaScript. The usage and creation of a class or variable name should be clear and accurately describes its purpose. Local variables however should be named using camel case which starts with a small letter whereas Global variables should start with a capital letter. Throw statements, or also known as throw an exception is used under each function. If an error occurs, JavaScript will stop and generate an error message. This helps simplify the debugging stage. Next, for better understanding and readability of the code, proper indentation is followed. 

### Testing Standards
Testing helps discovers bugs or defects before delivering the program to the client. This guarantees the quality of the software. Unit testing, integration testing and system testing are done in this software testing. 
<br>
Unit testing should be done during the very early stage of development. Each functions, modules or units are isolated, then tested manually to check whether it is working as intended. Bugs identified are fixed before proceeding to the next phase.
<br>
After the units have been unit tested, integration testing is performed. In this testing, units are integrated one by one until all the units are integrated. This is to ensure they can be incorporated with each other without error, and validate whether the requirements are implemented correctly or not. The testing is done simultaneously with the development as some units are not available to be test at times. The integration tests ends after all the integration test cases has been executed.
<br>
System testing is performed on a complete integrated system. It is carried out on the whole system in the context of either system requirements specifications (SRS) or functional requirements requirements or even both. The testing ends after no critical or priority related bugs are in an open state. If any low or medium priority bugs are in an open state, then it should be implemented with acceptance of customer.

### Metrics
The following are the planned metrics that will be collected, reported, and maintained in the area of software quality assurance:
- Adherence to schedule: Scedules and milestones will be tracked inorder to identify the prcentage of completion of the project.
- Number of software defects found: This reflects the quality of the code. The goal is to produce code that is free of bugs. Any errors found during the testing phase will be recorded according to our test [document standards](#document-standards).
- Software defect turnaround: This calculates the time and resources it takes to correct the identified defects. 
- Size of the code (LOC): The size of the code and lines of code used in each individual element will be used to estimate required testing effort and overall software productivity.
- Programming time(persons-months): Used to estimate testing effort required. 
- Storage Capacity: The storage capacity of the whole system will be used to measure the ease of implementation and productivity.
- Test case statuse: The passed/failed percentage will be recorded during each testing phase.

## Problem reporting and corrective actions
All problems will be reported after each software review or testing is carried out. The leader of the project will review the bug report and determine the severity of the bug (low, medium, high) before passing it to the developer team that is responsible for fixing the bugs found. The developer team will apply the changes to the software according to the severity of bug while making sure there is no collision with any other part of the software. The outcome will be reviewed again to ensure all the bugs are fixed. 

## Tools and technologies used for source code management
Git is used as the version control system to manage the documents and source code of the project. It is installed and maintained on the local system of each team member's devices and provides a self-contained record of the ongoing programming versions. Github is also used as an assist together with Git to allow team collaboration through cloud. GitHub is a code hosting platform that provides Git repository hosting service. It allows the team members to share their codes or documents to each other through remote repository and carry out version control at the same time. A link to our github repository can be found [here](https://github.com/kashing1999/dev-example-flights).

## Testing methodology:
The testing team follows closely alongside every step of the development process. To ensure that all requirements are met and bugs are fixed as soon as possible, several testing methodologies are employed. The testing methodologies that were employed include:
1. Unit testing
2. Integration testing
3. System testing
4. UI testing

### Unit testing
Unit testing is a software testing process which focuses on individual units of source code, such as a functions in a program.  Unit tests are usually written once and reused so that the tests can be automated after a change in the source code. Our team will take a semi-automated approach to unit testing. The purpose of unit testing is to ensure that each unit performs as intended and helps to speed up the debugging process during and after development. Unit tests are white box tests as the test designers have to understand the inputs and outputs of the unit to test it effectively. There are a few guidelines set by our team for unit testing:

1. Unit tests should cover both right and wrong inputs
2. Unit tests should test for the boundary value of a unit
3. Each unit test should be fast and small
4. Each unit test should only cover one unit

### Integration testing
Integration testing should take place after unit testing. It tests the integration of individual software modules to check if they work together when combined. The main purpose of integration testing is to uncover defects present between modules when they are integrated. Hence, integration test is a white box test since testers are required to understand all functions of the code base. The team will take a semi-automated approach in this phase of testing. The follow are guidelines set by our team for integration testing:
1. The team shall use a bottom-up approach to integration testing
2. Unit testing shall be done before integration testing
3. Integration testing should only test for the integration between modules rather than the functionality of the modules.

### System testing
System testing is a black-box testing technique and it does not require internal knowledge of the code. It is done after the integration testing and it mainly emphasises on testing the functionality and features of the software as a whole. Inputs are provided to the system and the outputs are verified according to the expectations stated in the test cases. Test cases are created at the beginning to determine all the aspects to be covered in the system testing. Each test case is written based on the real-time usage of the software. After the execution of all the test cases, any bugs found are documented in the bug report. The follow are guidelines set by our team for integration testing:

1. System tests treats the software as a whole
2. Integration testing shall be done before system testing
3. System test cases should be written from user perspective 
4. Expected output should be included in test cases to be used in verification

### UI testing
UI testing is important to test whether the application performs as expected with respect to user interface behaviour. UI testing is done through the web server, where the visual elements available are manipulated. For testing mobile compatibility, the application is access through the available search engine on mobile. To determine the portability of the application, the application needs to be  accessed through different browsers and operating system. All the available widgets such as dropdown bars and buttons need to be tested to check whether it is working as intended and either it responds to user events such as mouse clicks. Layout of the application should be tested to determine whether the GUI elements aligns and responds accordingly to the resize of the web appplication. Position of GUI elements also need to be tested by accessing the application through different screen resolutions. Therefore, consistency of user interface displayed can be determine regardless of the size of monitor.  By accessing the application through different screen resolutions, the readibility of font used can be tested. This is to determine whether the font type and size used is clear and easy to read. For the purpose of testing the display of error message, leave the origin and destination empty.This error message should be informative so user will be informed of the error made. Followings are guidelines set by our team for UI testing:
1. Check screen validations
2. Check the usability conditions
3. Verify navigations
4. Verify data integrity
5. Verify the input fields and formats
 
## Records – collection, maintenance and retention
Documentation related to SQA is kept for future reference and to be shared with stakeholders. The Software Quality Assurance plan as well as the Test Case Documentation will be collected, maintained, and retained in our Github repository. In addition, the results of the tests will be maintained as quality records for future reference.

<div class="page"/>

# Test cases
## Unit tests
### Front-end
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

<div class="page"/>

### Back-end
| Test ID | Scenario Group | Decription | Test Steps | Expected Output | Factors | Metrics | Remarks |
| -      | -             | -         | -         | -              | -      | -      | -      |
| DB01    |Database setup| Test if get_flight_data.sh script downloads flight data required for database| 1. Open a terminal on the server and<br> change the working directory<br> to the directory containing <br>the `get_flight_data.sh` script <br> 2. Run the script with the command:<br>`bash get_flight_data.sh` | Flight data from 1990 to 2020 is downloaded from database to the same folder as the script | Correctness |Direct,Internal|-|
| DB02    |Database setup| Test if create_and_load.sh script creates a database and the correct tables using the schema in setup.sql with MariaDB and loads the corresponding data into the database | 1. Open a terminal on the server<br>and change the working directory<br> to the directory containing the<br>`create_and_load.sh` script <br> 2. Run the script with the command:<br>`bash create_and_load.sh` <br> `localhost 3306 <db_username>`<br>`<db_password>` | Database with corresponding tables are created and data is loaded into the database | Correctness |Direct,Internal|-|
| API01 | API Request Handling | Test if the API handles an API call to the "/api/airlines" route defined in airlineRoutes.js correctly | 1. Open a terminal on the server <br> 2. Make a web request to the API<br>with the "/airlines" route using curl:<br>`curl -v 'localhost:8080/api/`<br>`airlines'` | The API returns a list of all the airlines and the response header specifies that it is a json file | Correctness<br>Interoperability | Direct,Internal | - |
| API02 | API Request Handling | Test if the API handles an API call to the "/api/airports" route defined in airportsRoutes.js correctly | 1. Open a terminal on the server <br> 2. Make a web request to the API with<br>the"/airports" route using curl:<br>`curl -v 'localhost:8080/api/`<br>`airports'` | The API returns a list of all the airports and the response header specifies that it is a json file | Correctness<br>Interoperability | Direct,Internal | - |
| API03 | API Request Handling | Test if the API handles an API call to the "/api/flights/airlines_stats" route defined in flightsRoute.js correctly | 1. Open a terminal on the server <br> 2. Make a web request to the API<br>with the "/airlines_stats" route using curl:<br>`curl -v 'localhost:8080/api/`<br>`flights/airlines_stats`<br>`?o=LAX&dst=ORD&yf=2014&yt=2019` | The API returns the flights statistics for all airlines from LAX to ORD in JSON format | Correctness<br>Interoperability | Direct,Internal | - |
| API04 | API Request Handling | Test if the API handles an API call to the "/api/flights/airlines_stats" route defined in flightsRoute.js correctly when a month and day is given| 1. Open a terminal on the server <br> 2. Make a web request to the API with the<br>"/airlines_stats" route using curl:<br>`curl -v 'localhost:8080/api/`<br>`flights/airlines_stats`<br>`?o=LAX&dst=ORD&yf=2014`<br>`&yt=2019&m=12&d=1'` | The API returns the flights statistics for all airlines from LAX to ORD on the 1st of December in JSON format | Correctness<br>Interoperability | Direct,Internal | - |
| API05 | API Request Handling | Test if the API handles an API call to the "/api/flights/airlines_stats" route defined in flightsRoute.js when no parameters are given | 1. Open a terminal on the server <br> 2. Make a web request to the API with the<br>"/airlines_stats" route using curl:<br>`curl -v 'localhost:8080/api/`<br>`flights/airlines_stats'` | The API returns an empty JSON object | Correctness<br>Interoperability | Direct,Internal | - |
| API06 | API Request Handling | Test if the API handles an API call to the "/api/flights/airlines_stats" route defined in flightsRoute.js when invalid parameters are given | 1. Open a terminal on the server <br> 2. Make a web request to the API with the <br>"/airlines_stats" route using curl:<br>`curl -v 'localhost:8080/api/`<br>`flights/airlines_stats`<br>`?o=does&dst=notexist&yf=-1`<br>`&yt=1000&m=-1&d=1000'` | The API returns an empty JSON object | Correctness<br>Interoperability | Direct,Internal | Boundary Value Analysis |
| API07 | API Request Handling | Test if the API handles an API call to the "/api/flights/airline_delays" route defined in flightsRoute.js correctly | 1. Open a terminal on the server <br> 2. Make a web request to the API with the<br>"/airline_delays using curl:<br>`curl -v 'localhost:8080/api/`<br>`flights/airline_delays?o=LAX`<br>`&dst=ORD&a=AA&yf=2014&yt=2019'` | The API returns the delay types by percent for American Airlines in JSON format | Correctness<br>Interoperability | Direct,Internal | - |
| API08 | API Request Handling | Test if the API handles an API call to the "/api/flights/airline_delays" route defined in flightsRoute.js correctly when a month and day is given| 1. Open a terminal on the server <br> 2. Make a web request to the API with the<br>"/airline_delays route using curl:<br>`curl -v 'localhost:8080/api`<br>`flights/airline_delays?o=LAX`<br>`&dst=ORD&a=AA&yf=2014&yt=2019`<br>`&m=12&d=1'` | The API returns the delay types by percent for American Airlines on the 1st of December in JSON format | Correctness<br>Interoperability | Direct,Internal | - |
| API09 | API Request Handling | Test if the API handles an API call to the "/api/flights/airline_delays" route defined in flightsRoute.js when no parameters are given | 1. Open a terminal on the server <br> 2. Make a web request to the API with the <br>"/airline_delays" route using curl:<br>`curl -v 'localhost:8080/api/`<br>`flights/airline_delays'` | The API returns an empty JSON object | Correctness<br>Interoperability | Direct,Internal | - |
| API10 | API Request Handling | Test if the API handles an API call to the "/api/flights/airline_delays" defined in flightsRoute.js when invalid parameters are given | 1. Open a terminal on the server <br> 2. Make a web request to the API with the<br>"/airline_delays" route using curl:<br>`curl -v 'localhost:8080/api/`<br>`flights/airline_delays?o=does`<br>`&dst=notexist&a=fake`<br>`&yf=-1&yt=1000&m=-1&d=1000'` | The API returns an empty JSON object | Correctness<br>Interoperability | Direct,Internal | Boundary Value Analysis |
| API11 | API Request Handling | Test if the API handles an API call to the "/api/flights/delays_comparison" route defined in flightsRoute.js correctly | 1. Open a terminal on the server <br> 2. Make a web request to the API with the<br>"/delays_comparison using curl:<br>`curl -v 'localhost:8080/api/`<br>`flights/delays_comparison`<br>`?o=LAX&dst=ORD&a=AA&yf=2014`<br>`&yt=2019'` | The API returns the a comparison of delay types by percent for American Airlines versus all airlines in JSON format | Correctness<br>Interoperability | Direct,Internal | - |
| API12 | API Request Handling | Test if the API handles an API call to the "/api/flights/delays_comparison" route defined in flightsRoute.js correctly when a month and day is given| 1. Open a terminal on the server <br> 2. Make a web request to the API with the<br>"/delays_comparison route using curl:<br>`curl -v 'localhost:8080/api`<br>`flights/delays_comparison`<br>`?o=LAX&dst=ORD&a=AA&yf=2014`<br>`&yt=2019&m=12&d=1'` | The API returns a comparison of delay types by percent for American Airlines versus all airlines on the 1st of December in JSON format | Correctness<br>Interoperability | Direct,Internal | - |
| API13 | API Request Handling | Test if the API handles an API call to the "/api/flights/delays_comparison" route defined in flightsRoute.js when no parameters are given | 1. Open a terminal on the server <br> 2. Make a web request to the API with the<br>"/delays_comparison" route using curl:<br>`curl -v 'localhost:8080/api/`<br>`flights/delays_comparison'` | The API returns an empty JSON object | Correctness<br>Interoperability | Direct,Internal | - |
| API14 | API Request Handling | Test if the API handles an API call to the "/api/flights/delays_comparison" defined in flightsRoute.js when invalid parameters are given | 1. Open a terminal on the server <br> 2. Make a web request to the API with the<br>"/delays_comparison" route using curl:<br>`curl -v 'localhost:8080/api/`<br>`flights/delays_comparison?o=does`<br>`&dst=does&a=notexist&yf=-1`<br>`&yt=1000&m=-1&d=1000'` | The API returns an empty JSON object | Correctness<br>Interoperability | Direct,Internal | Boundary Value Analysis |
| API15 | API Request Handling | Test if the API handles an API call with a route that does not exist correctly | 1. Open a terminal on the server <br> 2. Make a web request to the API with a route that does not exist: `curl -v localhost:8080/api/does/not/exist` | The API returns an empty JSON object | Correctness<br>Interoperability | Direct,Internal | - |
| API16 | API Request Handling | Test if the API handles an API call with no route correctly | 1. Open a terminal on the server <br> 2. Make a web request to the API with no route: `curl -v localhost:8080` | The API returns an empty JSON object | Correctness<br>Interoperability | Direct,Internal | - |

<div class="page"/>

## Integration Tests
| Test ID | Scenario Group    | Decription                                                                                          |  Test Steps | Expected Output | Factors | Metrics | Remarks |
| :-      | :-                | :-                                                                                                  |  :-         | :-              | :-      | :-      | :-      |
| DBAPI-1 | DB-API connection | Tests if API is able to establish a connection with the database with valid credentials             from unit test | 1. Start the API with `npm start` and MariaDB with `sudo systemctl start mariadb`<br> 2. Place the following in .env in the nodejs folder: `DB_HOST=127.0.0.1` <br> `DB_PORT=3306` <br> `DB_USER=<db_username>` <br> `DB_PASS=<db_password>` <br> `DB_NAME=flights` <br> 3. Make a web request to the API using curl: `curl -v localhost:8080/api/airlines`|API returns data which was queried <br>by the database in JSON format|Correctness<br>Security<br>Interoperability|Direct,External||
| DBAPI-2 | DB-API connection | Tests if API is able to establish a connection with the database with no credentials               |1. Start the API with `npm start` and MariaDB with `sudo systemctl start mariadb`<br> 2. Place the following in .env in the nodejs folder: `DB_HOST=127.0.0.1` <br> `DB_PORT=3306` <br> `DB_USER=` <br> `DB_PASS=` <br> `DB_NAME=flights` <br> 3. Make a web request to the API using curl: `curl -v localhost:8080/api/airlines`| From the terminal where npm was started, it should show `ER_ACCESS_DENIED_ERROR`.<br>If a web request is made to the API, the API should return an error|Correctness<br>Security<br>Interoperability|Direct,External||
| DBAPI-3 | DB-API connection | Tests if API is able to establish a connection with the database with invalid credentials           |1. Start the API with `npm start` and MariaDB with `sudo systemctl start mariadb`<br> 2. Place the following in .env in the nodejs folder: `DB_HOST=127.0.0.1` <br> `DB_PORT=3306` <br> `DB_USER=doesnotexist` <br> `DB_PASS=wrongpassword` <br> `DB_NAME=flights` <br> 3. Make a web request to the API using curl: `curl -v localhost:8080/api/airlines`|From the terminal where npm was started, it should show `ER_ACCESS_DENIED_ERROR`|Correctness<br>Security<br>Interoperability|Direct,External||
| DBAPI-4 | DB-API connection | Tests if API will be able to handle an error if the database is offline                             |1. Start the API with `npm start` and make sure MariaDB is off: `sudo systemctl stop mariadb`<br> 2. Place the following in .env in the nodejs folder: `DB_HOST=127.0.0.1` <br> `DB_PORT=3306` <br> `DB_USER=<db_username>` <br> `DB_PASS=<db_pass>` <br> `DB_NAME=flights` <br> 3. Make a web request to the API using curl: `curl -v localhost:8080/api/airlines`|The API should timeout trying to establish a connection with the server|Correctness<br>Security<br>Interoperability|Direct,External||
| APIUI-1 | API-UI connection | Tests if the front end is able to proxy a valid web request to the API|1. Start the API and the UI development server respectively with `npm start`<br>2. Make a web request to the api through the UI server: `curl -v localhost:3000/api/airlines` | The UI server should proxy the request to the API, and proxy the response back to the user, returning a JSON of all airlines|Correctness<br>Interoperability|Direct,External||
| APIUI-2 | API-UI connection | Tests if the front end is able to handle an error when an invalid web request is sent to the API    | 1. Start the API and the UI development server respectively with `npm start`<br>2. Make a web request to the api through the UI server: `curl -v localhost:3000/api/airlines` | An empty JSON body should be proxied from the API through the UI to the user|Correctness<br>Interoperability|Direct,External||
| APIUI-3 | API-UI connection | Tests if the front end is able to handle an error when the API is offline| 1. Start the UI development server with `npm start`, but not the API<br>2. Make a web request to the api through the UI server: `curl -v localhost:3000/api/airlines` |2. UI server should be able to handle the failed connection, returning an empty JSON body|Correctness<br>Interoperability|Direct,External||

<div class="page"/>

## System Tests
| Test ID | Scenario Group | Decription | Test Steps | Expected Output | Factors | Metrics | Remarks |
| :-      | :-             | :-         | :-         | :-              | :-      | :-      | :-      |
| SYS01 | Flight filter (Origin and Destination) | Check the flights data displayed with all the required filter inputs | 1. Select origin of the flight in the filter<br>2. Select destination of the flight in the filter<br>3. Click the search button | Flight data of all airlines should appear in a table | Correctness,<br>Reliability | Direct,<br>External| |
| SYS02 | Flight filter (Origin and Destination) | Check the flights data displayed without all the required filter inputs | 1. Click the search button | None of the flights data are displayed | Correctness,<br>Reliability | Direct,<br>External | |
| SYS03 | Flight filter (Airline) | Check the data for different type of delays in percentage with certain airline selected in the filter | 1. Select origin of the flight in the filter<br>2. Select destination of the flight in the filter<br>3.Select an airline<br>4. Click the search button | Data for different type of delays in percentage for the chosen airline should appear as a pie chart | Correctness | Direct,<br>External | |
| SYS04 | Flight filter (Airline) | Check the data for different type of delays in percentage without certain airline selected in the filter | 1. Select origin of the flight in the filter<br>2. Select destination of the flight in the filter<br>3. Click the search button | No pie chart displayed below the filter | Correctness | Direct,<br>Externall || 
| SYS05 | Flight filter (Airline) | Check the data for comparison between average delays in minutes for certain airline and all the airlines for each delay type with certain airline selected in the filter | 1. Select origin of the flight in the filter<br>2. Select destination of the flight in the filter<br>3.Select an airline<br>4. Click the search button | Data for comparison between average delays in minutes for certain airline and all the airlines for each delay type should appear as a bar graph | Correctness| Direct,<br>External ||
| SYS06 | Flight filter (Airline) | Check the data for comparison between average delays in minutes for certain airline and all the airlines for each delay type without certain airline selected in the filter | 1. Select origin of the flight in the filter<br>2. Select destination of the flight in the filter<br>3. Click the search button | No bar graph displayed below the filter | Correctness | Direct,<br>External ||   
| SYS07 | Flight filter (Range of Dates) | Check the flight data displayed with certain range of dates selected in the filter | 1. Select origin of the flight in the filter<br>2. Select destination of the flight in the filter<br>3. Select the range for years<br>4. Select the month<br>5. Select the day<br>6. Click the search button | Only flight data within the range of dates specified should appear | Correctness | Direct,<br>External ||
| SYS08 | Airline table (Sorting rows) | Sort each row of the airlines in the table according to the column chosen | 1. Select origin of the flight in the filter<br>2. Select destination of the flight in the filter<br>3. Click the search button<br>4. Click on the header of each column<br>5. Double click on the header of each column | 1. Click once on the header of each column sort the row of airlines in ascending order<br>2. Double click on the header of each column sort the row of airlines in descending order | Reliability | Direct,<br>External ||
| SYS09 | Airline table (Pie chart and bar graph) | Check the data for different type of delays in percentage by clicking certain airline in the table | 1. Select origin of the flight in the filter<br>2. Select destination of the flight in the filter<br>3. Click the search button <br>4. Click one of the airline in the table | Data for different type of delays in percentage for the chosen airline should appear as a pie chart | Correctness | Direct,<br>External || 
| SYS10 | Airline table (Pie chart and bar graph) | Check the data for comparison between average delays in minutes for certain airline and all the airlines for each delay type by clicking certain airline in the table | 1. Select origin of the flight in the filter<br>2. Select destination of the flight in the filter<br>3. Click the search button <br>4. Click one of the airline in the table | Data for comparison between average delays in minutes for certain airline and all the airlines for each delay type should appear as a bar graph | Correctness | Direct,<br>External ||
| SYS11 | Browsers Compatability | Check the funtionality and performance of the software on different browsers | 1. Open the web application using different web browser (Chrome, Edge, Firefox, Safari)<br>2. Execute test cases SYS01 to SYS10 | The results for each execution of the test cases should be the same for all web browsers used | Portability | Direct,<br>Externall |
| SYS12 | Operating System Compatability | Check the funtionality and performance of the software on different operating systems | 1. Open the web application using different operating systems (Windows, Mac OS, Linux)<br>2. Execute test cases SYS01 to SYS10 | The results for each execution of the test cases should be the same for all operating systems used | Portability | Direct,<br>External |
| SYS13 | Mobile Compatability | Check the funtionality and performance of the software on mobile devices | 1. Open the web application using a mobile device<br>2. Execute test cases SYS01 to SYS10 | The results for each execution of the test cases should be the same as when testing on a computer | Portability | Direct,<br>External|

<div class="page"/>

# UI tests
| Test ID | Scenario Group | Decription | Test Steps | Expected Output | Factors | Metrics | Remarks |
| :-             | :-      | :-         | :-         | :-              | :-      | :-      | :-      |
|UI01|Mobile Compatibility|Check the compatibility of the user inteface though a mobile|1. Open the web server using a mobile.|The components of the website does not adjust according to the reduced screen size.<br />The user has to scroll horizaontally to view and input information.|Portability|Direct<br />External|-|
|UI02|User Experience|Check the web interface using different browsers|1. Open the interface suing Google chrome <br/> 2. Open the inteface using Safari.  |The user interface appears consistent on different web browsers.|Portability|Direct<br />External|-|
|UI03|User Experience|Check the web interface in different operating systems.|1. Open the interface in a windows OS.<br />2. Open the interface in a Mac OS.|The user interface appears consistent on different Operating Systems.|Portability|Direct<br />External|-|
|UI04|User Experience |Alter the size of the window and check the interface. |1. Reduce the window size and check if the interface components adjusts accordingly<br />2. Increase the window size and check if the interface adjust accordingly.|The components do not adjust to the decreasing window size.<br />2. The componently appear perfectly when the window is at its maximum size.|Portability|Direct<br />External|-|
|UI05|User Interaction|Check the positioning of GUI elements in different screen resolutions.|1. Open the interface in a 13 inch screen.<br />2. Open the interface on a 15 inch screen.|The interface should appear consistent regardless of the size of the monitor.|Correctness|Direct<br />External|-|
|UI06|User Interaction|Check if the font used is readable.|1. Open the interface in a different screens.<br />2. Open the interface on different brightness settings.|The text should be clear and easy to read.|Correctness|Direct<br />External|-|
|UI07|User Interaction|Check if the alignment of the text is proper.|1.Input Los Angeles and chicago as origin and detination airport.<br />2.Input American Airlines as Airline.<br />3. Input 2014 to 2019 as duration.<br />4. Click Search.| The text in the resulting output table should be aligned properly according to each heading.|Correctness|Direct<br />External|-|
|UI08|User Interaction|Check if error messeges are displayed correctly.|1. Click the search button without any input for origin airport.|A clear error message is displayed letting the user know not leave the field as null.|Correctness<br />Maintainability|Direct<br />Internal|-|
|UI09|User Interaction|Input wrong data.|1. Enter Los Angeles International airport for both origin and destination airports.|There will be no data displayed in the output table.|Correctness|-|-|
|UI10|User Interaction|Input null data.|1. Click the search button without any input.| An error messege will be displayed letting the user know not to leave the field as null.|Correctness<br />Maintainability|Direct<br />Internal|-|