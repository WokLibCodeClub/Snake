Loop with range function
------------------------

In the last session we introduced the `range()` function and showed three ways to use it, with either one, two or three numbers inside the brackets. The `range()` function then automatically generates a list of numbers, according the the parameters in the brackets.

One of the most common ways to use the `range` function is in a `for` loop. So instead of writing
```
for n in [1,2,3,4,5]:
    print(n)
```

where each item in the list is typed out individually, we can now use a range function in place of the list and write:
```
for n in range(1,6):
    print(n)
```

Challenge
=========

Start a new Python file, with filetype .py, and write code to produce this output:

10  
9  
8  
7  
6  
5  
4  
3  
2  
1  
0  
Lift off!

One easy way to do this would be to type a list which had all these items in it, then use a `for` loop to print each item in the list. A smarter, more Python-y, way is to use the `range` function to generate the numbers and use this in the `for` loop. If you do it this way you will need to use `range` to produce a list where the numbers get smaller, not bigger. This sounds like `range()` with three numbers in the brackets... Can you figure it out?

Changing Lists
--------------

In the Snake project all the letters in the word 'Snake' follow the same path as the letter S. To make this happen we have to remember where the letter S has been, and we do this by keeping a *list* of all the previous positions. So we have to be able to **change** the list as the letter S moves about. This section is about different ways we can change a list we've already made.

### Adding an item to the end of a list

Here is the code from last week to make a list of text items and put the list in a variable called myfruitslist. The second line of code prints out the list so we can check the contents:
```
myfruitslist = ['apple', 'orange', 'pear', 'strawberry', 'banana']
print(myfruitslist)
```
Here is the code to add a new item onto the end of this list:
```
myfruitslist.append('grape')
print(myfruitslist)
```
Again, the second line just prints the list, so we can see if it has changed.


### Deleting an item from a list

Remember that the items in a list all have a number, but the numbering starts at 0, so in my list above the item `apple` would be `myfruitslist[0]` and `pear` would be `myfruitslist[2]` etc.

This code will delete the **fourth** item from the myfruitslist:
```
del myfruitslist[3]
print(myfruitslist)
```
(Change the number inside the square brackets to delete the item you want to delete.)

Counting the items in a lists
-----------------------------

If we've written code to add items into a list and delete some items from the list we sometimes need to check how many items there are in the list at the moment. This is called the *length* of the list, which is shortened in Python to *len*. We can do this with this code, which makes a numerical variable called `numitems` and sets it equal to the number of items in the list:
```
numitems = len(myfruitslist)
print(numitems)
```
(The second line of code prints the value of numitems so we can see how many items there are in the list.)

Asking the user to type some input
----------------------------------

Python has a simple way of asking the user of a programme for some input - the function is called `input`, which is not surprising. This code asks the user to type her or his name, and puts the name into a variable called `a`. The second line of code is a more complicated print function which prints out some text, followed by variable `a`.
```
a = input('Type name: ')
print('My name is ' + a)
```
In an `input` statement the part inside the brackets is called the *prompt*. This is the bit that Python types on the screen to ask the user for input. Notice there is a blank space as the last character of this prompt. This is not essential, but it means when the user types something it will be separated from the prompt text by a space, which looks a bit neater. In the `print` statement there is another space at the end of the `'My name is '` text. This is so that there will be a gap between this text and the value of variable `a`.

More about user input
---------------------

