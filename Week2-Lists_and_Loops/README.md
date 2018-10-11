To complete the Snake project we need to learn about lists.

Lists
-----

A List in Python is simply a collection of different items, they can be numbers, or bits of text, or other things. To make them into a list you simply put all the items inside square brackets, then put a comma in between each of the items. Here is an example of a Python list:
```
['apple', 'orange', 'pear', 'strawberry', 'banana']
```
This is a list of text items - you can tell they are text items because each of the items is contained in quotes. Here is a list containing numbers:
```
[1,2,3,4,5,6,7,8,9,10]
```
Python also has a special type of variable is called a *List* variable, which contains a list. To make a List variable you simply set the variable equal to a list. Here is the code to make a list variable called myfruitslist which contains a list of fruits:
```
myfruitslist = ['apple', 'orange', 'pear', 'strawberry', 'banana']
```
You can use the Python print function to see what the list variable contains:
```
myfruitslist = ['apple', 'orange', 'pear', 'strawberry', 'banana']
print(myfruitslist)
```
You can also look at individual items in the list by using the list variable name, followed by a number in square brackets.


Make list of fruits. This is a list of text items because of the quotes, which can be single or double

Print item from list - note numbering starts at 0

Using a loop with a list

A list of numbers

Combine text and numbers in an output print.

Challenge - write a programme to print out a 3 times table using for and a list.

It's easy to type a number list if you only want a few numbers in it, but if you wanted a number list which went from 0 up to 100 or more it would be very tedious to type out all the numbers by hand. Luckily Python has a command which will generate an automatic number list - it's called the range function. 

There are three ways you can use the range function - and the best way to find out about them is to try them out.

range function - first method:

numberlist = range(9)

Here range will generate an automatic number list, but to see what this list looks like we have to use print but with an extra command. If we type print(numberlist) Python will simply print range(9) which isn't very helpful. If we want to see the numbers which are in the automatically generated list we need to use

print(list(numberlist))

If you run the code it will show the numbers in the list. What do you notice about these numbers? How would you use range to produce a list which went from 0 to 17? Try it and see if it works!

range function - second method:

numberlist = range(2,11)

Here we have put two numbers in brackets after range, separated by a comma. Use the same print command to see which numbers go into the number list with this command. 
 
range function - third method:

numberlist = range(4,21,3)

Here we have put three numbers in brackets after range, separated by commas. Use the same print command to see which numbers go into the number list with this command. 
 