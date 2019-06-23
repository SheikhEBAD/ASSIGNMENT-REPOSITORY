# ASSIGNMENT QUESTIONS WITH ANSWERS

## Q1 Write a Python program which accepts the radius of a circle from the user and compute the area?

## ANSWER

## Calculating Area of Circle

```python
import math
radius = float(input("Enter the Radius of the circle : "))
area = math.pow(radius,2)*math.pi
print("Area of Circle with radius 0.5 is",area)
```
## OUTPUT<br/>
Enter the Radius of the circle : 0.3<br/>
Area of Circle with radius 0.5 is 0.47239816339744

## Q2 Write a Python program to check if a number is positive, negative or zero?

## ANSWER

## Checking numbers if positive, negative or zero

```python
continueRun=True
while(continueRun==True):
    numToCheck=int(input("Enter your Number To Check : "))
    if(numToCheck>0):
        print("Positive Number Entered")
    elif(numToCheck<0):
        print("Negative Number Entered")
    else:
        print("Zero Entered")
    option=input("want to run again?(y/n): ")
    if(option=="y"):
        continueRun=True
    else:
        continueRun=False
```
## OUTPUT<br/>
Enter your Number To Check : -1<br/>
Negative Number Entered<br/>
want to run again?(y/n): y<br/>
Enter your Number To Check : 3<br/>
Positive Number Entered<br/>
want to run again?(y/n): y<br/>
Enter your Number To Check : 0<br/>
Zero Entered<br/>
want to run again?(y/n): n

## Q3 Write a Python program to check whether a number is completely divisible by another number. Accept two integer 
values form the user?

## ANSWER

## Checking divisibility between two numbers

```python
continueRun=True
while(continueRun==True):
    num1=int(input("Enter numerator: "))
    num2=int(input("Enter Denominator: "))
    if (num1%num2==0):
        print("Number "+str(num1)+" is completely divisible by "+str(num2))
    else:
        print("Number "+str(num1)+" is not completely divisible by "+str(num2))
    option=input("want to run again?(y/n): ")
    if(option=="y"):
        continueRun=True
    else:
        continueRun=False
        print("GOOD BYE")
```
## OUTPUT<br/>
Enter numerator: 4<br/>
Enter Denominator: 2<br/>
Number 4 is completely divisible by 2<br/>
want to run again?(y/n): y<br/>
Enter numerator: 2<br/>
Enter Denominator: 4<br/>
Number 2 is not completely divisible by 4<br/>
want to run again?(y/n): n<br/>
GOOD BYE

## Q4 Write a Python program to get the volume of a sphere, please take the radius as input from user?

## ANSWER

## Calculate Volume of a sphere

```python
import math
radius = float(input("Enter the Radius of the sphere : "))
volume = ((4/3)*math.pow(radius,3)*math.pi)
print("Volume of the Sphere with Radius 1 is",volume)
```
## OUTPUT<br/>
Enter the Radius of the sphere : 1<br/>
Volume of the Sphere with Radius 1 is 4.1887902047863905

## Q5 Write a Python program to get a string which is n (non-negative integer) copies of a given string?

## ANSWER

## Copying string to (n) times

```python
string1=input("Enter String: ")
copy1=int(input("How many copies of String you need: "))
print(str(copy1)+" copies of "+string1+" are ",end='')
for i in range(copy1):
    print(string1,end='')
```
## OUTPUT<br/>
Enter String: hello <br/>
How many copies of String you need: 4<br/>
4 copies of hello  are hello hello hello hello

## Q6 Write a Python program to find whether a given number (accept from the user) is even or odd, print out an appropriate 
message to the user?

## ANSWER

## Checking number if Even or Odd

```python
continueRun=True
while(continueRun==True):
    num1=int(input("Enter Number: "))
    if (num1%2==0):
        print(str(num1)+" is Even")
    else:
        print(str(num1)+" is odd")
    option=input("want to run again?(y/n): ")
    if(option=="y"):
        continueRun=True
    else:
        continueRun=False
        print("BYE")
```
## OUTPUT<br/>
Enter Number: 4<br/>
4 is Even<br/>
want to run again?(y/n): y<br/>
Enter Number: 9<br/>
9 is odd<br/>
want to run again?(y/n): n<br/>
BYE

## Q7 Write a Python program to test whether a passed letter is a vowel or not?

## ANSWER

## Checking letters if they are vowels or not

```python
continueRun=True
while(continueRun==True):
    vowel=input("Enter a character : ")
    
    if(vowel == "A" or vowel == "a" or vowel =="E" or vowel =="e" or vowel =="I" or vowel =="i" or vowel =="O" or vowel =="o" or 
    vowel =="U" or vowel =="u"):
        print("Letter "+vowel+" is Vowel")
    else:
        print("Letter "+vowel+" is not Vowel")
```
## OUTPUT<br/>
Enter a character: e<br/>
Letter e is Vowel<br/>
Enter a character: N<br/>
Letter N is not Vowel

## Q8 Write a Python program that will accept the base and height of a triangle and compute the area?

## ANSWER

## Calculating area of Triangle

```python
base=float(input("Enter Base : "))
height=float(input("Enter Height : "))
area=(base*height*0.5)
print("Area of Triangle is: "+str(area))
```
## OUTPUT<br/>
Enter Base : 3<br/>
Enter Height : 4<br/>
Area of Triangle is: 6.0

## Q9 Write a Python program to compute the future value of a specified principal amount, rate of interest, and a number of years?

## ANSWER

## Calculating Interest Value

```python
amount=int(input("Please enter principle amount: "))
rate=float(input("Please enter Rate of intrest in %: "))
year=int(input("Enter number of years for investment: "))
formula= (round(amount * (1+rate)**year,1))
print("After "+str(year)+" years your principle amount "+str(amount)+" over an intrest rate of "+str(rate)+"% will be "+str(formula))
```
## OUTPUT<br/>
Please enter principle amount: 10000<br/>
Please enter Rate of intrest in %: 0.1<br/>
Enter number of years for investment: 5<br/>
After 5 years your principle amount 10000 over an intrest rate of 0.1% will be 16105.1

## Q10 write a Python program to compute the distance between the points (x1, y1) and (x2, y2)?

## ANSWER

## Calculating Euclidean distance

```python
import math
x1 = int(input('Enter Co-ordinate for x1: '))
x2 = int(input('Enter Co-ordinate for x2: '))
y1 = int(input('Enter Co-ordinate for y1: '))
y2 = int(input('Enter Co-ordinate for y2: '))
distance=math.sqrt( (pow((x2-x1),2)+(pow((y2-y1),2) )) )
print("Distance between points ("+str(x1)+","+str(y1)+") and ("+str(x2)+","+str(y2)+")" +" is "+str(distance))
```
## OUTPUT<br/>
Enter Co-ordinate for x1: 2<br/>
Enter Co-ordinate for x2: 4<br/>
Enter Co-ordinate for y1: 4<br/>
Enter Co-ordinate for y2: 4<br/>
Distance between points (2,4) and (4,4) is 2.0

## Q11 Write a Python program to convert height in feet to centimetres?

## ANSWER

## Converting Feet int Centimeter

```python
feet=float(input("Enter Height in Feet:"))
cm=feet*30.48
print("There are "+str(cm)+" cm in "+str(feet)+"ft")
```
## OUTPUT<br/>
Enter Height in Feet:5<br/>
There are 152.4 cm in 5.0ft

## Q12 Write a Python program to calculate body mass index?

## ANSWER

## BMI Calculator

```python
import math
height = int(input("Enter Height in Cm: "))
weight = int(input("Enter Weight in Kg: "))
bmi = round(weight/(pow((height/100),2)),2)
print("Your BMI is " + str(bmi))
```
## OUTPUT<br/>
Enter Height in Cm: 180<br/>
Enter Weight in Kg: 75<br/>
Your BMI is 23.15

## Q13 Write a python program to sum of the first n positive integers?

## ANSWER

## Sum of n Positive Integers

```python
num1=int(input("Enter value of n: "))
sumcal=0
for i in range(1,num1+1):
    sumcal+=i
print("Sum of n Positive integer till "+str(num1)+" is "+str(sumcal))
```
## OUTPUT<br/>
Enter value of n: 5<br/>
Sum of n Positive integer till 5 is 15

## Q14 Write a Python program to calculate the sum of the digits in an integer?

## ANSWER

## Digits Sum of a Number

```python
continueRun=True
while(continueRun==True):
    number = input('Enter a number: ')
    sumcal=0
    temp=None
    for i in number:
        temp=i
        i = int(i)
        sumcal += i
    print('Sum of',end=" ")
    for i in number:
        print(i, end=" ")
        if i!=temp:
            print("+",end=" ")
    print(' is '+str(sumcal))
    option=input("want to run again?(y/n): ")
    if(option=="y"):
        continueRun=True
    else:
        continueRun=False
        print("GOOD BYE")
```
## OUTPUT<br/>
Enter a number: 125<br/>
Sum of 1 + 2 + 5  is 8<br/>
want to run again?(y/n): n<br/>
GOOD BYE

## THANKYOU

# THE END
