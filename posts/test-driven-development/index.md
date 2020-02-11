<!--
.. title: Test-Driven Development
.. slug: test-driven-development
.. date: 2020-02-11 12:52:12 UTC+01:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. type: text
-->

Recently, I've been working through [Obey the Testing Goat!](https://www.obeythetestinggoat.com/), 
a book that covers test-driven development for web-development with Django. 
Test-driven development (TDD) is a development practice in which developers first write tests and then 
write the code that is to be tested. This is in contrast to other practices in which code is tested after being written. 
Though I have encountered testing in the past, test-driven development's emphasis 
on writing tests first and is quite different from the programming styles I have used before.

#### Types of testing 
In software development, two common types of tests are **unit tests** and **functional tests**. 
Functional tests are used to test whether a feature works correctly from the *user's* perspective, 
for example, you may want to write a test to check whether a website displays the correct information, or if a button on a site
works as a it should. Functional tests are concerned with whether the feature being tested
works as it should, instead of whether or not the pieces of underlying code work correctly. Functional tests are often accompanied by a user-centered story that 
makes them readable even to people without a programming background. 

Unit tests, on the other hand, are used to ensure that the *code* works as it should. 
Python has a built-in unittest module that includes helpful tools for writing tests. Django 
also has a django.test.TestCase module which contains some Django-specific features. In TDD,
every line of code should be unit-tested, and unit tests should be written before the code itself, which helps ensure that the developer
understands the purpose of the code before writing it. 

#### The TDD process 

*Obey the Testing Goat* also discusses the *TDD process*, or TDD cycle, which can be summarized as follows:

1. Write a (functional or unit) test 

2. Run the test. If it passes, proceed to step 5, otherwise proceed to step 3.  

3. Identify the reason for the test's failure and write the minimum amount of code needed to fix the error (even if 
the code isn't very well-written)

4. Run the test again, and if it passes proceed to step 5. Otherwise, go back to step 3.

5. Identify code that needs refactoring, and then refactor as necessary. After refactoring,
return to step 2 to ensure that the refactoring didn't inadvertently break the code. If the code does not need refactoring, continue
building the program by returning to step 1 and writing a test for another
piece of 

