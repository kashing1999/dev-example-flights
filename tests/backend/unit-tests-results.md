|Test ID|Actual Output|Steps To Fix|Results after fixing|
|:-|:-|:-|:-|
|API05|Server hangs and nothing is sent back as output|Add a check if parameters are NULL or undefined|Returns empty JSON object|
|API09|Server hangs and nothing is sent back as output|Add a check if parameters are NULL or undefined|Returns empty JSON object|
|API10|Nothing is sent back as output|Check if the given number is Nan, if so return json object|Returns empty JSON object|
|API13|Server hangs and nothing is sent back as output|Add a check if parameters are NULL or undefined|Returns empty JSON object|
|API14|Gives null for everything|Check if the given number is NaN, if so return empty json object|Returns empty JSON ojbect|