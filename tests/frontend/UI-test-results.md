## UI/UX tests:

<br /> 

| Test ID | Scenario Group | Decription | Test Steps | Expected Output | Factors | Metrics | Results |
| :-             | :-      | :-         | :-         | :-              | :-      | :-      | :-      |
|UI01|Mobile Compatibility|Check the compatibility of the user inteface though a mobile|1. Open the web server using a mobile.|The components of the website does should adjust according to the smaller screen size.<br />The user has to scroll horizontally to view and input information.|Portability|Direct<br />External|Faliure|
|UI02|User Experience|Check the web interface using different browsers|1. Open the interface suing Google chrome <br/> 2. Open the inteface using Safari.  |The user interface appears consistent on different web browsers.|Portability|Direct<br />External|Success|
|UI03|User Experience|Check the web interface in different operating systems.|1. Open the interface in a windows OS.<br />2. Open the interface in a Mac OS.|The user interface appears consistent on different Operating Systems.|Portability|Direct<br />External|Success|
|UI04|User Experience |Alter the size of the window and check the interface. |1. Reduce the window size and check if the interface components adjusts accordingly<br />2. Increase the window size and check if the interface adjust accordingly.|The componently appear perfectly when the window is changed.|Portability|Direct<br />External|Failure|
|UI05|User Interaction|Check the positioning of GUI elements in different screen resolutions.|1. Open the interface in a 13 inch screen.<br />2. Open the interface on a 15 inch screen.|The interface should appear consistent regardless of the size of the monitor.|Correctness|Direct<br />External|Success|
|UI06|User Interaction|Check if the font used is readable.|1. Open the interface in a different screens.<br />2. Open the interface on different brightness settings.|The text should be clear and easy to read.|Correctness|Direct<br />External|Success|
|UI07|User Interaction|Check if the alignment of the text is proper.|1.Input Los Angeles and chicago as origin and detination airport.<br />2.Input American Airlines as Airline.<br />3. Input 2014 to 2019 as duration.<br />4. Click Search.| The text in the resulting output table should be aligned properly according to each heading.|Correctness|Direct<br />External|Success|
|UI08|User Interaction|Check if error messeges are displayed correctly.|1. Click the search button without any input for origin airport.|A clear error message is displayed letting the user know not leave the field as null.|Correctness<br />Maintainability|Direct<br />Internal|Success|
|UI09|User Interaction|Input wrong data.|1. Enter Los Angeles International airport for both origin and destination airports.|There will be no data displayed in the output table.|Correctness|-|Success|
|UI10|User Interaction|Input null data.|1. Click the search button without any input.| An error message will be displayed letting the user know not to leave the field as null.|Correctness<br />Maintainability|Direct<br />Internal|Success|
