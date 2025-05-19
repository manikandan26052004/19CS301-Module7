# 19CS301-Module7
EX: 7.1 RECURSION
### Aim: To Write a Python program to find the sum of square of a first n Natural Numbers using recursion

### Algorithm:
STEP 1: Start.

STEP 2: Define a function.

STEP 3: Create a base case for termination of the function.

STEP 4: Create a recursive case to calculate the result.

STEP 5: Print the result. 

STEP 6: Stop.

### Program:
```
NAME: MANIKANDAN R
REG NO: 212222220022
def s(n):
    if n<=0:
        return 0
    return(n**2+s(n-1))
n=int(input())
print("Result is",s(n))
```
### Output:
![image](https://github.com/gokulkrishnan2005/19CS301-Module7/blob/main/24.png)

### Result: Thus, the given program is implemented and executed successfully .
 

EX: 7.2 TYPES OF RECURSIONS
### Aim: To Write a Python Program to find the sum of all digits in a number using recursion
### Algorithm:
STEP 1: Start.

STEP 2: Define a function.

STEP 3: Create a recursive case in the first line of function for head recursion.

STEP 4: Print the result.

STEP 5: Stop.
### Program:
```
def fun(n):
     if (n >0):
          fun(n - 2)
      print(n-1, end=" ")
x = int(input())
if(x%2==0):
     fun(x)
else:
     fun(x+1)

```
### Output:
![image](https://github.com/user-attachments/assets/c4d6416f-d333-49c1-9dd5-0f774cdabb03)

###Result: Thus, the given program is implemented and executed successfully.
 


EX: 7.3 TAYLOR SERIES

###Aim: To python program to evaluate the series using recursion by collecting the x and n values from the user.
### ALGORITHM:
STEP 1: Start.

STEP 2: Create a variable x and n.

STEP 3: Get the values of x and n from user.

STEP 4: Create a base case and recursive case to calculate the result.

STEP 5: Print the result.

STEP 6: Stop.
### Program:
```
def series(x,n):
         if n==0:
            return 1
         else:
            return x**n/n+series(x,n-1)
x = int(input())
n = int(input())
print(series(x,n))
```
### Output:
![image](https://github.com/user-attachments/assets/1d00b1a4-cecb-466f-8593-805f00d27461)

 
### Result: Thus, the given program is implemented and executed successfully .
 

EX: 7.4 Solve by recursion relation

### Aim: To Write a Python Program to to check and accept the given string if contains all vowels i.e. ‘a’, ‘e’,‘i’.’o’, ‘u’ .

### Algorithm:
 Start.

Define function ispresent(str, l) to check if all elements in list l are in str.

If list l is empty, return True (base case).

If first element l[0] is in str, recursively call ispresent(str, l[1:]).

Input a string from the user.

Call ispresent(str, l) with l = ['a', 'e', 'i', 'o', 'u'].

If it returns True, print "Accepted".

Else, print "Not Accepted"

Stop.

### Program:
```
def ispresent(str,l):
    if len(l)<=0:
        return True
    else:
        if(l[0] in str):
    	    return (True and ispresent(str,l[1:]))
l=["a","e","i","o","u"]
str=input()
if(ispresent(str,l)):
	print("Accepted")
else:
	print("Not Accepted")

```
### Output:
![image](https://github.com/gokulkrishnan2005/19CS301-Module7/blob/main/25.png)

### Result: Thus, the given program is implemented and executed successfully .

EX: 7.1   determine the sum of all elements in the list using recursion:
### Aim: To Write a Python program to  determine the sum of all elements in the list using recursion

### Algorithm:

Start

Define function sum_list(l, length)

If length == 0, return 0 (base case for recursion).

Else, return l[length - 1] + sum_list(l, length - 1) (recursive step).

Create an empty list l.

Read integer n (number of elements).

Loop n times:

Read integer x from user.

Append x to list l.

Call sum_list(l, n) and print the result.

End

### Program:
```
def sum_list(l,length):
    if length==0:
        return l[0]
    return l[length]+sum_list(l,length-1)
    
l=[]
n=int(input())
for i in range(n):
    x=int(input())
    l.append(x)
```
### Output:
![image](https://github.com/gokulkrishnan2005/19CS301-Module7/blob/main/m7n.png)

### Result: Thus, the given program is implemented and executed successfully .
 

