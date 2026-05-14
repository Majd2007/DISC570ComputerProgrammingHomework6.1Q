# DISC570ComputerProgrammingHomework6.1Q

## Q1:
a = int(input("enter the first number: "))

b = int(input("enter the second number: "))

c = int(input("enter the third number: "))



def roots(a, b, c):

    return b**2 - 4*a*c
    
if roots(a, b, c) >0:

    print("two real roots")
    
    x_1 = (-b+(b**2 - 4*a*c))/(2*a)
    
    x_2 = (-b-(b**2 - 4*a*c))/(2*a)
    
    print("The roots are: ", x_1, x_2)
    
elif roots(a, b, c) ==0:

    print("one real roots")
    
    x_1 = (-b + (b ** 2 - 4 * a * c)) / (2 * a)
    
    print(x_1)
    
else:

    print("no real roots")

roots(a, b, c)


## Q.2:

numb = int(input("enter a 4 - digit number that is even and does NOT end with a 0: "))

if numb < 1000 or numb%2 == 1 or numb%5==0:

    print("Number not accepted")
    
else:

    print("Thanks!")
    

## Q.3:

def factorial(x):

    if x == 1:
    
        return 1
        
    else:
    
        return x * factorial(x-1)

print(factorial(5))


## Q.4:

AES = int(input("whats your grade in AES? "))

Math = int(input("whats your grade in Math? "))

Physics = int(input("whats your grade in Physics? "))

Programming = int(input("whats your grade in Programming? "))

x = (AES + Math + Physics + Programming)/4

if  AES <0 or Math <0 or Physics < 0 or Programming < 0:

    print("error")

elif x < 60:

    print("you will not progress")

elif x < 40:

    print("you will not pass")

elif x > 40 and x < 60:

    print("you will pass but not progress")

elif x>60:

    print("you will progress")
