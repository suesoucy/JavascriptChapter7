In this project, you will use regular expressions to verify that a password passes validation before it is accepted. In this webform, all proposed passwords must (1) be at least eight characters long, (2) have at least one uppercase letter, (3) have at least one digit, and (4) have at least one of the following symbols, ! @ # $. If the password fails validation, a message indicating the reason for failure should appear in the web form. A preview of the completed project is shown in figure 7-49. 
1. Use your code editor to open the project07-01_txt.html and project07-01_txt.js files from the js07project01 folder. Enter your name and the date in the comment section of each file and save them as project07-01.html and project07-01.js . 
2. Go to the project07-01.html file in your code editor and link the page to the project07-01.js file, deferring the script from loading until after the page loads. Save your changes to the file. 
3. Go to the project07-01.js file in your code editor. Within the event listener for the submit event add commands specified in steps 4, 5, and 6. 
4. Add the e.preventDefault() command to prevent the browser from responding to the submit event. 
5. Create the following variables containing regular expressions: 
    - Create the regex1 variable containing a regular expression literal that matches any single digit. 
    - Create the regex2 variable containing a regular expression literal that matches any single digit. 
    - Create the regex3 variable containing a regular expression with a character class containing the symbols !$#%
6. Create an if else statement that with the following conditions and outcomes:
    -   If the length of pwd is less than 8, set the text content of the feedback object to “your password must be at least 8 characters”.
    - Else if the test() method with the regex1 regular expression applied to the pwd variable returns a false value, set the text content of the feedback object to “your password must contain an uppercase letter”.
    - Else if the test()  method with the regex2 regular expression applied to the pwd returns false, set the text of the feedback to “your password must include a number”. 
    - Else if the test() method with the regex3 regular expression applied to the pwd returns false, set the text of the feedback to “ your password must include one of the following !$#%”. 
    - Otherwise, apply the submit() method to the signupForm object to submit the form for processing. 
7. Save your changes to the file and then load project07-01.html in your web browser. Verify that the form cannot be submitted unless a password is provided that has at least eight characters with at least one uppercase letter, one digit, and one of the following characters !#$%. Also verify that if an invalid password is provided, a text message appears on the webform indicating the reason for failure. 

