# Lab Report 2
## **Part 1**
## This is my code that I used for StringServer:
![Image](StringServer.png)

### My first implementation of /add-message:
![Image](addMessage1.png)

- In the code, all methods are called in StringServer.java with both classes, as the main method in the String Server class and the handleRequest method in the Handler class are called in this instance
- The main relevant argument that is utilized is the url itself, as it would contain the query to be able to make the changes. The relevant field is the ArrayList str in this case as it gives us a space where we could add the different string phrases we want to add in the server
- The ArrayList is seemingly the only relevant field that does change, as when you keep on inputting different phrases into the url to show on the website the ArrayList becomes larger, as shown in the next instance
