# Lab Report 2
## **Part 1**
## This is my code that I used for StringServer:
![Image](StringServer.png)

### My first implementation of /add-message:
![Image](addMessage1.png)

- In the code, all methods are called in StringServer.java with both classes, as the main method in the String Server class and the handleRequest method in the Handler class are called in this instance
- The main relevant argument that is utilized is the url itself, as it would contain the query to be able to make the changes. The relevant field is the ArrayList str in this case as it gives us a space where we could add the different string phrases we want to add in the server
- The ArrayList is seemingly the only relevant field that does change, as when you keep on inputting different phrases into the url to show on the website the ArrayList becomes larger, as shown in the next instance


### My second implementation of /add-message:
![Image](addMessage2.png)

- Very similar to the first implementation, but it seems to add to the ArrayList as it keeps the first phrase that we had inputted in the url while inputting the phrase I just put in right under the first in a new line.

## **Part 2**
### This is the buggy code that I had chose:
``` 
static void reverseInPlace(int[] arr) 
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }
 ```
##Here is an input that does induce a failure:
```
@Test 
public void testReverseInPlace2() {
    int[] input1 = {3, 2, 1};
    ArrayExamples.reverseInPlace(input1);
    System.out.println(input1);
    assertArrayEquals(new int[]{1, 2, 3}, input1);
	}
```

##Here is an input that doesn’t induce a failure
```
@Test 
public void testReverseInPlace() {
    int[] input1 = { 3 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 3 }, input1);
}
```
