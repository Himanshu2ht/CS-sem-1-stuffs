# Question 1

```bash
import math

def roots():
  print("Enter the required values to get roots of a quadratic equation.")
  a=int(input("Enter coefficient of x^2: "))
  b=int(input("Enter coefficient of x: "))
  c=int(input("Enter value of the constant: "))
  D=b*b-4*a*c
  rootD=math.sqrt(abs(D))
  if D>0:
    print("The roots of the quadratic equation are real and different. They are:")
    print((-b+rootD)/(2*a))
    print((-b-rootD)/(2*a))
  elif D == 0:
    print("The roots of the quadratic equation are real and equal. Their value is:")
    print(-b/(2*a))
  else:
    print("Roots of the quadratic equation are not real.")
    
roots()
```
### Code output-
![FireShot Capture 026 - Trinket_ run code anywhere - trinket io](https://github.com/user-attachments/assets/353b1cd1-c0b7-4650-94f2-cb4e57501648)

# Question 2

### j)
```bash
n=int(input("Enter a number to be checked: "))

def prime(n):
  
  if n==2:
    print("Entered number is prime.")
    return
  if n==1 or n==0:
    print("Not Applicable")
    return

  flag=0
  for i in range(2,int(n**0.5)+1):
    if n%i==0:
      flag=1
      break
    else:
      flag=0
  if flag==0:
    print("Entered number is prime.")
  else:
    print("Entered number is not prime.")
    
prime(n)
```
### Code output-
![FireShot Capture 027 - Trinket_ run code anywhere - trinket io](https://github.com/user-attachments/assets/7f1578ea-a8e7-4d93-81af-d2f6fa18ddcd)

### k)
```bash

```
### Code output-

### l)
```bash

```
### Code output-


