# ECNG 3006 Lab 3 Repository

For reference: Lab3Resource.pdf 


Unit testing involves taking a single function and invoking it with a given set of parameters. Then, when the execution finishes, an outcome is checked against the expected result. Code that accomplishes this is called a test case. Checking the outcome is usually done with a form of assertions. For example, assume you have the following function "foo": 

<p> int foo (int a, int b) </p>
<p> { return b–a-1; } </p>
<br>
<p> A test case might look like this: </p>
<p> void test_foo_case_a (){ </p>
<p> int ret; </p>
<p> int ret = foo(1,2); </p>
<p> assert(ret == 0); </p>
<p> } </p>


“Integration Testing” combines different functions and tests them as a group. It also tests the interface between modules and identifies critical defects which are caused due to the integration of different modules. To facilitate incremental integration testing we create stubs (called by Module under test - top-down development) and drivers (that call the module under test - bottom-up development). For example if we wish to call the function foo from inside a task function, we would invoke the task function, and verify that it operates correctly without being scheduled.

System (Verification) Testing establishes that the product meets the functional requirements. For example if we wish to assure that tasks are running within the specified constraints we could utilise task tracking to ensure that the stack does not overflow, and that deadlines are met.

Validation (acceptance) testing establishes that the system meets the user requirements.

Documentation of test results is typically by capturing output files generated via logs. Troubleshooting test failures can also be done using logs, but also by dumping memory upon kernel panic, or by invoking a debugger that will allow the user to "view" the memory and registers at the point of failure.

Modify any project that you have already created, to conduct:

<ol>
          <li> unit testing for any function </li>
          <li> integration testing between the unit tested function and a function that calls the function (you may use a driver function)</li>
          <li> verification testing that determines whether the system meets the functional requirements.</li>
<br>
          
For each exercise, ensure that the output file(s), the appropriately commented source files, test/stub/driver files, and test/final binary files, are part of your github repository.
