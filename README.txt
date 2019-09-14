Question 1:

First line creates a browserHelper object and puts it in a global variable so we 
can use it everywhere. 
The 'new' part
confuses me a bit but i guess it means we're creating an object(?). The rest seems pretty
reasonable for me though.
The browserHelper contains what we need to use the e2e training wheels.

The second line does the same, we put the chai library in a global variable so
we can use it's expect syntax.

Question 2:

I'm guessing firstly that we're about to create a fizzbuzz class. So we're
telling the test to create a fizzbuzz object to be used for the test.
We don't put that inside the it block because then THAT line of code would be tested.
We want to test the object, so we make the test create an instance of the class first
and then test if that instance behaves the way we want it to.


Question 3:

I have googled this several times in the past, and i'm still not really sure
about the specifics. But I know that "===" is basically a stricter version of "==".

For example if x = 1, then x == 1 is true. but true === 1 would output false.
"==" would output true in this case because it would convert one of the types
before comparing them and just look at the "true" value, the "===" operator is 
stricter and doesn't convert the types when comparing, those need to be the same
as well for it to output true.

Question 4:

Because eventually we are gonna have to put the 15 section at the top anyway.
The code needs to check if the number is divisible by 15 before it checks either
3 or 5, because 15 is divisible by both. If the 3 section would appear before the
15 section it would simply return 'Fizz', since it will also be divisible by 3.
Though i don't really understand why we would actually have to move the 5 section.
I think it should work with the order of 15, 3, and then 5?

Question 5:

Unit test:
This tests our code in a more raw way. It tests the logic of our code but not how
a user would interact with it. 

Feature test:
This tests our code from the perspective of a user. The feature test behaves like
a user would more or less on our page, clicks around, types in forms etc.

Question 6:

The browser initializes and goes to our prefered page. Then we tell the test that
before each test it should reload the page. After that, we tell the test to close
our our browser after the tests.

Question 7:

Expectations in testing what we are telling the test what WE want the outcome
to be. So i'm EXPECTING "example" to be equal to "example".

Question 8:

First, we are saying where the source of our JS code is.

Then, we add an event listener to wait for all the content on the DOM to load.
After that, we grab the button using a selector and storing it in a variable.
We also grab the div where the result will be displayed and store that in a 
variable as well.

Then we put an event listener on the button variable and tell it to wait
for 'click'.
After the click, we grab whatever was put inside the input field with 
a selector and store it in a variable.
Then we create an instance of FizzBuzz.
Then we tell the fizzbuzz instance to do it's check function so that
it can check the result of our fizzbuzz game when that particular value
is put in the input field and put that result inside a variable.
After that we take the result and put that inside the div that displays the answer.