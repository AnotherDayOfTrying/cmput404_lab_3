# CMPUT404 Lab 3

## Question 1: What is the link to your github repository for this lab?

https://github.com/AnotherDayOfTrying/cmput404_lab_3

## Question 2: After starting a brand new Django application and running the runserver command, what does the browser show you?

A landing page for django. There was rocket ship on it.

##  Question 3: After creating the first view within polls, what does the browser show you when navigating to / and to /polls respectively?

`/` gives a 404 error
`/polls` show our newly created view

## Question 4: What is a Django migration and why do we need them?

When we create a model the database is not aware of them. To update the database to be able to store our models we must perform a database migration. This creates the appropriate tables to store our models.

## Question 5: What do you see after you log into the Django administration site? From a high level, how do you get custom models to appear in the Django admin page?

We see our models and the information within the database. We can get custom models to appear by registering them.

## Question 6: What do you see when you go to /polls/38/ in your browser? What about /polls/38/results and /polls/38/vote? What happens when you don’t put a number, and instead use a string? How would you modify the urls.py file to allow arbitrary alphabetic characters?

`/polls/38/`: 404 Not Found
`/polls/38/results`: 404 Not Found
`/polls/38/vote`: 404 Not Found
If you use a string instead of a number: 404 Not Found
Using the `str` or `slug` path converters in the path url `i.e. <int:pk> -> <str:pk> or <slug:pk>`

## Question 7: Why is it a bad idea to hardcode urls into the templates?

It always a bad idea to hardcode anything is expected or can change. We do not hardcode URLs into our templates so that we do not need update them when we change any configurations within our app. Instead, they are automatically updated.

## Question 8: What are the benefits of using Django's generic views over writing views 'the hard way'? When should you use a generic view and when shouldn't you use a generic view?

Generic views will handle most of the code for a webpage. You will not need to create a template. You should use a generic view if you need a quick and dirty method to get a view up and running with the bare minimum. Do should not use a generic view if you want a custom webpage, webpage has some complexity to it.
