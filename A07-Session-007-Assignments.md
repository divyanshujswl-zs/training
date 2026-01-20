

**Problem 1**

 Imagine a slice of Customers having attributes (name: string, age: integer, salary: integer). Goal is to implement a simple sorting algorithm (like selection sort or bubble sort \- Keep this part simple) that can sort a list of customers. 

For this, you need to create a function called SortTester() as shown below. SortTester should call your implementation of sort function with right parameters. Note that the sort function should not accept any flag to distinguish between name/age/salary or the order (asc/desc). Note that SortTester will be called by the automated tests and should return a slice of \[\]string containing the names of the customers (after they are sorted)

Type Customer struct {  
    Name string  
    Age int  
    Salary int  
}

// Possible values for attribute: “age”, “name”, “salary”  
// Possible values for direction: “arc”, “desc”  
SortTester(customers \[\]Customer, attribute string, direction string) (names \[\]string)

SortTester(\[\]Customer, “age”, “asc”) \-\> Sorts by ascending order of age  
SortTester(\[\]Customer, “name”, “desc”) \-\> Sorts by descending order of name  
SortTester(\[\]Customer, “salary”, “asc”) \-\> Sorts by ascending order of salary.

Example:

Input: SortHelper({{“Name1”, 45, 10000}, {“Name2”, 65, 5000}, {“Name3”, 32, 5000}}, “age”)  
Output: {Name3, Name1, Name2}

**References:**

1. [https://blog.jetbrains.com/go/2022/11/22/comprehensive-guide-to-testing-in-go/](https://blog.jetbrains.com/go/2022/11/22/comprehensive-guide-to-testing-in-go/)  
2. [https://www.jetbrains.com/guide/go/tutorials/mock\_testing\_with\_go/more\_techniques/](https://www.jetbrains.com/guide/go/tutorials/mock_testing_with_go/more_techniques/)  
3. [https://www.codecentric.de/en/knowledge-hub/blog/gomock-tutorial](https://www.codecentric.de/en/knowledge-hub/blog/gomock-tutorial)  
4. [https://blog.logrocket.com/exploring-go-mocking-methods-gomock-framework/?utm\_source=chatgpt.com](https://blog.logrocket.com/exploring-go-mocking-methods-gomock-framework/?utm_source=chatgpt.com)

