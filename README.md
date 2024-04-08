# Task-1
This is my first task of python programming intership at CodSoft 
def Addition(x,y):
   return x+y 
def Subtraction(x,y):
    return x-y
def Multiplication(x,y):
    return x*y
def Division(x,y):
    return x/y
print("Select the operation:")
print("1.Addition")
print("2.Subtraction")
print("3.Multiplication")
print("4.Division")
while True:
    operation=input("Enter the operation(1/2/3/4):")
    if operation in ('1','2','3','4'):
        try:
            num1=float(input("Enter first number:"))
            num2=float(input("Enter second number:"))
        except ValueError:
            print("Invalid Input.Try Again")
            continue
        if operation=='1':
            print(num1,"+",num2,"=",Addition(num1,num2))
        elif operation=='2':
            print(num1,"-",num2,"=",Subtraction(num1,num2))
        elif operation=='3':
            print(num1,"*",num2,"=",Multiplication(num1,num2))
        elif operation=='4':
            print(num1,"/",num2,"=",Division(num1,num2))
        next_calculation=input("Continue?(yes/no):") 
        if next_calculation=="no":
            break
        else:
            print("Invalid Input")
