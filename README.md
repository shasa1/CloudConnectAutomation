# User Management API Automation Framework

A simple API automation test suite that verifies functionality of a public user management API 
available at https://m3o.com/user/api.

****************************************************************************

Flows automated as part of the project are as follows -

* Creation of a new user with mandatory fields and verification that it was saved successfully
* Read an existing user
* Update of existing user 
* Deletion of existing user
* Error scenarios, Create a user with duplicated emailID and username information

****************************************************************************

How the Framework works?

AnnotationTransformer class which implements IAnnotationTransformer is reponsible for reading the data from RunManager sheet in testdata.xlsx It sets the annotation of the test methods like description,enabled, priority, dataprovider values read from the excel.

Things to note : Test name in the first column of the excel sheet should match with atleast an @Test available in test classes mentioned in the testng.xml

All the tests will have the same dataprovider in the TestUtils class.

For example the loginTest in RunManager sheet of testdata.xlsx will take the data from TestData sheet which have row where the testname is loginTest.

If there are multiple rows with loginTest as test name , framework will consider it as this as multiple iterations for a test case.





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


