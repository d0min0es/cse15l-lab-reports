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


## Part 2: Reflection

Something interesting I learned more about within the second half of the quarter from class is the use of if statements from bash script. From parameters to syntax, there are a few nuances that I found interesting compared to if statements we learn in java.
