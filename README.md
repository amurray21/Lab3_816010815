# ECNG 3006 Lab 3 Repository

For reference: Lab3Resource.pdf 

Unit testing involves taking a single function and invoking it with a given set of parameters. Then, when the execution finishes, an outcome is checked against the expected result. Code that accomplishes this is called a test case. Checking the outcome is usually done with a form of assertions. For example, assume you have the following function "foo": 

<p style="color:red;" >
int foo (int a, int b)
{ return b–a-1; }
A test case might look like this: 

void test_foo_case_a (){
int ret;
ret = foo(1,2);
assert(ret == 0); 
} 
</p>
