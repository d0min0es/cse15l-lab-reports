# Lab Report 2

## Part 1: Creating a Web Server
### Code for StringServer
```
import java.io.IOException;
import java.net.URI;

class Handler implements URLHandler {
    // The one bit of state on the server: a number that will be manipulated by
    // various requests.
    StringBuilder sb = new StringBuilder();

    public String handleRequest(URI url) {
        if (url.getPath().equals("/")) {
            return sb.toString();
        } else {
            System.out.println("Path: " + url.getPath());
            if (url.getPath().contains("/add-message")) {
                String[] parameters = url.getQuery().split("=");
                if (parameters[0].equals("s")) {
                    sb.append(parameters[1]).append("\n");
                return sb.toString();
                }
            }
            return "404 Not Found!";
        }
    }
}
    class StringServer {
    public static void main(String[] args) throws IOException {
        if(args.length == 0){
            System.out.println("Missing port number! Try any number between 1024 to 49151");
            return;
        }
        
        int port = Integer.parseInt(args[0]);
        Server.start(port, new Handler());
        
    }
}
```
## Outputs
![Image](screensh1.jpg)

## URL Inputs
![Image](screensh3.jpg)
![Image](screensh2.jpg)

### Screenshot 1 
- The method called in the code shown above for the first screenshot was the handleRequest from the Handler class, which ends up getting called when the server gets a request
- The relevant arguments and field values are `localhost:4000` and `/add-message?s=hello`, which together asks the server to append the string "hello"
- In this context, the only field that impacts what the server output is the stringbuilder sb field which will append a different string followed by `/n` when provided a string argument

### Screenshot 2
- The method called in the code above for the second screenshot was also the handleRequest from the handler class, called when there's a server request
- The relevant arguments and field values are `localhost:4000` and `/add-message?s=how%20are%20you`, which together asks the server to append the string "how are you" and the `%20` is notation for the server to include spaces between the separate string arguments
- The specific request isn't changing any values of any relevant fields from the class because it's simply applying the handleRequest method with the addition of notation to include spaces between strings

## Part 2: Failing Output
![Image](testreverse.jpg)

```
@Test
public void testReversed() {
int[] input1 = {1, 2, 3};
assertArrayEquals(new int[]{3, 2, 1}, ArrayEquals.reversed(input1));

}
```
### Failure-Inducing Output
- One example of a failure-inducing ouput for the `Reverse` method in `ArrayExamples.java` is the input above, `int[] input1 = {1, 2, 3}` which ends up returning an array of all 0's ( `{0, 0, 0}` ) instead of reversing the order of the elements in the provided list.

```
public void testReversed() {
int[] input2 = {0, 0, 0, 0};
assertArrayEquals(new int[]{0, 0, 0, 0}, ArrayEquals.reversed(input2));

}
```
### Non-Failure Inducing Output
- An example of an input that doesn't produce a failure would be a array list like the one given above, `int[] input2 = {0, 0, 0, 0}`

### The Symptom
![Image](testResults.jpg)

### Bug
#### Before
```
static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }
```
#### After
```
static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[arr.length - i - 1];
    }
    return newArray;
  }
```
The issue with the code in the before code that produces a failing test result is that the for loop is assigning reversed values from `newArray` to the original `arr`. Additionally, the method is returning the orginial array, meaning that the values of 0 from `newArray` are replacing the orginal int values in `arr`. 
The way to fix these errors would be to swap `arr[i]` with `newArray[i]`, `newArray[...]` with `arr[...]`, and then changing the return array to `newArray` in order for the new array to get assigned values from the array used in the method parameter

---
## Part 3: Week 2/3 Recap
Something interesting I learned from week 2 of CSE15L lab was that there were three different ieng6 computers could be accessed and they aren't allowed the run the same port at the same time as others using the same computer. Ports are used for computers to relay internet and network messages when connected to a server. Therefore, if several students using an `ieng6-201` computer have to select different port numbers in order to run their web server.
