# qaf-blank-project-maven

This is automation project skeleton to start with using MAVEN. Please refer [documentaion](https://qmetry.github.io/qaf/) for more help.


This is sample project with Maven directory structure:
 
The 'config' directory contains testng.xml file, and is a place holder for configuration files.

The 'resources' directory contains all required resources including properties files and data files, and is a place holder for other resources.

The 'src' directory contains all java files and is a place holder for other java files.

The 'test-results' directory contains result files.

The 'scenarios' directory is the default place holder for all the scenario files. 


To change/modify dependencies check pom.xml
To run the project, from command prompt go to project home and run mvn. Open dashboard.htm to view results.

Note: This sample project uses chrome driver and it requires chrome driver binary.
You need to download and set webdriver.chrome.driver property in application.properties file with driver binary path.

![Test Results](qtm-result.png?raw=true "Title")

Please refer https://qmetry.github.io/qaf/ 
Thanks,
QAS Team.

* Hierarchy which will be used to parse test result files on QTM. Supprted formats are :-
* JUnit 
  * 1 - Use current Hierarchy in which JUnit Testcase is treated as TestStep and Testsuite is treated as Testcase
  * 2 - Use Junit Testcase as Testcase and link all those (from all testsuites and all files of Junit) to one Testsuite
  * 3 - Create Multiple Testsuites and then link their respective testcases in corresponding Testsuites
* TestNG
  * 1 - Use class as Testcase and test-method as TestStep
  * 2 - Use test-method as Testcase
