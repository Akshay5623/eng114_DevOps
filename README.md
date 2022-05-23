# eng114_DevOps
My repo for my DevOps work

# Git bash shell commands

- pwd = check whats in the directory
- cd = change directory
- cd .. = go back one directory
- ls = list whats in directory
- la -a - this shows all the hidden files as well
- mkdir = make directory
- rmdir = remove directory
- code = opens in vs code
- program name --version = check what version of a program you are using
- git help = gives a list of commands
- git init = initalises the repo
- git branch -m master main = changes name of branch from master to main. This is a good habit to get into.
- touch = create a file
- nano = edit that file
- how to save a nanofile = ctrl+x, y, enter
- git add = puts file in a queue to be pushed
- git commit -m "enter message here " = commit with a message, should say what the update is.
- git log = see the commits
- press q if stuck in git log to exit it.
- git pull origin branchname --allow-unrelated-histories = this can help if there is 2 files that are the same on a local repo and a github repo
- git push origin main = push the files to the repo
- git reset --hard - helps to restore an accidentally deleted file
- git clean -fxd -
- git checkout -b branchname = create and change to a new branch called e.g dev
- git checkout branchname = change to whatever branch selected
- git diff = see what the differences are between work
- git add . = adds everything in the folder
- git clone = clone a repository.
- cp name of file you want to coopy name of file you want to create - its a copy and paste essentially.

 PUT ALL FILES YOU WANT TO HIDE IN A .gitignore FILE SO IT DOESNT GET PUSHED TO THE REPO

# Python Notes

hi = "Hello World!"
print(hi) = prints the value of hi
print(type(hi)) = shows the data type of the variable

First Task - get the user to enter name, age and date of birth and then print it to the terminal
name = input("Please enter your name: ")
age = input("Please enter your age: ")
dob = input("Please enter your date of birth: ")

print(name)
print(age)
print(dob)

Operators

number3 = 45.j - this is a complex type, shouldn't need but good to know
print(type(number3))
long numbers no longer exist in python from version 3 onwards

float_num = 1.365
int_num = 4
print(float_num + int_num) - this shows that different numerical operators can interact with each other

Strings
Can use single or double quotes, try to keep consistency throughout
Try to use double quotes as there can be issues when you need to use an apostrophe
Can use single quotes when you need to use a quote in a string as the quote would need double quotes

String slicing
hw = "Hello! World"
print(hw[7:]) - Prints World
print(hw[-5:]) - Prints World
print(hw[:5]) - Prints Hello
print(hw[0:5]) - Prints Hello
print(len(hw)) - shows the length of the string

example_text = "here some text with lots of text"
print(example_text.count("e")) - return number of non overlapping occurrences
print(example_text.lower()) - returns string in lower case
print(example_text.upper()) - returns string in upper case
print(example_text.capitalize()) - capitalises first letter of string
print(example_text.replace("with ", ",")) - replaces with for a comma

Formatted string (f strings)
name = "Lassie"
years = 7
height_cm = 60.2
print(f"{name} is {years} years old and {height_cm}cm tall.")
This produces the outcome - Lassie is 7 years old and 60.2cm tall.

Formatted string with inputs
name = input("Please enter your name: ")
age = int(input("Please enter your age: "))
dob = input("Please enter your date of birth: ")
address = input("Please enter your address: ")
siblings = input("Please enter how many siblings you have: ")
print(f"Your name is {name}, your age is {age}, your date of birth is {dob}, you live at {address} and you have {siblings} siblings!")

Formatted string with different data types
name = "John"
age = 24
dob = "20 May 1998"
siblings = 6
print(f"your name is {name}, your age is {age}, your date of birth is {dob}, you have {siblings} siblings")

Booleans
Booleans are capitalised
a = True
b = False
print(a == b) # False
print(a != b) # True
print(a >= True) # True
print(b <= False) # True

print(True and False) # both conditions must be true otherwise its false
print(False and True) # both conditions must be true otherwise its false
 print(False or True) # if one of the conditions is true the statement will be true

End Task
name = input("Please enter your name: ")
height = int(input("Please enter your height in cm: "))
favourite_colour = input("Please enter your favourite colour: ")
secret_spirit_animal = input("Please enter your secret spirit animal: ")
print(f"Your name is {name}, your height is {height} cm and your favourite colour is {favourite_colour}.")
print(f"The first letter of your spirit animal is {secret_spirit_animal[0]}, the last letter of your spirit animal is {secret_spirit_animal[-1]}")
print(f"Your spirit animal is {str(len(secret_spirit_animal))} letters long")

guess_animal = input("What is your secret spirit animal?: ")
if guess_animal == secret_spirit_animal:
 print("OMG you got it correct!")
else:
 print("You got it wrong! Unlucky")
