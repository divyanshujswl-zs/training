  
**Instructions**

1. Make use of go modules for the above problems.

**Problem 1** 

1. Create a separate package called stack that defines a stack of integers.   
2. Add methods to support Push() and Pop() operations. Pop() should return the top-most value of the stack and a bool to indicate if the value was found or not.   
3. Ensure that the stack’s internals are not accessible from outside the package.

**Problem 2**

1. Create a new package called calculator and define a new type.   
   1. Define methods on the new type to support operations such as add, subtract, multiply and divide.   
   2. Calculator functionalities should be usable from the main package.  
2. Memory support in the Calculator:   
   1. Define new operations such as SetMemory(), AddToMemory(), SubtractFromMemory() and ResetMemory().  
   2. For example,  
      1. SetMemory(5)  
      2. val \= AddToMemory(10) // Should return 15

**Problem 3**

1. Implement a TicTacToe game (No GUI required):  
2. Factory function/Constructor to create a TicTacToe game object. Assume a 3x3 grid.  
3. Define methods to add cross or dot to a grid location. If game is over, this method should return the result.  
4. You should not allow invalid moves (e.g. consecutive ticks or consecutive dots or adding to a already filled location).  
5. Player can start with either cross or dot.

