# Lab Report 4

## Step 4 - Log into ieng6

---

<img width="564" alt="Screen Shot 2023-06-07 at 10 27 04 PM" src="https://github.com/d0min0es/cse15l-lab-reports/assets/130091836/11f0e56a-706e-4428-aeb6-2a3cbdbfd7fc">


To log into my ieng6 account, I simply just typed:

`$ ssh cs15lsp23--@ieng6.ucsd.edu <enter>`

in the terminal since `<enter>` allows the terminal to run the command. I was then able to log into my remote account.

## Step 5 - Clone your fork of the repository from your Github account

---

<img width="544" alt="Screen Shot 2023-06-07 at 10 49 28 PM" src="https://github.com/d0min0es/cse15l-lab-reports/assets/130091836/5f99b6d2-e33f-498b-b8b2-1f127e09f9bd">

To clone the repository, I simply copied the link from GitHub and typed:

`$ git clone <link from GitHub> <enter>` 

Since I already have clone this repository, it tells me that the destination path already exists

## Step 6 - Run the tests, demonstrating that they fail

---

<img width="560" alt="Screen Shot 2023-06-07 at 10 54 01 PM" src="https://github.com/d0min0es/cse15l-lab-reports/assets/130091836/c04f094e-dca3-4592-ad19-3542013aea13">


During this step, we expect the tests to fail, but first we would need to compile the files in the directory. In order for me
to get into the right directory, I typed:

`$ cd lab7/` 

which would basically bring me to *lab7* directory. Next, I typed `<Ctrl-C> javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` 
to copy the command and `<Ctrl-V> javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java <enter>` to paste the command into my terminal
in order to compile the files. Afterwards, I did the same thing `<Ctrl-C> java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` to copy and `<Ctrl-V> java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests <enter>` to paste the
command to run tests on the terminal. As we could see on the screenshot above, the output showed that the test has 1 failure. 

---

## Step 7 - Edit the code file to fix the failing test

Now that we know there is one failure on the tests, we can do open a text editor in the terminal by simply typing `$ nano ListExamples.java`. This will allow 
us to edit the code inside the terminal. It should look something like this:

<img width="568" alt="Screen Shot 2023-06-07 at 10 56 49 PM" src="https://github.com/d0min0es/cse15l-lab-reports/assets/130091836/7b48b08f-272a-4d3c-8c38-897dda99ca8f">

To check on what was wrong with the code, I have to type 

`
<down> the # of times needed to find the issue
`

and found out that *index1* was instead supposed to be *index2*, so in order to fix this I have to type `<right><right><right>
<right><right><right><right><right><right><right><right>` to reach to *index1* and `<delete><2>` to change it to *index2*. Finally,
after making all these changes, I typed `<Ctrl-O><enter>` to write and save the changes and `<Ctrl-X>` to exit the nano 
text editor. 

---

## Step 8 - Run the tests, demonstrating that they now succeed

Now that we have finally made changes on the code, it is obvious that we would want to rerun the tests to see if it would pass or not. Since
I have previously typed all those commands in the terminal, this time I simply just need to type `<up><up><up><enter>` to go back to my compile
command then `<up><up><enter>` to run the tests. 

<img width="569" alt="Screen Shot 2023-06-07 at 11 11 40 PM" src="https://github.com/d0min0es/cse15l-lab-reports/assets/130091836/d3c086fc-739b-4e60-8b33-847b6e70af31">

As you could see, all the tests have passed!

---

## Step 9 - Commit and push the resulting change to your Github account 

Since all the tests passed, we can commit and push the file into the *GitHub* repository by typing `$ git add *` to select all the files
in the curretn directory and `$ git commit -m "<updated file>"` to take a snapshot of all the changes made to the file and the message 
that you want to put after changing the file. However I cleared my terminal and already performed the command earlier so the output I got it shown below:

<img width="460" alt="Screen Shot 2023-06-07 at 11 49 26 PM" src="https://github.com/d0min0es/cse15l-lab-reports/assets/130091836/6b5e1e89-1a70-475f-b36b-4993b0847b1f">


Lastly, I typed `$ git push` to forward the changes I made into my repository on GitHub:


![updates](https://github.com/d0min0es/cse15l-lab-reports/assets/130091836/7020da86-5cb3-431a-9844-df86d38fa627)
