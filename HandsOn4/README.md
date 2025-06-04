In this project you will explore how to apply array methods to add, remove, and search for entries within the array of customer names. A webpage  has been created for you containing web form buttons to engage the different array features. Your task is to create event handlers for those buttons. A preview of the completed page is shown in Figure7-52.
1. Use your code editor to open the project07-04_txt.html and project07-04_txt.js files from the js07project04 folder. Enter your name and the date in the command section of each file and save them as project07-04.html and project07-04.js. 
2. Go to the project07-04.html file in your code editor and link the page to the project07-04.js file, deferring the script from loading until after the page loads. Take some time to study the content and structure of the document. There are four buttons you will need to program for adding, searching for, and removing customer names and another button for removing the top customer from the queue. Save your changes to the file. 
3. Return to the project07-04.js file in your code editor. Add an onClick event handler for the addButton object. Within the event handler do the following: 
    - Use the push() method to add the value of the customerName object to the end of the customers array.
    - Run the generateCustomersList() function to update the contents of the ordered list that appears on the web page. 
    - Change the text of the status paragraph to “customer added to the end of the queue” where customer is the value of the customerName object.
4. Add an onClick event handler for the searchButton object. Within the event handler do the following: 
    - Use the indexOf() method to locate the index of the array item whose value equals the value of the customerName object. Add 1 to the index value and store the result in the place variable. 
    - If place is equal to 0, change the text of the status paragraph to “customer is not found in the queue” where customer is the value of the customerName object, otherwise change the text of the status paragraph to “customer found in position place of the queue” where place is the value of the place variable. 
5. Add an onClick event handler for the removeButton object. Within the event handler, do the following: 
    - Use the indexOf() method to locate the index of the array item whose value equals the value of the customerName object. Store the index in a variable named index. 
    - If index is not equal to -1 then (i) use the splice() method to remove one item from the customers array whose index equal the value of the index variable, (ii) change the text of the status paragraph to “customer removed from the queue”, and (iii) call the generateCustomerList() function to recreate the ordered list of customer names. Otherwise, change the text of the status paragraph to “ customer is not found in the queue”.
6. Add an onClick event handler for the topButton object. Do the following: 
    - Apply the shift() method to remove the first item from the customers array, storing the value returned by the shift() method in the topCustomer variable.
    - Change the text of the status paragraph to “Top customer from the queue” where topCustomer is the value of the topCustomer variable. 
    - Call the generateCustomerList() function.
7. Save your changes to the file and open project07-04.html in your web browser. Do the following tasks to test your code: 
    - Add Alijah Jones to the customer list. Verify that her name appears as the 26th in the entry list. 
    - Search for Gene Bearden and verify that his entry is in the 21st position in the queue
    - Remove John Hilton from the customer list. Verify that the number of customers is reduced back to 25. 
    - Remove the top customer from the list to reduce the customer list to 24 entries.
    - Search for Peter Blake. Verify that the page reports that no such entry can be found in the customer list. 

