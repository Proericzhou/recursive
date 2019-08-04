Fibonacci 
```
def fib(i): 
    '''
    Function to give the number of an index from the fibbonacci sequence
    '''
    #Base Case 1
    if i<0: 
        return -1
    #Base Case 2
    elif i==1: 
        return 0
    #Base Case 3
    elif i==2: 
        return 1
    #recursion
    else: 
        return (fib(i-1) + fib(i-2))
#Testcase
print(fib(9)) 
```
Fibonacci with Input
def fibinput(): 
    '''
    Function to give the number of an index from the fibbonacci sequence with user input
    '''
    i = input("enter in a positive number please")
    #Base Case 1
    if i<0: 
        return -1
    #Base Case 2
    elif i==1: 
        return 0
    #Base Case 3
    elif i==2: 
        return 1
    #recursion
    else: 
        return (fibinput(i-1) + fibinput(i-2))

print(fibinput()) 

Factorial
def fac(x):
   """Function to return the factorial
   of a number"""
   #Base Case
   if x == 1:
       return x
    #Recursion
   else:
       return x * fac(x-1)
#Test Case
print(fac(2))

#Factorial with Input

def facinput(n):
   """Function to return the factorial
   of a number using recursion"""
   #Base Case
   if n == 1:
       return n
    #Recursion
   else:
       return n * facinput(n-1)

#User Input
num = int(input("Enter a number: "))

# check if input is negative
if num < 0:
   print("Sorry, factorial does not exist for negative numbers. :(")
elif num == 0:
   print("The factorial of 0 is 1")
else:
   print("The factorial of",num,"is",facinput(num))

