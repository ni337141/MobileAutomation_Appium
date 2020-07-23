# MobileAutomation_Appium'

This framework is designed on BDD approach and page object model pattern.

Three different src package defined as below src/main/java, src/main/resorces and src/test/java

It contains one bat file 'AutomationFramework' , this bat file is configured with pom and maven goals . Directly we can double click on it and it will start executing all test cases. We can directly run pom file.

reports: Reports contain extentReport.html file with all cucumber steps.

src/main/java:- Contains framework related packages and java file , that all is generic and not application dependent. There are many java files such as configuration and different utilities as per requirement, below points can describe in more depth

Base package:- Base package have Testbase files as base.java and basetest.java, base.java file is main parent file which is being inherited by all other java files. 

BaseTest.java file is child of base.java and it contains setup and launching application configuration other driver related configuration details.

config.properties:- config package contains configreader.java file is resposible for reading global variable defined in globalconfig.properties file.

Listenres:- Listeners contains extent listener for extent report and also testng listener as per our lister requirement and wait for final result of changes.

Utilities:- Utilities will have all differnt utilities such as excelUtil ,DBUtil and LogUtil kind of as per demand of utilites.

LogUtil.java : using for log4j and for logging details of console.

ExtentReport: For generating extent reporting as per test cases.

src/test/java : contains all java file related to testing of application such as pages package, stepDefination package testrunner and jsonTest data.

TestData: used jsonfile for using testdata to enter username and passowrd and other data.

pages: all pages of pageobject model such as loginpage and homepage.

runner: TestRunner responsible for running cucumber using testNG

stepDef: all stepdefination related to feature file

src/main/resources : all nonjava file such as feature file ,Log File,Json test data and properties file.

Config.properties: contains all global variable

Feature file: contains feature file as per bdd steps

JsonData: all json data with details

testNg: testng file for configuring testng runner and listner.


############################################################# End of Document #############################################################
