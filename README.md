# Code Review – Process and Importance
## __Preparing code for review__
Here are some standard points to keep in mind when preparing your code for review:
- __Always keep the code review in mind:__ When beginning any programming, you should have the code review in mind. So keep your code small. If possible, limit your code to one feature.
- __Make sure that all your tests pass even if your code builds:__ If your code builds but you have failing tests, then deal immediately with what's causing those tests to fail. Then, when the tests pass as expected, you can move on. It is important to make sure that all unit tests are passed, and that end-to-end testing passes all tests. It is important that all testing is complete and gets the green light, since releasing code that works but was a test fail could result in some very unhappy customers when the code goes to production.
- __Remember YAGNI:__ As you code, make sure to only add code that is necessary to meet the requirement or feature you are working on. If you don't need it yet, then don't code it. Only add code when it is needed and not before.
- __Check for duplicate code:__ If your code must be object-oriented and be DRY and SOLID, then review your own code to see whether it contains any procedural or duplicate code. Should it do so, take the time to refactor it so that it is object oriented, DRY, and SOLID.
- __Use static analyzers:__ Static code analyzers that have been configured to enforce your company's best practices will check your code and highlight any issues that are encountered. Make sure that you do not ignore information and warnings. These could cause you issues further down the line.

## __Leading a code review__
![Negative feedback](/imgs/negative_feedback.png "Negative feedback")

*Negative feedback*

![Positive feedback](/imgs/positive_feedback.png "Positive feedback")

*Positive feedback*

## __Knowing what to review__
### __Company's coding guidelines and business requirement(s)__
### __Naming conventions__
Here are a couple of questions that a reviewer should ask
1.	Are the names long enough to be human-readable and understandable?
2.	Are they meaningful in relation to the intent of the code, but short enough to not irritate other programmers?

###	__Formatting__
Here is a set of questions a reviewer should consider asking in their review:
1.	Is code to be indented using spaces or tabs?
2.	Has the correct amount of white space been employed?
3.	Are there any lines of code that are too long that should be spread over multiple lines?
4.	What about line breaks?
5.	Following the style guidelines, is there only one statement per line? Is there only one declaration per line?
6.	Are continuation lines correctly indented using one tab stop?
7.	Are methods separated by one line?
8.	Are multiple clauses that make up a single expression separated by parentheses?
9.	Are classes and methods clean and small, and do they only do the work they are meant to do?

###	__Testing__
When it comes to testing the code, the reviewer should check for the following:
1.	Has the programmer provided tests for all the code?
2.	Is there any code that is untested?
3.	Do all the tests work?
4.	Do any of the tests fail?
5.	Is there adequate documentation of the code, including comments, documentation comments, tests, and product documentation?
6.	Do you see anything that stands out that, even if it compiles and works in isolation, could cause bugs when integrated into the system?
7.	Is the code well documented to aid maintenance and support?

Process Testing

![Prepare test plan from requirements](/imgs/prepare_test_plan_from_requirements.png "Prepare test plan from requirements")

*Prepare test plan from requirements*

### __Performance and security__
Other things that may need to be considered include performance and security:
1.	How well does the code perform?
2.	Are there any bottlenecks that need to be addressed?
3.	Is the code programmed in such a way to protect against SQL injection attacks and denial-of-service attacks?
4.	Is code properly validated to keep the data clean so that only valid data gets stored in the database?
5.	Have you checked the user interface, documentation, and error messages for spelling mistakes?
6.	Have you encountered any magic numbers or hard coded values?
7.	Is the configuration data correct?
8.	Have any secrets accidentally been checked in?

### __Software Development Life Cycle (SDLC)__
![sdlc](/imgs/sdlc.png "sdlc")

*Software Development Life Cycle*

### __Providing and responding to review feedback__

![Peer code review](/imgs/peer_code_review.png "Peer code review")

*Peer code review*


