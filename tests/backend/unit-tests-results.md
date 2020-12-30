|Test ID|Actual Output|Steps To Fix|Results after fixing|
|:-|:-|:-|:-|
|API05|Server hangs and nothing is sent back as output|Add a check if parameters are NULL||
|API09|Server hangs and nothing is sent back as output|Add a check if parameters are NULL||
|API10|Nothing is sent back as output|Check if the given number is Nan, if so return json object||
|API13|Server hangs and nothing is sent back as output|Add a check if parameters are NULL||
|API14|Gives null for everything|Check if the given number is NaN, if so return empty json object||