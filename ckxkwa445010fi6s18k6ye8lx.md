## Basic Python Concepts - Strings, Variables, User Input, and more

In this post, we are going to learn about some of the basic concepts of Python which more or less are also found in other programming languages. We'll start from the installation of Python and cover mathematical operations, strings, user input, string operations, variables, and In place operators.

If you don't know, this blog post and all other future posts in the Python series are part of  [this](https://www.udemy.com/course/python-masterclass-course/) Udemy course. Do check it out.

## Installation

Before starting if you don't have Python installed on your computer, install the latest version of [Python 3](https://www.python.org/downloads/) from their website and a corresponding IDE to code which we'll use for writing big programs, you can either go with [VS Code](https://code.visualstudio.com/download) or [Pycharm](https://www.jetbrains.com/pycharm/download/#section=windows).

## Our First Program

We'll start with the basic *Hello World* program. So open your Python console and follow the article - 

```
print('Hello World')
``` 
Type the above code in the console and hit enter. By now you would have seen the **Hello World** printed on your console. That's how easy it is to print something on the console in Python. But let's just move ahead because not everything is going to be that easy in the future.

## Maths Operations

Python console can also be directly used as a calculator and we can perform most of the common operations which we do on a calculator.

### Addition, Subtraction, Multiplication, and Division

```python
120 + 80 
```
Type the above code and hit enter and you will see the right answer 200. You can also perform subtraction, multiplication, and division in the console. Copy the code below in your console and see the results.
```
50 - 20

30 * 2

12 / 2
```
If you're focusing enough, you can see that when we divide certain numbers in Python, we get our result in decimal, just like we got 6.0 in the result of the above division. This is called a Float.

### Float

Decimal numbers are known as Float in programming. Float is a number that is not an integer. 
Using float with any mathematical expression will always result in float. When dividing 2 numbers, you can avoid getting float as a result by using *double slash(//)*.

```
12 // 2
```
The above code will give 6 as a result instead of 6.0, it happens because when we use a double slash in a division, Python gives us the quotient of the division.

### ZeroDivisionError

Dividing any number with zero in Python gives divide by zero error. So avoid dividing any number with zero or performing any other calculation which involves division by zero.

###  Exponent

Exponent is a number raised to the power of a certain number. In Python, you can do this by using **

```
3 ** 2
```
The above expression will raise 2 to the power of 3 and you'll get 9 as the result.

### Modulus

We already discussed how using double slash you can avoid getting float as a result of division. This happens because double slash gives the quotient of a division as a result.
For Ex: 10//3 = 3

But what if instead of getting quotient, you want the remainder of the division? We have something called **Modulus** for this case. The symbol of modulus is percent(%). Let's see it in action below - 

```
11 % 3
```
The above operation will result in 2 as the answer because that will be the actual result of the above division. This operation is incredibly useful when you want to know whether a certain number is odd or even. 

## String

Any text written in Python is a string or in other words, you can also say that anything written within quotes whether single('') or double("") is a string. If you type an integer within quotes, it will also be considered as a string, not an integer. 
For Ex: 5 is an integer, '5' is a string.

*NOTE: While writing a string if you want to put an apostrophe somewhere in between, use a backslash(\\)*

- Instead of writing, 'He's a good boy', write, `'He\'s a good boy'`.
- The latter version of the string will save you from error because you already have finished the string in the first 2 letters. According to Python, you started your string from **H** and finished it at **e** since you already have used 2 quotes up to that point.
- If you want your string to be printed on multiple lines instead of one, you can use `\n` at the point after which you want to start a new line. 

## Accepting input from the user

User inputs are very common when building large applications. Consider the example of a **Contacts** app where the user has to enter the phone number and name to save a contact or a **Chat** app where users can input words, numbers, emojis, and whatnot. 

In Python, we have a function called ***input()*** that allow users to input numbers, strings, etc in our program.

```
input('Please enter a value: ')
```
The string inside *input()* will be displayed to the user when asked for input. You can modify it according to your needs. Whatever value user inputs will be displayed to the console.

## String Operation

### Concatenation operation

Concatenation is the action of joining 2 or more strings together. Suppose there is a string called *'Hello'* and there is another string called *'World'*. When you concatenate these 2 strings, it becomes *'HelloWorld'*.

```
'Hello' + 'World'
```
The plus sign above is the concatenation operator which is used to concatenate strings. If you enter the code right and hit enter, you'll see `'HelloWorld'` printed on your console.

*Note:* 

- You cannot concatenate a string with a number. 
- However, you can multiple a string with a certain number to repeat its occurrence. For Ex - `'Hello'*3` will result in `'HelloHelloHello'`.
- Again you cannot multiple a string with a string, it will produce error.

## Variables

If you are familiar with Python or any other programming language, you might already know what a variable is. But in case you don't, you can think of it as a container to store data. Variables are common in every programming language and they let us store data types supported in that programming language. In Python, you can store all the supported data types in the variables. 

```
a = 100
```
In the above code, a is the variable that we've used to store the value of 100. The equal(=) sign is called an assignment operator whose job is to assign values. Type `print(a)` to print the value of variable **a** in the console.

## In place operators

Suppose you're recording your age in a variable and want to update it again this birthday.

```
age = 21
age = age + 1
```
In the above code, we first stored our age in a variable and then used a method to update the variable which is logical but isn't the best practice because writing the variable name twice in a line just to add a single value to it is not considered a great practice.

Instead, we have In place operators which help us change the value without repeating the variable name twice in the line. See the code below - 

```
age+=1
```

- `age+=1` has same effect as `age=age+1`. The `+=` removes the need to repeat the variable name twice in the line totally.

- We can also use the subtract and multiplication operator instead of the addition operator to update the subtracted or multiplied value of the variable like `age-=2` and `age*=4`. The former will reduce the value of the age variable by 2 and the latter will multiply it by 4.

## Parting Thoughts

In this article, we learned about maths operations, strings, variables, user input, In place operators, etc., and that marked the end of our **Basic Python Concepts**. 

There are thousands of things in a programming language and I don't mean that this article has covered every basic concept of Python but we've surely learned enough to move ahead and learn other topics and in the next article of the series we'll learn about **Control Structures in Python**.

Stay tuned.