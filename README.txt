Do at least ONE of the following tasks: refactor is mandatory. Write tests is optional, will be good bonus to see it. 
Please do not invest more than 2-4 hours on this.
Upload your results to a Github repo, for easier sharing and reviewing.

Thank you and good luck!



Code to refactor
=================
1) app/Http/Controllers/BookingController.php
2) app/Repository/BookingRepository.php

Code to write tests (optional)
=====================
3) App/Helpers/TeHelper.php method willExpireAt
4) App/Repository/UserRepository.php, method createOrUpdate


----------------------------

What I expect in your repo:

X. A readme with:   Your thoughts about the code. What makes it amazing code. Or what makes it ok code. Or what makes it terrible code. How would you have done it. Thoughts on formatting, structure, logic.. The more details that you can provide about the code (what's terrible about it or/and what is good about it) the easier for us to assess your coding style, mentality etc

And 

Thoughts on the Original Code
The original code has both strengths and areas for improvement:

Strengths:

Modular Approach: The code follows a modular approach by utilizing a repository pattern. This separation of concerns separates data access logic from the controller, promoting maintainability.
Request Handling: The code leverages Laravel's request object to handle incoming HTTP requests, which is a good practice in Laravel development.
Role-Based Logic: It incorporates conditional checks to determine the appropriate response based on user roles, making it flexible for different user types.

Areas for Improvement:
Formatting and Readability: The code lacks consistent formatting, which impacts its readability. Proper indentation, spacing, and consistent brace usage should be enforced for better code comprehension.
Magic Values: There are instances where magic values (e.g., 'true', 'false') are used directly in the code. It's advisable to define these values as constants or use boolean literals for clarity.
Configuration Access: The code uses env to access configuration values. It's recommended to use Laravel's config function for consistency throughout the application.
Code Duplication: Some code is duplicated across different methods. Extracting common functionality into reusable helper methods or consolidating code can reduce duplication and improve maintainability.
Error Handling: Proper error handling and exception handling are lacking in the code. Implementing error-handling mechanisms will ensure graceful error handling and meaningful error messages for users.
Naming Conventions: Consistent naming conventions for variables, methods, and classes should be followed to make the code more cohesive.
Documentation: Inline documentation, especially for complex logic, can improve code maintainability and make it easier for developers to understand.

Refactoring and Test Enhancements
The following changes have been made during the refactoring process:

Utilized Laravel's config function to access configuration values consistently.
Identified and extracted common functionality into reusable helper methods to reduce code duplication.
Implemented proper error handling and exception handling for graceful error handling and meaningful error messages.
Enforced consistent naming conventions for variables, methods, and classes.
Added inline documentation to clarify the purpose of the code and improve maintainability.
Two commits have been made in this repository:

The first commit contains the original code.
The second commit contains the refactored code and test enhancements.
For a detailed view of the changes, please refer to the commits in this repository.

Y.  Refactor it if you feel it needs refactoring. The more love you put into it. The easier for us to asses your thoughts, code principles etc


IMPORTANT: Make two commits. First commit with original code. Second with your refactor so we can easily trace changes. 


NB: you do not need to set up the code on local and make the web app run. It will not run as its not a complete web app. This is purely to assess you thoughts about code, formatting, logic etc


===== So expected output is a GitHub link with either =====

1. Readme described above (point X above) + refactored code 
OR
2. Readme described above (point X above) + refactored core + a unit test of the code that we have sent

Thank you!


