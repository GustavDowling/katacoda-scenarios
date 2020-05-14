Now lets set up our test suite. 

We can do this by going into the tests repository.

I have already prepared two test suites for you, to view them, either go into the text editor here in katacoda or run something like: 

"cat TestSuite1"

To make TestSuite1 our testsuite we simply rename TestSuite1 to AppTest.java :

mv TestSuite1 AppTest.java

Now lettuce run the mutation test again.

[code]

We can already see some results on the command line, you should see that it killed x % of mutants and achieved y % code coverage. This is because we have no tests for the "main" class which takes the input, otherwise we would have 100% as you will soon see.

A more detailed log is saved as an HTML file in [fix]. 

Due to Katacoda limitations we can not view the HTML file in this environment, if you copy all the files in the folder at [fix] then you can open the HTML file in your browser. Easier is to just look at the screenshots below, from an HTML report generated using the same test suite and program as you are using. 

image11

Here we see the code and mutation coverage, 

image12



