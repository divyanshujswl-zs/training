**Session \- 04 \- Golang Control Flow**

***Note:*** 

1. *For each of your program do the following*  
   1. *Create a new branch in your github repo*  
   2. *Create the program and ensure it is working*  
   3. *Ensure to merge your code in **your GitHub** repo, under **development** branch*  
   4. *Also push the code to **Training Repo.***  
      1. *Folder: Additional\_Assignments/\<You name\>*  
      2. *Branch: Additional\_Assignments/\<You name\>*

2. **Exercise 1**  
   1. Read a score in percentage  
   2. Make the program grade the score.  
   3. Create a function which takes the percentage and returns the grade  
      1. \>= 75 → Distinction  
      2. \>= 60 → First Class  
      3. \>= 50 →  Second Class  
      4. \>= 35 → Pass  
      5. Else Fail  
   4. Make sure, the Failure case is first checked and returned  
3. **Exercise 2 \-** if initialization; condition  
   1. Write a function that checks a given number as Even/Odd  
4. **Exercise 3**  
   1. Make a copy of Exercise 1  
   2. Extend the grade function to check for valid range.  
   3. In case of invalid range, return error  
   4. Handle the Error in the main function  
5. **Exercise 4 \- switch**  
   1. The function should take a http error code and return the error message  
6. **Exercise 5 \- switch**  
   1. Write a function to accept log level \- ERROR, WARN, INFO  
      2. On ERROR  
         1. Print message “Sending email to developers”  
      3. On WARN  
         1. Print message “Writing warning Log”  
      4. ON INFO  
         1. Print message “Logging necessary fields for debugging”  
      5. Default  
         1. Print message “No logging”  
   2. In case WARN, both WARN and INFO should be executed  
   3. In case ERROR, all 3, ERROR, WARN and INFO should be executed

7. **Exercise 6 \- For basic syntax**  
   1. Generate numbers from 1 to 100  
   2. Print each number and if it is Even or odd  
8. **Exercise 7 \- For** (like while)  
   1. Write same Even/Odd example using for like while example  
9. **Exercise 8 \- For** \- Infinite  
   1. Write an infinite for loop  
   2. On each loop  
      1. Accept a number  
      2. Print the multiplication table  
      3. Repeat from step 1  
   3. When user presses Ctrl+C, safely exit the program with “Shutting down” message  
10. **Exercise 9 \- For**  
    1. Write a program to print multiplication table from 1 to10  
       1. When product reaches \> 50, skip the rest of the current table   
       2. Start the next table   
11. **Exercise 10 \- For**  
    1. Write a program to print multiplication table from 1 to10  
       1. Print only Even number product results  
12. **Exercise 11**  
    1. Write function01() calling function02() calling function03()  
    2. Make sure each function has 2 defer statements at the beginning  
       1. defer \-\> prints “defering function \<n\>”  
       2. defer \-\> prints “winding down all resources of function \<n\>”  
    3. Make the innermost function panic  
    4. Study the behaviour of all defer statements  
    5. Also study how 2 defers statement behave  
13. **Exercise 12**  
    1. Create a text file with your friends list  
    2. Write a program which which reads **original.txt** and create a copy file **copy.txt**  
    3. Ensure the resources are not leaked  
14. **Exercise 13**  
    1. Create a function which does following  
       1. Receive Cab standard price, as pointer  
       2. Cab Demand: Number of cab requests  
       3. Cab available: Number of cabs available  
       4. Calculate Surge Applied Price  
          1. Surge Factor \=  Demand / Supply  
       5. The surge applied cab price should be updated in the cab price  
    2. Main function should first print base price and then print surge calculated price  
    3. Print enough extra information to verify the calculation

15. **Exercise 14**  
    1. Create a Student structure  
       1. Name   
       2. Roll Number  
       3. Admission Date  
       4. IsSchoolCabinetMember  
       5. Last Logged (In/Out) TimeStamp   
       6. Last Test Score (Percentage)  
    2. Define 2 students and print  
       1. Define student object variables  
       2. Store all its properties  
       3. Write a function to print the data  
       4. Ensure to print the date/time in appropriate format, to provide full data  
    3. Define 2 more students using struct initialization approach  
       1. Print all student data  
16. **Exercise 15**  
    1. Make a copy of Exercise 14, to extend the functionality  
    2. Write a function to update the Last Logged time  
       1. Parameters  
          1. Student struct as pointe  
          2. Time Spend as duration  
       2. Update the Last Logged Time, by adding the duration  
    3. Print student data using the function already created  
17. **Exercise 16**  
    1. Create a 3D point struct (PointID, X, Y, Z coordinates)  
       1. PointID is a string to name the point  
    2. Create 2 point objects without named members  
    3. Create 2 more point objects with named members  
    4. Use a function to print the point and print all the 4 point data  
18. **Exercise 17**  
    1. Create a Vehicle struct  
       1. Make  
       2. Model  
       3. Year   
    2. Create a Car struct  
       1. Has all properties on vehicle (think of best approach)  
       2. Number of Doors  
    3. Cerate Bike struct  
       1. Has all properties on vehicle  
       2. Has Side car  
    4. Create 2 Car objects and print the data  
    5. Create 2 Bike object and print the data

    

19. **Exercise 18**  
    1. Make copy of the **Exercise 17** and extend  
    2. Modify the object create with struct initialization approach

**Additional Resources:**

1. GoDev \- Study Flow control  
   1. [https://go.dev/tour/flowcontrol/1](https://go.dev/tour/flowcontrol/1)

