Question 1:

First line creates a browserHelper object and puts it in a global variable so we 
can use it everywhere. 
The 'new' part
confuses me a bit but i guess it means we're creating an object(?). The rest seems pretty
reasonable for me though.
The browserHelper contains what we need to use the e2e training wheels.

The second line does the same, we put the chai library in a global variable so
we can use it's expect syntax everywhere.

Question 2:

I'm guessing firstly that we're about to create a fizzbuzz class. So we're
telling the test to create a fizzbuzz object to be used for the test.
We don't put that inside the it block because then THAT line of code would be tested.
We want to test the object, so we make the test create an instance of the class first
and then test if that instance behaves the way we want it to.