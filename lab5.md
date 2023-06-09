# Lab Report 5: Debugging Scnario/Reflection

## Part 1: Debugging Scenario
![image](https://github.com/d0min0es/cse15l-lab-reports/assets/130091836/0b0640af-209e-4055-b44f-e2c72c6650fb)

The code that the student was referencingn in their edStem from `ListExamples.java` consists of:

<img width="456" alt="image" src="https://github.com/d0min0es/cse15l-lab-reports/assets/130091836/bb625856-d142-44db-bb30-54a7799bc402">

The bug that showed was:

<img width="560" alt="image" src="https://github.com/d0min0es/cse15l-lab-reports/assets/130091836/42d2ff43-86c3-4afb-8f0d-6f271349ba0b">



## TA Response
Based on the output that you screenshotted, you were expecting to run a series of tests. However, it fails as the array lengths were different. In other words, something in your code is affecting the size of the array and is showing when your test isn't running. By looking at your code, I would check out line 26 of your  code, where the lengths of `index1` and `index2` are different. It might be wise to start the index to 0 instead of 1000 when running it through a loop, when `index1` doesn't starting from that. 

## Student's Response
<img width="569" alt="image" src="https://github.com/d0min0es/cse15l-lab-reports/assets/130091836/e8419bb1-61d6-4ac8-9b7b-395330fcd4b8">


Your suggestion actually really helped me out. Starting index1 at 1000 was affecting the rest of my code as any conditional statements that ran were when `index1` was smaller than `list1`. I was able to fix this by navigating to the edit feature on my terminal using `nano ListExamples.java` so I could make the changes you described above. I then closed and saved my changes and then compiled and ran the tests again to find that they worked. 

## Information Used for the Setup
The file and directory used for this example was from `ListExamples.java` from lab 7. The code of this file used as shown above is this:

<img width="456" alt="image" src="https://github.com/d0min0es/cse15l-lab-reports/assets/130091836/bb625856-d142-44db-bb30-54a7799bc402">

The command line I used to trigger the bug was `cd lab7` for entering the directory, `nano ListExamples.java` to access the code file through the terminal, then changing the size of `index1`. Then after this I saved my changes and then used the following compile and run commands to run the tests in the terminal: 

```
javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java 
java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests
```

## Part 2: Reflection

Something interesting I learned more about within the second half of the quarter from class is the use of if statements from bash script. From parameters to syntax, there are a few nuances that I found interesting compared to if statements we learn in java. Bash script can make performing commands that would usually go on the commmand the line within a script. Learning about a specific aspect of the bash statements like the if statements has showed me once again how many different nuances there are in coding.
