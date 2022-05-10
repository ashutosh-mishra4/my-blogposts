## If/Else Elif and Lists in Python

## If/Else statement

If/Else in any programming language is used to make a decision depending upon a particular condition. Just like in real life we make decisions, we have to also make decisions in programming. Let's see this with an example:-

**Example 1:** *Write a program that accepts the user's age as input and determines whether the person is an adult or not.*

```
age = int(input('Enter your age: '))

if (age >= 18):
    print('You are an adult')
else:
    print('You are not an adult')
``` 
#### Explanation: 

- We first declare a variable called age with an **input** function to accept user input wrapped inside the **int** function. The *input* function is used to get input from the user and the *int* function is used to convert that value into a number.

- Then we wrote an *if* statement to check whether the user is 18 or above years of age. If yes, then "You are an adult" gets printed on the console. We have to specify a **:** (colon) after the if condition and give an indentation in the next line. Indentation is nothing but the extra white space which you see before the *print *statement in the above code.

- Finally, we have an *else* statement that will run in case *if* statement fails. In the above example, if the user turns out to be less than 18 years of age, "You are not an adult" will be printed on the console.

## Elif statement

**Elif** statement in python is the substitute for the **Else/If** statement which is used in other programming languages. It is used to decide on multiple conditions. Let's learn it better with an example-


**Example 2:** *Create a grading system that assigns various grades to the students depending upon the marks obtained*

```python
marks = int(input('Enter your marks: '))

if(marks >= 90):
  print('Grade A+')
elif(marks >= 80):
  print('Grade A')
elif(marks >= 70):
  print('Grade B')
elif(marks >= 60):
  print('Grade C')
elif(marks < 60):
  print('Grade D')
```
#### Explanation

- In the first line, we created an input function, wrapped it inside *int()* to convert the input marks into integers, and assigned them to the *marks* variable.
- Then there's an *If* statement to check whether the input marks are equal to or more than 90, if yes, **Grade A+** will be printed on the console.
- After that, there are 4 *Elif* statements. Each statement has its own **Grade**.
- If marks are **>=80**, **Grade A** will be printed, **Grade B** for *>=70*, **Grade C** *>= 60*, and **Grade D** for marks *<60*.

## Lists
List is a data structure in Python which allows you to store multiple items in one place.  You can think of *List* as an alternative to *Arrays* in Python. There are multiple real world use cases for Lists. Ex- Storing books and movie names in books and movie recommendation websites. 

```python
# Let's print the name of various social media platforms
socials = ["Twitter", "Facebook", "Instagram"]
print(socials) #Expected output - ['Twitter', 'Facebook', 'Instagram']
```

#### Explanation

- We created a list with various social media platform names, assigned it to variable socials, and used the *print()* function to print it on the console.
- You have to always wrap the content of the list inside **square brackets([ ])**
- Just like arrays, each item in the list has its index position which starts from 0. In the above example, *Twitter* has position 0, *Facebook* 1, and *Instagram* 2.

You can also print an item from the list using its index position. In the above code change  `print(socials)` to `print(socials[1])` and you'll get *Facebook* as the printed result.

## List Operations

### 1. Replacing an item

```python
# Let's create a numbered list in ascending order
numbers = [1,2,3,5,5,6,7,8]
print(numbers) # Expected output - [1,2,3,5,5,6,7,8]
# As you can see, we stored 5 twice, let's fix it
numbers[3] = 4  #This code will replace the value stored at index 3 with 4
print(numbers) # Expected output - [1,2,3,4,5,6,7,8]
# Yayyyyy, we successfully changed the value of 5 stored at index 3 with 4
```

#### Explanation

- At first, we created an ascending numbered list with *5* appearing twice in the list, at indexes 3 and 4.
- To fix this issue, we wrote another code `numbers[3] = 4`. This will replace the value stored at index position 3 with 4. If you want to change the value of any other position, you can change 3 in `numbers[3]` with a different index number, like `numbers[0]`, and `number[1]` and so on.


### 2. Concatenating multiple lists

In Python, it is possible to concatenate multiple lists with each other. Let's see this with an example-

```python
# Let's create 2 numbered lists - 1 to 5 and 6 to 10
numbers = [1,2,3,4,5]
newnumbers = [6,7,8,9,10]
print(numbers+newnumbers) # Expected output - [1,2,3,4,5,6,7,8,9, 10]
# This happened because we added the newnumbers list to numbers list and printed the result.
```

#### Explanation

- We created 2 numbered lists with numbers 1-5 and 6-10 respectively.
- After that, we printed the combined result of the addition of both lists and got our combined result.

### 3. Multiplication of Lists

In Python, you can also perform multiplication operations on *Lists*. You cannot multiply lists with each other but you can multiply them with an integer to repeat the value a certain number of times.

```python
# Let's create a numbered list with value 1 to 5
numbers = [1,2,3,4,5]
print(numbers*2) # Expected output - [1,2,3,4,5,1,2,3,4,5]
# We multiplied our list by 2 and got the same result values twice due to the multiplication.
```

#### Explanation

- We first created a *numbers* list with values of 1 to 5.
- After that, we printed the result of the *numbers* list multiplied by two and got the result **[1,2,3,4,5,1,2,3,4,5]** because of the multiplication.

### 4. Check the existence of an item

This is one of the most important operations of the list - *To check whether a particular item is present in the list or not.* Let's see this with an example-

```python
# Let' create a list with a few sample colors
colors = ["Red", "Blue", "Orange", "Pink"]
# Now let's check whether the color "Purple" exists in the list or not.
print("Purple" in colors) # Returns false because "Purple" is not in our list.
# Now let's check whether "Blue" is present in our list or not
print("Blue" in colors) # Returns true because "Blue" is present in our list.
```

#### Explanation

- We first created a list of colors with color *Red, Blue, Orange, and Pink*
- Next, we check whether **Purple** exists in our list or not with the following code - `print("Purple" in colors)`
- We got the result as *false* because there is no "Purple" in our list. Next, we did the same thing with "Blue".
- This time got the result *true* because "Blue" is present in our list.

### Conclusion

That's it for today's post and I will see you soon in another Python tutorial. This tutorial and all the future tutorials in this series are based on **[The Complete Python Masterclass](https://www.udemy.com/course/python-masterclass-course/)**. Check out this course if you want to learn Python in detail.

*Happy Coding!*