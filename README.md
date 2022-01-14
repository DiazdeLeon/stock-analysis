
# 1.	Overview of Project: Stock Analysis 2018 vs 2017

<p align="justify"> The purposes of this analysis can be summarized in two parts, the first one will be the analysis of the entire stock market over 2017 and 2018. It will be presented a macro which will help to the user to review the results of the stocks volumes and returns to support a good market decision. 
 
As well as the coding of the macro was refactored to optimize the time of process and to make the code more professional.  
 
In the second part of the analysis, it will be addressed the importance of code refactoring. As an introduction, code refactoring is a way of restructuring and optimizing existing code without changing its external behavior. It is a way to improve the code quality. 

# 2.	Results of stock analysis 2018 vs 2017

 The macro developed has property to choose the analysis year, this means the user can type the year at his/her convenience, in this case was 2017 and 2018. 

       yearValue = InputBox("What year would you like to run the analysis on?")

       Worksheets("All Stocks Analysis").Activate

       range("A1").Value = "All Stocks (" + yearValue + ")"

Secondly the macro has a timer which shows the execution time elapsed.  
 
        startTime = Timer

        endTime = Timer

        MsgBox "This code ran in " & (endTime - startTime) & " seconds for the year " & (yearValue)


The following pictures show a comparison of the stock performance between 2017 and 2018, as well as the execution time elapsed of the original script and the refactored script.
 
 ![image](https://user-images.githubusercontent.com/95872614/149551479-13cc8a9d-400c-494d-bc03-c890ef45c912.png)

<p align="justify"> It is observed that the original code had a mistake or bug in the calculation of the total daily volume of the stocks as well as on their returns. The calculations generated by this code brought the same figures for both years. The elapsed time in the execution for 2017 is 0.613 seconds and for 2018 is 0.574 seconds. 
In this case refactoring the code is applicable and necessary to fix the bug and to optimize the execution elapsed time. After refactoring the code, it is observed that the calculations were executed accurate, and the bug was fixed. Also, the elapsed time of execution was reduced, for 2017 the elapsed time is 9.765 E-02 seconds and 2018 is 6.640 E-02.
 

# 3.	Summary
 
<p align="justify"> Code refactoring helps in removing the complexions and enhancing the reliability of the code. Basically, it is a cycle of continues improvement of the code by different methods to make better. In this case, refactoring the code allowed to fix a bug in the calculations of the daily volume and returns as well as in the reduction of the execution time elapsed. 

**The main objectives of code refactoring are:**
 
-	to enhance the code
-	to eliminate the so-called code smell 
-	to reduced complexity for easier understanding. 

Following the revision of code refactoring it was possible to see the advantages or disadvantages of it. 
 
 **The advantages in general might be summarized as it follows:**
 
-	To make the code easier to understand, meaning to keep the code clean and organized. 
-	To help to find bugs
-	To remove redundancies and duplications improve the effectiveness of the code

**The disadvantages of refactoring code are:**
 
- Time consuming, it can take a lot of time to code refactoring and sometimes the deadline for the submission of the code might be tight.  
- Chance of mistakes, if he person in charge of the refactoring does not have a clear plan or map of the process it might be possible to get loss in the code itself.  
How do these pros and cons apply to refactoring the original VBA script?
-	makes programs run faster,

***Lessons learned during the challenge was that, while refactoring the code I noticed that I had to:***

- Move one step at a time. It was necessary to refactor the code as a baby step modifications. The goal was not to affect the product’s functionality.
- Test. The refactoring process should go hand in hand with tests to make sure the alterations made did not result in new bugs.
- Avoid to add any new function to the code. 
 
Since my experience on this challenge the main disadvantage is that I got lost. There was a point in which I did not know what I was doing. 

As a conclusion, the main purpose of code refactoring is to make the code clean, neat, more efficient, and maintainable.
