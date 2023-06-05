# CSE 15l Lab Report 5 - Kiko Pan 

In this lab report, I will be creating a debugging scenario as if it was a discussion post on EdStem. 

## Student Post

**Title:** Need help fixing bug in ListExamples file of lab 7

**Category:** Debugging

**What environment are you using (computer, operating system, web browser, terminal/editor, and so on)**

I am editing the lab7 file that I have cloned into ieng6 server that I opened using VSCode terminal.  

**Detail the symptom you're seeing. Be specific; include both what you're seeing and what you expected to see instead. Screenshots are great, copy-pasted terminal output is also great. Avoid saying “it doesn't work”.**

I was writing my code for ListExamples.java and I wanted to test whether or not my code worked correctly so I ran the ListExamplesTest file using ```sh ./test.sh``` but it gave me an error. It says that I have an error on line 32 and it points at a space. I'm not sure what I did wrong here. 

<p align="center"> <img src = "Screen Shot 2023-06-04 at 10.44.33 PM.png" width = "700" height = "350"> </p>
<p align="center"> <img src = "Screen Shot 2023-06-04 at 11.26.26 PM.png" width = "550" height = "550"> </p>

**Detail the failure-inducing input and context. That might mean any or all of the command you're running, a test case, command-line arguments, working directory, even the last few commands you ran. Do your best to provide as much context as you can.**

I got two error messages when I tried to run my tests and the errors came from line 32. I'm thinking it has something to do with the if statement but I'm not sure exactly what. 

## TA Response

You're on the right track! The bug in your code comes from line 32. In line 32 it looks like you have a conditional statement that starts with if. Have you tried refreshing your memory about how conditional statements are used and formatted? 

## Bug Fixed 

The bug that caused the failing test cases were due to an improper use of if statements. It didn't have any parameters so it failed to run. To fix this, I reread my code to think of what parameter would fit best and the statement and decided that the code would work best with an else statement instead of an if statement. 

<p align="center"> <img src = "Screen Shot 2023-06-04 at 11.27.59 PM.png" width = "750" height = "250"> </p>

<p align="center"> <img src = "Screen Shot 2023-06-04 at 11.28.11 PM.png" width = "550" height = "550"> </p>

## Overview

I used the lab7 file that I had previously cloned because it had test cases and code written for the ListExamples. I first changed my directory to the lab7 directory and used vim to edit the ListExamples.java file where it contained the code I was going to test. The ListExamplesTest.java file was the file that was used to test my code in ListExamples.java. I ran the test file using ```sh ./test.sh``` and realized that I had an error in my code. After reviewing how to use conditional statements as advised by my TA, I realized that my if statement was causing the bug since there was no parameters. Instead of using an if statement, I changed it to else instead so that it didn't require any parameters. To do that, I edited through vim and deleted the ```if``` by hovering over it and pressing ```x``` and then I pressed ```i``` to insert the ```else```. I then exited the insert feature by doing ```esc```. To save and exit vim I typed ```:wq```.

## Part 2 - Reflection 
One thing that I learned during the second half of the quarter was how to log into ssh without requiring a password. I thought that was pretty cool when I first saw you could do that during the skill demo. Another thing was learning about vim commands and being able to edit code within the terminal. I thought it was cool learning how to use vim and the different commands that it has. 
