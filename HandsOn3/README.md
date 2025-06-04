In this project, you use the properties and methods of Date objects to create a clock that counts down the time to the start of the new year. The clock will update itself every second and will work for any date of  any year. Because the countdown clock displays only integer values, you will work with the Math.floor() method, which rounds down a calculated value to the next lowest integer. For example, when applied to a value like 38.47, the Math.floor() method will return a value of 38. The clock also needs to determine fractional parts of the days, hours, minutes, and seconds left in the year. To return the fractional part of a value, apply the following expression 
	value= Math.floor(value)
Where value from which to extract the fractional part. When applied to a value of 38.47, this expression will return a value of 0.47. A preview of the clock is shown in Figure 7-51.
1. Use your code editor to open the project07-03_html and project07-03_txt.js files from the js07project03 folder. Enter your name and the date in the comment section of each file and save them as project07-03.html and project07-03.js.
2. Go to the project07-03.html file in your code editor and link the page to the project07-03.js file, deferring the script from loading until after the page loads. Save your changes to the file. 
3. Return to the project07-03.js file in your code editor and add a command that uses the setInterval() method to run the countdown() function every 1000 milliseconds.
4. Create the countdown() function and within the function add the commands specified in steps 5 through 11. 
5. Declare the now variable and use the new Date() object constructor store within it the current date and time. 
6. Apply the toLocaleString() method to the now variable to display the text of the current date and time in the currentTime object. 
7. Declare the newYear variable and use the new Date() object constructor store the date “January 1, 2024.”
8. Use the getFullYear() retrieve the 4 digit year value from the now variable, increase the value by 1 and store the result in the nextYear variable. 
9. Use the setFullYear() method to change the year value of the newYear to the value of the nextYear variable. 
10. Perform the following calculations to determine the days, hours, minutes, and seconds left until the New Year:
    - Calculate the days left by calculating the difference between newYear and now and dividing that difference by 1000*60*60*24. Store the result in the daysLeft variable. 
    - Multiply the fractional part of the daysLeft variable by 24 and store the result in the hrsLeft variable.
    - Multiply the fractional part of the hrsLeft variable by 60 and store the result in the minsLeft variable.
    - Multiply the fractional part of the minsLeft variable by 60 and store the result in the secsLeft variable. 
11. Display the following results in the webpage clock: 
    - Apply the Math.Floor() method to the daysLeft variable and write the result to the text content of the daysLeftBox object.
    - Repeat the previous step for the hrsLeft, minsLeft, and secsLeft variables, storing their results in the hrsLeft, minsLeftBox, and secsLeftBox objects. 
12. Save your changes to the file and open project07-03.html in your web browser. Verify that the web page shows the current date and time and updates the time left in the current year every second. 

