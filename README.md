# Python
Programming in Python
Write python program to print first letter of your name 
a) Example: Peter
               *      *
               *             *
               *              *
               *      *
               *
               *
               *
b) Print your name by using for loop

c) check the user name is palindrome or not


ANSWER:-

A. 
result_str="";    
for row in range(0,7):    
    for column in range(0,7):     
        if (column == 1 or ((row == 0 or row == 3) and column > 1 and column < 5) or (column == 5 and row != 0 and row < 3) or (column == row - 1 and row > 2)):  
            result_str=result_str+"*"    
        else:      
            result_str=result_str+" "    
    result_str=result_str+"\n"    
print(result_str);

b
 name="Rajveer"
 for letters in name:
     print (letters)

c
def palindrome(word):
    x=word.replace(" ","")
    return x==x[::-1]

username = input("Enter your name:-")

if palindrome(username):
    print(f"{username} is a palindrome!")
else:
    print(f"{username} is not a palindrome.")
