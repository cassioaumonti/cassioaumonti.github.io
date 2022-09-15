## Second Blog Post

Hello again,

Project 1 is done (link below) and it was great learning!!

In Project 1, the goal was to work with functions in R and work out the code organization and readability. In summary, there were several tasks that should be done using functions from packages, mainly from *tydiverse* package, and built-in functions present in the base R. These tasks encompassed reading in a .csv file, rename and select some variables, transform the file format from wide to long, work with strings and extract information from them, and encapsulate all these steps into functions.

The main reason one may have to build a function is repetition, in other words, if you have to perform a task multiple times, then building a function is a good idea. With a function one can make the code cleaner and interpretable as opposed to having the same lines of code run copied several times across the script. Obviously nothing comes easily, to build a function the data scientist has to "think generally" and picture many situations that might come up when different situations arise. For example, when working with strings, it is important to keep in mind that the length of the string may change in large data sets (that was the case for project 1). When such an issue comes in, then the concept of "think generally" is clear. Hence, the data scientist must create the function to adapt to that type of changes (the expected ones). There is no way to be prepared for all possible changes that the data set can bring, so you can just throw an error message on screen and you are good to go. This way the user will know what is allowed to do with the function. This type of information is widely used in documentation of packages in R. The main package for this project, *tideyverse*, has lots of examples and explanations in its documentation, It was a good learning experience going through them.

However, I have to say that the most interesting feature that I learned with this project was the concept of class of an object and how to use it to create a generic function in R. As well known, R is an object oriented-programming language and this allows the users to also access features of the system not only related to mathematics or another data analysis. Many packages are created everyday using R and they all use specific class objects to define plotting styles and options according to what the package does. In project 1, this feature was explored such that, it was created "county" and "state" class objects and specific plotting styles and options depending on the object class it is input. The amazing part, however, is that this plotting function is accessed as the usual `plot()` function in R. The difference is that when the plot function reads the input data set, it gets the class of the object and then R assigns the correct plot function for that particular class of object. This means that the user can run `plot()` function for a specific object class and the correct function is assigned. No need for calling the exact function name in this case. For package builders this feature is a hand on the wheel.

Another interesting feature, now from the *readr* package, is to read in files using a URL link. Very useful feature for web scraping. The data scientist working with financial analysis, for example, must know how to download many gigabytes of data from the web without so much effort. There are other ways of doing scraping, but understanding the concept of getting data from online sources is the first step.

I can't wait for project 2. Lots of new and exciting things to come.

Thank you for reaching so far. See you next time.


[Project 1 (download the code)](/Monti_Cassio_Project1_ST558.Rmd)

[Project 1](https://cassioaumonti.github.io/Monti_Cassio_Project1_ST558.html)
