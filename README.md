Remove brackets from an algebraic expression
In this article we will see how to Remove brackets from an equation in Python. User are supposed to enter equation and then we will remove brackets.

In an algebraic expression, brackets show the priority of the operation. If the operator outside the bracket has more precedence than the operator between the operands in the brackets the operation inside the brackets will be performed first and then the output of the operation will be operated with operand outside the brackets.

Python program to Remove brackets from an algebraic expression
Problem
We are required to create a simplified expression by removing brackets from the expressions entered by the user.

Example 1
Input is as follows:(x+y)+(z+q)

String without bracket is: x+y+z+q

Example 2
Input is as follows: (x-y+z)-p+q

String without bracket is: x-y+z-p+q

Example 3
Input is as follows: (a-b)+[c*d]+{e/f}
String without bracket is a-b+c*d+e/f

Algorithm
 

Step 1:- Start.
Step 2:- Take user input.
Step 3:- Initialize an empty string.
Step 4:- Start a for loop.
Step 5:- Check if the character is bracket using its ASCII value.
Step 6:- If the character is not bracket add it to empty string.
Step 7:- Print the String.
Step 8:- End.
Python program to remove brackets from an expression
Run
#take user input
Exp = "(a-b)+[c*d]+{e/f}"
#initialize an empty string 
Equation = ''
#traversing through string
for i in Exp:
    #checking for brackets
    if ord(i) == 41 or ord(i) == 40 or ord(i) == 91 or ord(i) == 93 or ord(i) == 123 or ord(i) == 125:
        #If True
        pass
    else:
        #if False
        #add it to empty String
        Equation = Equation + i
 #print the string
print(' String without bracket is ' + Equation)
Output:
String without bracket is a-b+c*d+e/f
