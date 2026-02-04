**Command Line Arguments in Python**

Command line arguments are values passed to a Python program when it is run from the command line or terminal.
They allow the program to take input without using input().

Python provides the sys module to handle command line arguments.

sys.argv is a list

It stores all arguments passed from the command line

import sys
print(sys.argv)
----------------------------------------------------------------
First you have import the sys module which is pre install with python package 
then you can write the code
when you have to take the output such as a number or anything 
you can use the sys.argv[position on which you can it should be 1,2,3]
final command would be : num 1 = num1 = int(sys.argv[1])

-> You have to use the command line to run the code in such a way below 
python3 clu.py 3 + 6
where 3 = num1 = int(sys.argv[1])

-----------------------------------------------------------------

```
#command line arg 

import sys

def add(num1, num2):
    return num1 + num2

def sub(num1, num2):
    return num1 - num2

def mul(num1, num2):
    return num1 * num2

num1 = int(sys.argv[1])
sign = sys.argv[2]
num2 = int(sys.argv[3])

if sign == "+":
    print(add(num1, num2))
elif sign == "-":
    print(sub(num1, num2))
elif sign == "*":
    print(mul(num1, num2))
else:
    print("Invalid operator")  ```
------------------------------------------------------------------
