# User Management API Automation Framework

A simple API automation test suite that verifies functionality of a public user management API 
available at https://m3o.com/user/api.

Modular Test Driven Framework

****************************************************************************

Flows automated as part of the project are as follows -

* Creation of a new user with mandatory fields and verification that it was saved successfully
* Read an existing user
* Update of existing user 
* Deletion of existing user
* Error scenarios, Create a user with duplicated emailID and username information

****************************************************************************

Tools/Technologies included are as follows - 

* RestAssured
* Java
* TestNG
* Maven 
* Surefire
* JsonPath
* JsonSmart

****************************************************************************

How the Framework works?

Its a Modular Test Driven Framework, all the test scenarios use '@Test' annotation of TestNG in their respective test files.
The test data is created on the fly for each scenarios and re-used and destroyed at the end of test completion.

The Payload/test data is maintained in a separate json file. There is test data dependency between test file.
Easy to add a test scenario, ease of maintaining the test data.

The framework has custom reporting for additional details on the test cycle.
Having TestNg's default test reporting to view the details/results of test execution

****************************************************************************

How to execute the Tests ?

* Clone the repository to your workspace.
* Build the project using 
* Execute the test using testng.xml directly
		OR
* Execute the command 'mvn clean test' on the CMD prompt or Terminal
* Once the execution completes the result will be available at: 
 
****************************************************************************


### Assignment
Please create a simple test suite that verifies functionality of a public user management API available at https://m3o.com/user/api.

### Some example flows that you could cover in your tests
* Creation of a new user with mandatory/optional fields and verification that it was saved successfully
* Update of existing user 
* Deletion of existing user
* Some error scenarios, like trying to create a user with duplicated id or missing/invalid information

### Our expectations for this task
* Please use Java or Kotlin as programming language and Maven or Gradle as a build tool.
* Use API testing library of your preference (for example, RestAssured, Retrofit or similar).
* Optional: think about reporting or some other way to make test results quick to interpret and test failures easier to investigate.
* Include description of your solution, choice of tools and instruction on how to execute the tests in the readme file.
* Please push your code to the provided git repository and submit your assignment within 5 calendar days.

### Tips
* Let us know if you have any questions - we're happy to help.
* Keep it simple, no need to spend too much time on this task or implement more than 5 test cases.
* Think about easiness of adding new test cases and making changes when building your test suite/framework.
* If there is something you would have improved or done differently if you had more time, please feel free to mention it in the readme file.


