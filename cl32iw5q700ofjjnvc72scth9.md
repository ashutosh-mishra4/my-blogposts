## List Functions in Python

*List is a data structure in Python which allows you to store multiple items in one place. You can think of List as an alternative to Arrays in Python. *

We already learned about lists and some common list operations in our last post, if you missed that, you can read it [here](https://fullstackstage.com/ifelse-elif-and-lists-in-python).

Now let's move ahead and take look at some of the common and useful **list functions** in Python-

## 1. Appending an item

In the previous post, we saw how to replace an item in a list. In this post, we will see how to append an item to the list.

### Syntax

```python
listname.append(item)
```
To append an item to a list, you have to use *.append()* after the name of the list and pass the item you want to insert as an argument. Let's understand this better with an example - 

```python
# Let's create a list with a few sample colors
colors = ["Red", "Blue", "Orange", "Pink"]
print(colors) # Expected output - ['Red', 'Blue', 'Orange', 'Pink']
# Now let's add "Purple" to our list
colors.append("Purple") 
print(colors)# Expected output - ['Red', 'Blue', 'Orange', 'Pink', 'Purple']
```

### Explanation

- In the above code, we first created a color list with a few color names and printed it on the console.
- Then, we used *append()* function to add color *Purple* to our list with the following code - `colors.append("Purple")`
- Finally, when we used the *print* statement this time, we got **Purple** along with other colors in the list.

## 2. Find the length of the List

Determining the length of a list is an effortless task in Python. You have to use the *len()* function.

### Syntax

```python
len(listname)
```
len() function is easy to use, you have to just call the *len()* and pass the list as an argument. Let's see an example-

```python
# Let's create a list with a few sample colors
colors = ["Red", "Blue", "Orange", "Pink"]
print(len(colors)) # Expected output - 4
```
### Explanation

- Just like the previous snippet, we first created a color list.
- After that, we printed the `len(colors)` function to know the length of the list. To determine the length of a list, you have to pass the *list* name inside the `len()` function.

## 3. Inserting an item in the list

We have already seen how to replace a particular item in the list. Now we will see, how to insert an item in a particular position. 

### Syntax

```python
listname.insert(index, item)
```

To insert an item at a particular position on the list, we have to add *.insert()* after the name of the list and pass 2 arguments to the function - the index position at which we want to insert our item and the item itself. See the below example  - 

```python
# Let's create a list with a few sample colors
colors = ["Red", "Blue", "Orange", "Pink"]
print(colors) # Expected output - ['Red', 'Blue', 'Orange', 'Pink']
# Now let's add color "Purple" on the index postion 2
colors.insert(2, "Purple")
print(colors) # Expected output - ['Red', 'Blue', 'Purple', 'Orange', 'Pink']
```

### Explanation

- After creating and printing the color list, we used the `insert()` function to add the color *Purple* on the index position 2 in our list.
- We used `colors.insert(2, "Purple")` which inserted the "Purple" on the 2nd index position. 

Inserting an item on a certain index position does not replace the previous item, it only shifts it and other subsequent items to their next positions.


## 4. Find the index value of an item

Every item in a list has an index position. When working on a complex project, you may need to determine the index position of a value. The *index()* function comes to help here. It helps you identify the index position of an item in the list.

### Syntax

```python
listname.index(item)
```

To identify the index position of an item, you have to add *.index* after the listname and pass the item as an argument. Let's understand this better with an example-

```python
# Let' create a list with a few sample colors
colors = ["Red", "Blue", "Orange", "Pink"]
# Now let's identify the position of the color "Blue"
print(colors.index("Blue")) # Expected output - 1
```

### Exaplanation

- In the above code, we created a color list and used the *index()* function on it and passed **"Blue"** as an argument.
- The code in return gave us the index position of the color "Blue", i.e., 1.

## Conclusion

That's it for today's post and I will see you soon in another Python tutorial. This tutorial and all the future tutorials in this series are based on **[The Complete Python Masterclass](https://www.udemy.com/course/python-masterclass-course/)**. Check out this course if you want to learn Python in detail.

*Happy Coding!*