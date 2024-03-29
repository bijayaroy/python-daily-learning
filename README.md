# PYTHON 
## Day 1: Introduction to Python

- History of Python:
  - Python was created by Guido van Rossum and first released in 1991.
  - Python's story begins in December 1989 when Guido van Rossum, a Dutch programmer, started working on a new programming language during his Christmas holidays. Van Rossum's goal was to create a language that would emphasize code readability and encourage developers to write clean and expressive code.
- One of the most important changes in Python's evolution has been the addition of new libraries and frameworks. These libraries provide pre-written code that can be used to perform common tasks, such as accessing databases, sending emails, and creating web applications. This has made Python even more powerful and versatile, and has helped it to become one of the most popular programming languages in the world.

- Basic Introduction:
  - Python is a high-level, interpreted programming language. This means that Python code is easy for humans to read and write, and it does not need to be compiled before it can be run. Python is also interpreted, which means that it is executed one line at a time, as it is read by the interpreter. Python is a general-purpose programming language, which means that it can be used for a wide variety of tasks, including web development, data science, machine learning, and more. Python is also a very popular language for beginners, as it is relatively easy to learn and use

## Day 2: Understanding Python Syntax
Indentation:
Python uses indentation to define blocks of code. This means that all lines of code that belong to the same block must be indented at the same level.


White space:
Python uses white space to separate different elements of a code statement. This includes spaces, tabs, and newlines.


Keywords:
Keywords are special words that have a specific meaning in Python. They cannot be used as variable names.


Identifiers:
Identifiers are used to name variables, functions, classes, and other objects in Python. They must start with a letter or an underscore (_) and can contain letters, numbers, and underscores.


Operators:
Operators are used to perform operations on data. They include arithmetic operators, comparison operators, logical operators, and assignment operators.


Comments:
Comments are important for code readability because they make it easier for other developers to understand your code. When you write comments, you are essentially explaining your code to yourself and others. This can be helpful when you are working on a project with other people, or when you come back to your code later and need to remember what it does.
There are three different types of comments in Python:
Single-line comments: These comments start with a hash (#) and continue to the end of the line.
Multi-line comments: These comments start with a triple quote (""") and end with a triple quote.

## Day 3: Variables and Data Types

### Variables:
  - Variables are used to store and manage data in a program.
```python
age = 25
name = "John"
```
Variable naming conventions and best practices:
use lowercase with underscores for readability.
Descriptive and meaningful names enhance code clarity.
```python
user_age = 25
user_name = "John"
```
### Data Types:
  - Fundamental data types: int, float, str, bool.
int: Represents integers.
float: Represents floating-point numbers.
str: Represents strings.
bool: Represents Boolean values (True or False).

```python
age = 25 # int
height = 5.9 # float
name = "John" # str
is_adult = True # bool
```
Exploring their characteristics and use cases.
```python
x = 5 + 2.0      # Results in a float
message = "Hello, " + "world!"  # String concatenation
```

## Day 4 : Conditional Statements (if, elif, else) and Numbers, Casting, and Operators:
### (if, elif, else):
Control the flow of a program based on conditions.
```python
x = 10

if x > 0:
 print("Positive")
elif x == 0:
 print("Zero")
else:
 print("Negative")
```
### Numbers, Casting, and Operators:

- Numbers:
  - Working with integers and floats.
```python
x = 5
y = 2.0
sum_result = x + y
```

- Casting and Type Conversion:
	Changing the data type of a variable.
```python
x = 5.7
int_x = int(x)  # Casting to int, result: 5
```

  - Method for converting between data types.
	Use functions like int(), float(), str(), etc.

- Operators:
  - Exploring arithmetic, comparison, logical, and assignment operators like +, -, *, /, ==, !=, and, or, +=, etc.
Example:
```python
result = (3 + 4) * 2 # Arithmetic
is_equal = (x == y) # Comparison
```

## Day 5 : Loops (for, while):
### For Loop:
```python
for i in range(5):
 print(i)
```
### While Loop:
```python
i = 0
while i < 5:
 print(i)
 i += 1
```
### Break and Continue Statements:
Break:
```python
for i in range(10):
 if i == 5:
 break
 print(i)
```
Continue:
```python
for i in range(10):
 if i == 5:
 continue
print(i)
```
## Day 6 : Functions
### Functions:
A function is a block of organized, reusable code that performs a specific task.
Functions help in modularizing code and promoting reusability.

Syntax:
```python
def function_name(parameters):
    # Function body
    # ...
    return result  # optional
```
Example:

```python
def greet(name):
    return f"Hello, {name}!"

result = greet("John")
print(result)
```


### Parameters and Arguments:

Parameters are variables in a function definition.
Arguments are values passed into a function.


### Return Statement:

A function can return a value using the return statement.
If no return statement is present, the function returns None by default.


### Scope:

Variables defined inside a function are local to that function.
Variables defined outside functions are global.

## Day 7: Modular Programming:
### Modular Programming:
Modular programming is a software design technique where a program is divided into independent, interchangeable modules.
Advantages:

Reusability: Modules can be reused in different parts of the program.
Maintainability: Changes in one module don't affect others if the interface remains the same.
Scalability: Easier to scale by adding or removing modules.
How to Create Modules:

Save a Python script (.py file) with functions and variables.
Import the module into another script using import module_name.
Example Module (math_operations.py):

```python
# math_operations.py
def add(x, y):
    return x + y

def subtract(x, y):
    return x - y
```
Using the Module in Another Script:

```python
# main_script.py
import math_operations

result_add = math_operations.add(5, 3)
result_subtract = math_operations.subtract(8, 4)

print(result_add, result_subtract)
```
### if name == "main":

Allows a script to be used both as an importable module and as a standalone script.
```python
# math_operations.py
def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

if __name__ == "__main__":
    # Code only executed when the script is run directly
    print(add(5, 3))
```
## Day 8: Arrays
In Python, arrays are often implemented using the built-in list type. The array can also be handled in Python by a module named array. They can be useful when we have to manipulate only specific data type values. A user can treat lists as arrays. However, the user cannot constrain the type of elements stored in a list. If you create arrays using the array module, all elements of the array must be of the same type.  While Python doesn't have a native array type like some other programming languages, its lists provide dynamic arrays with additional functionalities. (Source: GeeksForGeeks)

### Arrays (using Python Lists):
Creation:
```python
my_array = [1, 2, 3, 4, 5]
```
### Adding Elements:

You can use append() to add elements to the end of the array.
```python
my_array.append(6)
```
### Removing Elements:

Use .pop() or .remove() to remove and return an element by index.
```python
removed_element = my_array.pop(2)
```
### Indexing and Slicing:

Slice operation is performed on array with the use of colon(:). To print elements from beginning to a range use [:Index], to print elements from end use [:-Index], to print elements from specific Index till the end use [Index:], to print elements within a range, use [Start Index:End Index] and to print whole List with the use of slicing operation, use [:]. Further, to print whole array in reverse order, use [::-1].
```python
sublist = my_list[1:4]  # Elements from index 1 to 3
```
Common Operations:

Find the index of an element: my_array.index(element).
Count occurrences of an element: my_array.count(element).


NumPy Arrays:
If you need more advanced array manipulation and operations, you can use the NumPy library, which provides efficient and convenient array-like objects.

Installation:

`
pip install numpy
`


Creating NumPy Arrays:

```python
import numpy as np
numpy_array = np.array([1, 2, 3, 4, 5])
```
Operations:

NumPy allows element-wise operations and supports a variety of mathematical operations directly on arrays.
```python
result_array = numpy_array * 2
```
### Array Manipulation:

Reshaping: numpy_array.reshape(rows, columns).
Concatenation: np.concatenate((array1, array2)).
 
Similar to Python lists but extended for multi-dimensional arrays.
```python
squared_array = [x**2 for x in range(1, 6)]
```
Important Note:
- NumPy arrays are more efficient for numerical computations compared to Python lists, especially for large datasets.
- When dealing with mathematical and scientific computations involving arrays, NumPy is the preferred choice due to its optimized implementations.

## Day 9 : Programs related to Array:

### Printing an array:
```python
import array as arr

# create an array of integers
numbers = arr.array('i', [1, 2, 3, 4, 5])

# print the array
print(numbers)

# Output: array('i', [1, 2, 3, 4, 5])
```
### Finding the largest number in an array:
```python
import array as arr

# create an array of integers
numbers = arr.array('i', [10, 5, 15, 4, 6, 20, 9])

# find the largest number
largest = numbers[0]
for i in range(1, len(numbers)):
    if numbers[i] > largest:
        largest = numbers[i]

# print the largest number
print("Largest number:", largest)

# Output: Largest number: 20
```
### Sum of elements in an array:
```python
def sum(arr):
    result = 0
    for x in arr:
        result += x
    return result
```
### Storing all even numbers from an array in another array:
```python
import array as arr

# create an array of integers
numbers = arr.array('i', [10, 5, 15, 4, 6, 20, 9])

# create an empty array to store even numbers
even_numbers = arr.array('i', [])

# iterate over the original array and add even numbers to the new array
for number in numbers:
    if number % 2 == 0:
        even_numbers.append(number)

# print the new array
print(even_numbers)

# Output: array('i', [10, 4, 6, 20])
```
### Finding the average of all numbers in an array:
```python
import array as arr

# create an array of integers
numbers = arr.array('i', [1, 2, 3, 4, 5])

# calculate the sum of all numbers
sum = 0
for number in numbers:
    sum += number

# calculate the average
average = sum / len(numbers)

# print the average
print("Average:", average)

# Output: Average: 3.0
```
## Day 10: More Functions for Array
Some more useful functions provided in Python for arrays:

### Array Typecode Function
This function returns the data type by which the array is initialized. In this example, we are using arr.typecode to find out the data type of array initialization.

```python
# importing "array" for array operations
import array
    
# initializing array with array values
arr= array.array('i',[1, 2, 3, 1, 2, 5]) 
   
# using typecode to print datatype of array
print ("The datatype of array is : ")
print (arr.typecode)
#Output

#The datatype of array is : 
#i
```

### Array itemsize Function
This function returns the size in bytes of a single array element. In this example, we are using itemsize function to find out the size in byte of an array element.

```python
# importing "array" for array operations
import array
    
# initializing array with array values
arr= array.array('i',[1, 2, 3, 1, 2, 5]) 
   
# using itemsize to print itemsize of array
print ("The itemsize of array is : ")
print (arr.itemsize)
#Output
#The itemsize of array is : 
#4
```

### buffer_info() in Python
Returns a tuple representing the address in which array is stored and number of elements in it. In this example, we are using buffer_info() to do the same.

```python
# importing "array" for array operations
import array
    
# initializing array with array values
arr= array.array('i',[1, 2, 3, 1, 2, 5]) 
 
# using buffer_info() to print buffer info. of array
print ("The buffer info. of array is : ")
print (arr.buffer_info())
#Output
#The buffer info. of array is : 
#(140491260368688, 6)
```

### Array fromlist() Function
This function is used to append a list mentioned in its argument to end of array. In this example, we are using fromlist() to append a list to end of array.

```python
# importing "array" for array operations
import array
    
# initializing array with array values
arr = array.array('i',[1, 2, 3, 1, 2, 5]) 
li = [1, 2, 3]
   
# using fromlist() to append list at end of array
arr.fromlist(li)
   
# printing the modified array
print ("The modified array is : ",end="")
for i in range (0,9):
    print (arr[i],end=" ")
#Output
#The modified array is : 1 2 3 1 2 5 1 2 3 
```

### tolist() in Python
This function is used to transform an array into a list. In this example, we are using tolist() to convert an array to list.

```python
# importing "array" for array operations
import array
    
# initializing array with array values
arr = array.array('i',[1, 2, 3, 1, 2, 5]) 
   
# using tolist() to convert array into list
li2 = arr.tolist()
   
# printing the new list
print ("The new list created is : ",end="")
for i in range (0,len(li2)):
    print (li2[i],end=" ")
#Output
#The new list created is : 1 2 3 1 2 5 
```
## Day 11: Strings
In Python, a string is a sequence of characters enclosed within single quotes (' '), double quotes (" "), or triple quotes (''' ''' or """ """). 

Strings are immutable, meaning that once they are created, their values cannot be changed.
Like many other popular programming languages, strings in Python are arrays of bytes representing unicode characters.
However, Python does not have a character data type, a single character is simply a string with a length of 1.
Square brackets can be used to access elements of the string.
```python
a = "Hello, World!"
print(a[1])
```
Assigning a string to a variable is done with the variable name followed by an equal sign and the string:
```python
a = "Hello"
print(a)
```
Python provides a variety of built-in methods for manipulating strings. Some commonly used methods include:

- len(string): Returns the length of the string.
- string.lower(), string.upper(): Converts the string to lowercase or uppercase.
- string.startswith(prefix), string.endswith(suffix): Checks if the string starts or ends with a specified prefix or suffix.
- string.find(substring): Returns the index of the first occurrence of the substring, or -1 if not found.

# Day 12: Strings(contd.)
More functions related to it:
string.strip(), string.lstrip(), string.rstrip(): Removes any whitespaces before or at the end.
```python
sentence = "   This is a sample sentence.   "
print(sentence.strip())
# Output: "This is a sample sentence."
```
Check String: To check if a certain phrase or character is present in a string, we can use the keyword in.
```python
txt = "The best things in life are free!"
print("free" in txt)

text = "The best things in life are free!"
print("expensive" not in text)
```
Slicing: You can return a range of characters by using the slice syntax. Specify the start index and the end index, separated by a colon, to return a part of the string.
```python
b = "Hello, World!"
print(b[2:5])
```
Replace String: The replace() method replaces a string with another string:
```python
a = "Hello, World!"
print(a.replace("H", "J"))
```
Split String: The split() method returns a list where the text between the specified separator becomes the list items.
```python
a = "Hello, World!"
print(a.split(",")) # returns ['Hello', ' World!']
```
## Day 13 : Numpy array

NumPy arrays are a fundamental data structure in the NumPy library, which is a popular Python library used for numerical computing. NumPy arrays provide a way to store and manipulate large arrays of numerical data efficiently.

Here's a brief overview of NumPy arrays:

Homogeneous Data: NumPy arrays are homogeneous, meaning all elements in the array must have the same data type. This contrasts with Python lists, which can contain elements of different data types.

Multidimensional: NumPy arrays can have any number of dimensions. The most common are 1-dimensional arrays (vectors), 2-dimensional arrays (matrices), and higher-dimensional arrays.

Efficiency: NumPy arrays are implemented in C, which makes them much more efficient than Python lists, especially for large datasets.

Universal Functions (ufuncs): NumPy provides a large set of mathematical functions that operate element-wise on arrays, known as universal functions or ufuncs. These functions allow for fast computations on arrays without the need for explicit looping in Python.

Indexing and Slicing: NumPy arrays support advanced indexing and slicing operations, similar to Python lists, allowing you to access subsets of the array efficiently.

Broadcasting: NumPy arrays support broadcasting, which is a powerful mechanism that allows arithmetic operations to be performed between arrays of different shapes, often eliminating the need for explicit looping.

Integration with other Libraries: NumPy arrays are used as the standard data structure for exchanging data between different scientific computing libraries in Python, such as SciPy, Pandas, Matplotlib, and scikit-learn.

Here's a simple example of creating a NumPy array and performing some basic operations:

```python
import numpy as np

# Creating a 1-dimensional NumPy array
arr1d = np.array([1, 2, 3, 4, 5])

# Creating a 2-dimensional NumPy array
arr2d = np.array([[1, 2, 3], [4, 5, 6]])

# Accessing elements of an array
print(arr1d[0])  # Output: 1
print(arr2d[1, 2])  # Output: 6

# Slicing arrays
print(arr1d[:3])  # Output: [1 2 3]
print(arr2d[:, 1:])  # Output: [[2 3]
                      #          [5 6]]

# Performing arithmetic operations
result = arr1d * 2
print(result)  # Output: [ 2  4  6  8 10]

# Broadcasting
arr3 = np.array([[1], [2], [3]])
arr4 = np.array([1, 2, 3])
result = arr3 + arr4
print(result)  # Output: [[2 3 4]
               #          [3 4 5]
               #          [4 5 6]]
```
0-D Arrays
0-D arrays, or Scalars, are the elements in an array. Each value in an array is a 0-D array.

```python
import numpy as np

arr = np.array(42)

print(arr)
```
1-D Arrays
An array that has 0-D arrays as its elements is called uni-dimensional or 1-D array.

These are the most common and basic arrays.
```python
import numpy as np

arr = np.array([1, 2, 3, 4, 5])

print(arr)
```
2-D Arrays
An array that has 1-D arrays as its elements is called a 2-D array.

These are often used to represent matrix or 2nd order tensors.

NumPy has a whole sub module dedicated towards matrix operations called numpy.mat

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6]])

print(arr)
```
3-D arrays
An array that has 2-D arrays (matrices) as its elements is called 3-D array.

These are often used to represent a 3rd order tensor.

```python
import numpy as np

arr = np.array([[[1, 2, 3], [4, 5, 6]], [[1, 2, 3], [4, 5, 6]]])

print(arr)
```
NumPy Arrays provides the [ndim] attribute that returns an integer that tells us how many dimensions the array have.
Negative Indexing
Use negative indexing to access an array from the end.

```python
import numpy as np

arr = np.array([[1,2,3,4,5], [6,7,8,9,10]])

print('Last element from 2nd dim: ', arr[1, -1])
```
Data Types in NumPy
NumPy has some extra data types, and refer to data types with one character, like i for integers, u for unsigned integers etc.

Below is a list of all data types in NumPy and the characters used to represent them.

i - integer
b - boolean
u - unsigned integer
f - float
c - complex float
m - timedelta
M - datetime
O - object
S - string
U - unicode string
V - fixed chunk of memory for other type ( void )

Change data type from float to integer by using 'i' as parameter value:
```python
import numpy as np

arr = np.array([1.1, 2.1, 3.1])

newarr = arr.astype('i')

print(newarr)
print(newarr.dtype)
```

### Hackerrank Challenge: 
Q1.The provided code stub will read in a dictionary containing key/value pairs of name:[marks] for a list of students. Print the average of the marks array for the student name provided, showing 2 places after the decimal.

```python
if __name__ == '__main__':
    n = int(input())
    student_marks = {}
    for _ in range(n):
        name, *line = input().split()
        scores = list(map(float, line))
        student_marks[name] = scores
    query_name = input()
    
    if query_name in student_marks:
        marks = student_marks[query_name]
        average = sum(marks) / len(marks)
        print("{:.2f}".format(average))
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/53acd6a5-872a-4c89-9bb7-c16e1804b154)

Q2. You are given a two lists A and B. Your task is to compute their cartesian product X.

```python
# Take user input for the first list
list1 = input().split()

# Take user input for the second list
list2 = input().split()

# Convert elements to integers
list1 = [int(x) for x in list1]
list2 = [int(x) for x in list2]

# Using list comprehension to compute Cartesian product
cartesian_product = [(x, y) for x in list1 for y in list2]

# Printing each tuple separately
for pair in cartesian_product:
    print(pair, end=" ")
```
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/e699cf29-aeda-48f1-b792-24800596ed7d)

## Day 14: Tree
A tree represents hierarchical relationships between elements. It consists of nodes connected by edges. Each node contains a value (or data) and references to its child nodes. The topmost node in a tree is called the root node, and nodes with no children are called leaf nodes.

The Tree data structure can be useful in many cases:

Hierarchical Data: File systems, organizational models, etc.
Databases: Used for quick data retrieval.
Routing Tables: Used for routing data in network algorithms.
Sorting/Searching: Used for sorting data and searching for data.

Tree Terminology and Rules:

- The first node in a tree is called the root node.
- A link connecting one node to another is called an edge.
- A parent node has links to its child nodes. Another word for a parent node is internal node.
- A node can have zero, one, or many child nodes.
- A node can only have one parent node.
- Nodes without links to other child nodes are called leaves, or leaf nodes.
- The tree height is the maximum number of edges from the root node to a leaf node. The height of the tree above is 2.
- The height of a node is the maximum number of edges between the node and a leaf node.
- The tree size is the number of nodes in the tree.

Types of Trees
- Binary Trees: Each node has up to two children, the left child node and the right child node. This structure is the foundation for more complex tree types like Binary Search Trees and AVL Trees.
- Binary Search Trees (BSTs): A type of Binary Tree where for each node, the left child node has a lower value, and the right child node has a higher value.
- AVL Trees: A type of Binary Search Tree that self-balances so that for every node, the difference in height between the left and right subtrees is at most one. This balance is maintained through rotations when nodes are inserted or deleted.

A binary tree is a hierarchical data structure composed of nodes, where each node has at most two children, referred to as the left child and the right child. The topmost node of the tree is called the root node. In a binary tree, each child node can have a reference to its parent node.

Benefits of Binary Trees over Arrays and Linked Lists:

Arrays are fast when you want to access an element directly, like element number 700 in an array of 1000 elements for example. But inserting and deleting elements require other elements to shift in memory to make place for the new element, or to take the deleted elements place, and that is time consuming.
Linked Lists are fast when inserting or deleting nodes, no memory shifting needed, but to access an element inside the list, the list must be traversed, and that takes time.
Binary Trees, such as Binary Search Trees and AVL Trees, are great compared to Arrays and Linked Lists because they are BOTH fast at accessing a node, AND fast when it comes to deleting or inserting a node, with no shifts in memory needed.

Properties of Binary Trees:
Root Node: The topmost node in a binary tree.
Parent Node: A node that has child nodes.
Child Node: A node that is connected to a parent node.
Leaf Node: A node that does not have any children.
Internal Node: A node that has at least one child.
Height: The height of a binary tree is the maximum distance from the root node to a leaf node. The height of an empty tree is considered to be -1.
Depth (or Level): The depth of a node is the number of edges from the root node to that node.
Balanced Binary Tree: A binary tree in which the heights of the left and right subtrees of any node differ by at most one.
Complete Binary Tree: A binary tree in which every level, except possibly the last, is completely filled, and all nodes are as far left as possible.
Full Binary Tree: A binary tree in which every node has either zero or two children.
Perfect Binary Tree: A binary tree in which all internal nodes have exactly two children, and all leaf nodes are at the same level.
Binary Search Tree (BST): A binary tree in which the value of each node in the left subtree is less than the value of the node itself, and the value of each node in the right subtree is greater than the value of the node itself.

```python
class TreeNode:
    def __init__(self, data):
        self.data = data
        self.children = []

    def add_child(self, child_node):
        self.children.append(child_node)

# Example usage:
if __name__ == "__main__":
    # Create nodes
    root = TreeNode("A")
    node_b = TreeNode("B")
    node_c = TreeNode("C")
    node_d = TreeNode("D")
    node_e = TreeNode("E")
    node_f = TreeNode("F")

    # Connect nodes
    root.add_child(node_b)
    root.add_child(node_c)
    node_b.add_child(node_d)
    node_b.add_child(node_e)
    node_c.add_child(node_f)

    # Print the tree structure
    def print_tree(node, level=0):
        print("  " * level + str(node.data))
        if node.children:
            for child in node.children:
                print_tree(child, level + 1)

    print_tree(root)
#Output
#A
#  B
#    D
#    E
#  C
#    F
```
Binary Tree Traversal
Going through a Tree by visiting every node, one node at a time, is called traversal.

Since Arrays and Linked Lists are linear data structures, there is only one obvious way to traverse these: start at the first element, or node, and continue to visit the next until you have visited them all.

But since a Tree can branch out in different directions (non-linear), there are different ways of traversing Trees.

There are two main categories of Tree traversal methods:

Breadth First Search (BFS) is when the nodes on the same level are visited before going to the next level in the tree. This means that the tree is explored in a more sideways direction.

Depth First Search (DFS) is when the traversal moves down the tree all the way to the leaf nodes, exploring the tree branch by branch in a downwards direction.

There are three different types of DFS traversals:

pre-order
```python
def preOrderTraversal(node):
    if node is None:
        return
    print(node.data, end=", ")
    preOrderTraversal(node.left)
    preOrderTraversal(node.right)
```
in-order
```python
def inOrderTraversal(node):
    if node is None:
        return
    inOrderTraversal(node.left)
    print(node.data, end=", ")
    inOrderTraversal(node.right)
```
post-order
```python
def postOrderTraversal(node):
    if node is None:
        return
    postOrderTraversal(node.left)
    postOrderTraversal(node.right)
    print(node.data, end=", ")
```
Binary Search tree:
A Binary Search Tree (BST) is a type of Binary Tree data structure, where the following properties must be true for any node "X" in the tree:

The X node's left child and all of its descendants (children, children's children, and so on) have lower values than X's value.
The right child, and all its descendants have higher values than X's value.
Left and right subtrees must also be Binary Search Trees.

Operations on Binary Search Trees:
Insertion: To insert a new node into a BST, you compare the value of the new node with the value of the current node. If it's less, you move to the left subtree; if it's greater, you move to the right subtree. This process continues until you find an appropriate empty spot to insert the new node.
Deletion: Deleting a node from a BST can be a bit more complex. There are several cases to consider:
If the node to be deleted has no children, you can simply remove it from the tree.
If the node has one child, you can replace the node with its child.
If the node has two children, you can either replace it with the minimum value node from its right subtree (or the maximum value node from its left subtree), or you can swap it with its successor (or predecessor) in the tree and then delete that successor node.
Search: To search for a value in a BST, you start at the root node and compare the target value with the current node's value. If they match, you've found the node. If the target value is less than the current node's value, you move to the left subtree; if it's greater, you move to the right subtree. This process continues recursively until you find the node with the target value or reach a leaf node.
Traversal: There are three primary ways to traverse a BST:
Inorder Traversal: Traverse the left subtree, visit the node, then traverse the right subtree. This results in a sorted list if the BST is balanced.
Preorder Traversal: Visit the node, then traverse the left and right subtrees.
Postorder Traversal: Traverse the left and right subtrees, then visit the node.
Complexity of Operations:
Search: The time complexity of searching in a BST is O(h), where h is the height of the tree. In a balanced BST, the height is logarithmic (O(log n)), where n is the number of nodes. However, in the worst-case scenario (when the tree is highly unbalanced), the height can be linear (O(n)), resulting in degraded performance.
Insertion and Deletion: Both operations require a search first, so their time complexity is also O(h). However, if rebalancing is necessary to maintain the BST property, additional operations may be required, resulting in a time complexity of O(log n) in balanced trees.


Benefits of Binary Search Trees:


Efficient Search: BSTs provide efficient searching due to their ordered structure, especially when the tree is balanced.
Dynamic Operations: BSTs allow dynamic insertion and deletion of nodes, making them suitable for applications with frequently changing data.
Simple Structure: BSTs have a simple and intuitive structure, making them easy to implement and understand.


Limitations of Binary Search Trees:


Degraded Performance: Unbalanced BSTs can lead to degraded performance, with search, insertion, and deletion operations taking linear time in the worst-case scenario.
Memory Consumption: The memory usage of a BST can grow significantly if the tree becomes unbalanced, potentially leading to inefficient use of memory resources.

AVL Tree:

An AVL tree is a self-balancing binary search tree named after its inventors, Adelson-Velsky and Landis. It maintains a strict balance criterion to ensure efficient insertion, deletion, and search operations with a guaranteed worst-case time complexity of O(log n), where n is the number of nodes in the tree. The balance criterion is based on the height difference (also known as the balance factor) between the left and right subtrees of any node.


Properties of AVL Trees:
Balance Factor: For any node in an AVL tree, the height of its left subtree and the height of its right subtree differ by at most 1.
Height: The height of an AVL tree is the maximum depth of any node in the tree. The height of an empty tree is considered -1.
Balanced Subtrees: In an AVL tree, all subtrees rooted at any node also satisfy the balance factor property.
Self-Balancing: After insertion or deletion of a node, AVL trees automatically perform rotations to maintain balance if necessary.


AVL Tree Rotations:
AVL trees use rotations to restore balance when it is violated due to insertion or deletion operations. There are four possible rotations:
Left Rotation: A rotation performed to restore balance when the right subtree is taller than the left subtree by more than one level.
Right Rotation: A rotation performed to restore balance when the left subtree is taller than the right subtree by more than one level.
Left-Right Rotation (LR Rotation): A combination of left rotation followed by right rotation used to balance the tree.
Right-Left Rotation (RL Rotation): A combination of right rotation followed by left rotation used to balance the tree.
Operations on AVL Trees:
Insertion: After inserting a new node, AVL trees check the balance factor of each node and perform rotations if necessary to restore balance.
Deletion: After deleting a node, AVL trees check the balance factor of each node and perform rotations if necessary to restore balance.
Search: Searching for a node with a given key in the AVL tree follows the same logic as in binary search trees with O(log n) time complexity.
Traversal: Inorder, preorder, and postorder traversal methods are applicable to AVL trees, providing access to all nodes in sorted order.
Height Calculation: AVL trees provide a height-balanced structure, ensuring that the height of the tree remains logarithmic.


Benefits of AVL Trees:
Efficiency: AVL trees offer efficient operations, ensuring O(log n) time complexity for insertion, deletion, and search operations.
Self-Balancing: AVL trees automatically adjust their structure to maintain balance, reducing the risk of performance degradation.
Predictability: The balance criterion of AVL trees ensures predictable performance characteristics, making them suitable for applications with strict performance requirements.


Limitations of AVL Trees:
Overhead: Maintaining balance in AVL trees requires additional overhead in terms of extra bookkeeping and rotations, impacting memory usage and performance.
Complexity: The implementation of AVL trees, especially rotation algorithms, can be more complex compared to simpler data structures like binary search trees.


### Hackerrank Challenge:
Q1. Consider a list (list = []). You can perform the following commands:

insert i e: Insert integer  at position .
print: Print the list.
remove e: Delete the first occurrence of integer .
append e: Insert integer  at the end of the list.
sort: Sort the list.
pop: Pop the last element from the list.
reverse: Reverse the list.
Initialize your list and read in the value of  followed by  lines of commands where each command will be of the  types listed above. Iterate through each command in order and perform the corresponding operation on your list.

```python
if __name__ == '__main__':
    N = int(input())
    lst = []

    for _ in range(N):
        command = input().split()

        if command[0] == 'insert':
            lst.insert(int(command[1]), int(command[2]))
        elif command[0] == 'print':
            print(lst)
        elif command[0] == 'remove':
            lst.remove(int(command[1]))
        elif command[0] == 'append':
            lst.append(int(command[1]))
        elif command[0] == 'sort':
            lst.sort()
        elif command[0] == 'pop':
            lst.pop()
        elif command[0] == 'reverse':
            lst.reverse()
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/47cf4689-f1e3-4ab6-9413-bb1a42b8ac53)

Q2. Given an integer, n, and  n space-separated integers as input, create a tuple,t , of those n integers. Then compute and print the result of hash(t).
```python
n = int(input())
integer_list = map(int, input().split())

t = tuple(integer_list)
result = hash(t)

print(result)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/cffab12e-ef0b-4928-a19a-fc6eeee8b7a5)

## Day 15 : Trees (contd.)

#### B-Tree:
Definition:

A B-tree is a self-balancing tree data structure designed to store and manage large amounts of data efficiently in secondary storage such as disks.
It was invented by Rudolf Bayer and Edward McCreight in 1972 as a generalization of binary search trees.
Properties:

In a B-tree, each node can contain a variable number of keys and pointers to child nodes.
The keys within a node are stored in sorted order, facilitating efficient search operations.
All leaf nodes are at the same level, which ensures balanced access to data across the entire tree.
B-trees are characterized by a parameter B, known as the "order" of the tree, which determines the maximum number of children a node can have.
A B-tree must satisfy certain properties, including the minimum degree requirement, which ensures that nodes have a minimum number of keys.
Operations:

Search: Similar to binary search trees, searching in a B-tree follows a recursive process, navigating through the tree based on the comparison of keys.
Insertion: Inserting a new key into a B-tree involves finding the appropriate position for the key and inserting it while maintaining the sorted order of keys within nodes.
Deletion: Deleting a key from a B-tree requires locating the key, removing it from the node, and potentially rebalancing the tree to maintain its properties.
Applications:

B-trees are widely used in databases and file systems for indexing and managing large datasets efficiently.
They are suitable for scenarios where data is stored on disk and must be accessed in blocks or pages.
#### B+ Tree:
Definition:

A B+ tree is a variation of the B-tree that enhances its structure for efficient range queries and sequential access.
It was introduced by Rudolf Bayer and Edward McCreight in 1972 and later popularized by Douglas Comer.
Properties:

Like a B-tree, a B+ tree consists of internal nodes and leaf nodes, with keys stored only in the leaf nodes.
All leaf nodes are linked together in a linked list, enabling efficient range queries and sequential access.
Internal nodes in a B+ tree act as index nodes, containing pointers to child nodes and dividing keys to guide searches.
Advantages:

B+ trees offer improved performance for range queries and sequential access due to the linked list structure of leaf nodes.
They are well-suited for database systems where range queries are common, such as retrieving all records within a specified range or performing range-based joins.
Operations:

The basic operations of insertion, deletion, and search in a B+ tree are similar to those in a B-tree.
Insertion and deletion may require additional operations to maintain the linked list structure of leaf nodes.
Applications:

B+ trees are widely used in database systems as indexing structures for efficient retrieval of data within a range.
They are also employed in file systems and operating systems for managing large files and directories efficiently.


General Tree (Inserting,Deleting,BFS and DFS):

```python
class TreeNode:
    def __init__(self, value):
        self.value = value
        self.children = []

def insert_node(root, value):
    new_node = TreeNode(value)
    root.children.append(new_node)

def delete_node(root, value):
    for child in root.children:
        if child.value == value:
            root.children.remove(child)
            return
        delete_node(child, value)

def bfs(root):
    queue = [root]
    traversal = []
    while queue:
        node = queue.pop(0)
        traversal.append(node.value)
        for child in node.children:
            queue.append(child)
    return traversal

def dfs(root):
    traversal = []
    traversal.append(root.value)
    for child in root.children:
        traversal.extend(dfs(child))
    return traversal

# Example Usage
root = TreeNode(1)
insert_node(root, 2)
insert_node(root, 3)
insert_node(root.children[0], 4)
insert_node(root.children[0], 5)

print("BFS Traversal:", bfs(root))
print("DFS Traversal:", dfs(root))
```
Binary Tree :
```python
class TreeNode:
    def __init__(self, value):
        self.value = value
        self.left = None
        self.right = None

def insert_node(root, value):
    if root is None:
        return TreeNode(value)
    else:
        if value <= root.value:
            root.left = insert_node(root.left, value)
        else:
            root.right = insert_node(root.right, value)
    return root

def delete_node(root, value):
    if root is None:
        return root
    if value < root.value:
        root.left = delete_node(root.left, value)
    elif value > root.value:
        root.right = delete_node(root.right, value)
    else:
        if root.left is None:
            return root.right
        elif root.right is None:
            return root.left
        root.value = find_min_value(root.right)
        root.right = delete_node(root.right, root.value)
    return root

def find_min_value(root):
    min_value = root.value
    while root.left is not None:
        min_value = root.left.value
        root = root.left
    return min_value

def bfs(root):
    queue = [root]
    traversal = []
    while queue:
        node = queue.pop(0)
        traversal.append(node.value)
        if node.left:
            queue.append(node.left)
        if node.right:
            queue.append(node.right)
    return traversal

def dfs_inorder(root):
    if root is None:
        return []
    return dfs_inorder(root.left) + [root.value] + dfs_inorder(root.right)

# Example Usage
root = None
root = insert_node(root, 10)
root = insert_node(root, 5)
root = insert_node(root, 15)
root = insert_node(root, 3)
root = insert_node(root, 7)
root = insert_node(root, 12)
root = insert_node(root, 18)

print("BFS Traversal:", bfs(root))
print("DFS Inorder Traversal:", dfs_inorder(root))
```

Binary Search Tree:
```python
class TreeNode:
    def __init__(self, value):
        self.value = value
        self.left = None
        self.right = None

def insert_node(root, value):
    if root is None:
        return TreeNode(value)
    else:
        if value <= root.value:
            root.left = insert_node(root.left, value)
        else:
            root.right = insert_node(root.right, value)
    return root

def delete_node(root, value):
    if root is None:
        return root
    if value < root.value:
        root.left = delete_node(root.left, value)
    elif value > root.value:
        root.right = delete_node(root.right, value)
    else:
        if root.left is None:
            return root.right
        elif root.right is None:
            return root.left
        root.value = find_min_value(root.right)
        root.right = delete_node(root.right, root.value)
    return root

def find_min_value(root):
    min_value = root.value
    while root.left is not None:
        min_value = root.left.value
        root = root.left
    return min_value

def bfs(root):
    queue = [root]
    traversal = []
    while queue:
        node = queue.pop(0)
        traversal.append(node.value)
        if node.left:
            queue.append(node.left)
        if node.right:
            queue.append(node.right)
    return traversal

def dfs_inorder(root):
    if root is None:
        return []
    return dfs_inorder(root.left) + [root.value] + dfs_inorder(root.right)

# Example Usage
root = None
root = insert_node(root, 10)
root = insert_node(root, 5)
root = insert_node(root, 15)
root = insert_node(root, 3)
root = insert_node(root, 7)
root = insert_node(root, 12)
root = insert_node(root, 18)

print("BFS Traversal:", bfs(root))
print("DFS Inorder Traversal:", dfs_inorder(root))
```

### Top Questions related to Trees:
- Maximum Depth of Binary Tree
- Check if two trees have same structure
- Invert/Flip Binary Tree
- Binary Tree Maximum Path Sum
- Binary Tree Level Order Traversal
- Serialize and Deserialize Binary Tree
- Subtree of Another Tree
- Construct Binary Tree from Preorder and Inorder Traversal
- Validate Binary Search Tree
- Kth Smallest Element in a BST
- Lowest Common Ancestor of BST
- Implement Trie (Prefix Tree)
- Add and Search Word

### Hackerrank Challenge:
Q1. You are given a string and your task is to swap cases. In other words, convert all lowercase letters to uppercase letters and vice versa.
```python
def swap_case(s):
    swapped_string = ""
    for char in s:
        if char.isupper():
            swapped_string += char.lower()
        else:
            swapped_string += char.upper()
    return swapped_string

if __name__ == '__main__':
    s = input()
    result = swap_case(s)
    print(result)
```
Output:

![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/1898685d-abaa-4a2a-83f5-0086b1de668e)

Q2. You are given a string. Split the string on a " " (space) delimiter and join using a - hyphen.

```python
def split_and_join(line):
    # Split the input string based on whitespace
    split_line = line.split()
    # Join the split parts using a hyphen as the delimiter
    joined_line = "-".join(split_line)
    return joined_line

if __name__ == '__main__':
    line = input()
    result = split_and_join(line)
    print(result)
```
Output:


![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/84d246e6-3950-4fb0-848d-47a01e839648)

## Day 16 : Array (Revision): 
TOP QUESTIONS IN ARRAY:
Q1. Find a peak element which is not smaller than its neighbours. Given an array arr of n elements that is first strictly increasing and then maybe strictly decreasing, find the maximum element in the array.

Note: If the array is increasing then just print the last element will be the maximum value.
```python
def findPeak(arr,n):
    #If an array has just one element
    if(n==1):
        return 0
    #If the array is in increasing order, just check the first element is greater or not
    if(arr[0]>=arr[1]):
        return 0
    #If the array is in decreasing order, just check the last element is greater or not
    if(arr[n-1]>=arr[n-2]):
        return n-1
    #for the rest of the elemnts if there is an increasing and decreasing combination in the array
    for i in range(1, n-1):
        if(arr[i]>=arr[i-1] and arr[i]>=arr[i+1]):
            return i
        
arr=[]
n=int(input("Enter the number of elements in the array: "))
for i in range(0, n):
    e=int(input("Enter element {}:".format(i+1)))
    arr.append(e)
print("Index of peak-point is: ",findPeak(arr,n)+1)
```
Output:
```
Enter the number of elements in the array: 6
Enter element 1:1
Enter element 2:3
Enter element 3:20
Enter element 4:4
Enter element 5:1
Enter element 6:0
Index of peak-point is:  3
```
Q2. Program to find the minimum (or maximum) element of an array Given an array, write functions to find the minimum and maximum elements in it.

```python
def minimum(arr,n):
    min_value = arr[0]
    for i in range (1, n):
        if(min_value>=arr[i]):
            min_value=arr[i]
    return min_value

def maximum(arr,n):
    max_value = arr[0]
    for i in range (1, n):
        if(max_value<=arr[i]):
            max_value=arr[i]
    return max_value

arr=[]
n=int(input("Enter the number of elements in the array: "))
for i in range(0, n):
    e=int(input("Enter element {}:".format(i+1)))
    arr.append(e)
print("Maximum Value:",maximum(arr,n))
print("Minimum Value:",minimum(arr,n))
```
Output:
```
Enter the number of elements in the array: 6
Enter element 1:5
Enter element 2:3
Enter element 3:7
Enter element 4:2
Enter element 5:6
Enter element 6:8
Maximum Value: 8
Minimum Value: 2
```
Q3. Given an array (or string), the task is to reverse the array/string.
```python
def reverse(arr, start, end):
    while(start<=end):
        arr[start], arr[end]= arr[end], arr[start]
        start+=1
        end-=1
    return arr

n=int(input("Enter the number of elements in an array : "))
arr=[]
for i in range(0,n):
    e=int(input("Enter element {}: ".format(i+1)))
    arr.append(e)
print("The reversed array : ",reverse(arr,0,n-1)) 
```
Output:
```
Enter the number of elements in an array : 6
Enter element 1: 5
Enter element 2: 3
Enter element 3: 4
Enter element 4: 8
Enter element 5: 2
Enter element 6: 44
The reversed array :  [44, 2, 8, 4, 3, 5]
```
Q4. Write a program to sort a given array(in ascending order)
```python
def sort(arr,n):
    for i in range(0,n):
        min_e=i
        for j in range(i+1,n):
            if(arr[min_e]>arr[j]):
                min_e=j
        arr[min_e],arr[i]=arr[i],arr[min_e]
    return arr

n=int(input("Enter the number of elements in an array : "))
arr=[]
for i in range(0,n):
    e=int(input("Enter element {}: ".format(i+1)))
    arr.append(e)
print("The sorted array : ",sort(arr,n)) 
```
Output:
```
Enter the number of elements in an array : 6
Enter element 1: 4
Enter element 2: 7
Enter element 3: 3
Enter element 4: 5
Enter element 5: 8
Enter element 6: 2
The sorted array :  [2, 3, 4, 5, 7, 8]
```
Q5. Find K-th smallest/largest element in the array
```python
def ksmall(arr,n):
    for i in range(0,n):
        min_e=i
        for j in range(i+1,n):
            if(arr[min_e]>arr[j]):
                min_e=j
        arr[min_e],arr[i]=arr[i],arr[min_e]
    return arr[k-1]

def klarge(arr,n):
    for i in range(0,n):
        min_e=i
        for j in range(i+1,n):
            if(arr[min_e]>arr[j]):
                min_e=j
        arr[min_e],arr[i]=arr[i],arr[min_e]
    return arr[n-k]

n=int(input("Enter the number of elements in an array : "))
arr=[]
for i in range(0,n):
    e=int(input("Enter element {}: ".format(i+1)))
    arr.append(e)
k=int(input("Enter the value of k: "))
print("The {}th smallest element :".format(k))
print(ksmall(arr,n))
print("The {}th largest element :".format(k))
print(klarge(arr,n))
Enter the number of elements in an array : 6
```
Output:
```
Enter element 1: 2
Enter element 2: 3
Enter element 3: 5
Enter element 4: 4
Enter element 5: 7
Enter element 6: 8
Enter the value of k: 2
The 2th smallest element :
3
The 2th largest element :
7
```
Q6. Count number of occurrences (or frequency) in a sorted array

Examples: Input: arr[] = {1, 1, 2, 2, 2, 2, 3,}, x = 2 Output: 4 // x (or 2) occurs 4 times in arr[] Input: arr[] = {1, 1, 2, 2, 2, 2, 3,}, x = 3 Output: 1 Input: arr[] = {1, 1, 2, 2, 2, 2, 3,}, x = 1 Output: 2 Input: arr[] = {1, 1, 2, 2, 2, 2, 3,}, x = 4 Output: -1 // 4 doesn't occur in arr[]
```python
def occurence(arr,n,x):
    oc=0
    for i in range (0,n):
        if(arr[i]==x):
            oc+=1
    return oc

n=int(input("Enter the number of elements in an array : "))
arr=[]
for i in range(0,n):
    e=int(input("Enter element {}: ".format(i+1)))
    arr.append(e)
x=int(input("Enter the value of x for which the occurence is to be calculated: "))
print("Number of occurences : ",occurence(arr,n,x))
```
Output:
```
Enter the number of elements in an array : 6
Enter element 1: 1
Enter element 2: 3
Enter element 3: 3
Enter element 4: 4
Enter element 5: 4
Enter element 6: 4
Enter the value of x for which the occurence is to be calculated: 4
Number of occurences : 3
```
Q7. Given an array A[] consisting of only 0s, 1s, and 2s. The task is to write a function that sorts the given array. The functions should put all 0s first, then all 1s and all 2s in last.

This problem is also the same as the famous “Dutch National Flag problem”. The problem was proposed by Edsger Dijkstra. The problem is as follows:

Given N balls of colour red, white or blue arranged in a line in random order. You have to arrange all the balls such that the balls with the same colours are adjacent with the order of the balls, with the order of the colours being red, white and blue (i.e., all red coloured balls come first then the white coloured balls and then the blue coloured balls).
```python
def sort012(arr):
    l=0
    m=0
    h=n-1
    while(m<=h):
        #if arr[m] is equal to 0
        if(arr[m]==0):
            arr[l],arr[m]=arr[m],arr[l]
            l+=1
            m+=1
        #if arr[m] is equal to 1
        elif(arr[m]==1):
            m+=1
        #if arr[m] is equal to 2
        else:
            arr[m],arr[h]=arr[h],arr[m]
            h-=1
    return arr

n=int(input("Enter the number of elements in an array : "))
arr=[]
for i in range(0,n):
    e=int(input("Enter element {}: ".format(i+1)))
    arr.append(e)
print("Sorted array : ",sort012(arr))
```
Output:
```
Enter the number of elements in an array : 6
Enter element 1: 0
Enter element 2: 1
Enter element 3: 2
Enter element 4: 0
Enter element 5: 1
Enter element 6: 2
Sorted array :  [0, 0, 1, 1, 2, 2]
```
### Hackerrank Challenge:
Q1. You are given the firstname and lastname of a person on two different lines. Your task is to read them and print the following:

Hello firstname lastname! You just delved into python.

```python
def print_full_name(first, last):
    # Print the message
    print("Hello", first, last + "!", "You just delved into python.")


if __name__ == '__main__':
    first_name = input()
    last_name = input()
    print_full_name(first_name, last_name)
```

Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/239ac5dc-b51c-4580-89ca-795c7bd54241)

Q2. We have seen that lists are mutable (they can be changed), and tuples are immutable (they cannot be changed).

Let's try to understand this with an example.

You are given an immutable string, and you want to make changes to it.

```python
def mutate_string(string, position, character):
    # Convert the string to a list to allow modifications
    string_list = list(string)
    
    # Replace the character at the specified position
    string_list[position] = character
    
    # Convert the list back to a string and return it
    return ''.join(string_list)

if __name__ == '__main__':
    s = input()
    i, c = input().split()
    s_new = mutate_string(s, int(i), c)
    print(s_new)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/e17d3fdf-b75b-4d1f-acac-5838a04276d2)

## Day 17: Array Revision(contd.)
Q8. Given an array arr[] of non-negative integers and an integer sum, find a subarray that adds to a given sum. Note: There may be more than one subarray with sum as the given sum, print first such subarray.

Examples: Input: arr[] = {1, 4, 20, 3, 10, 5}, sum = 33 Output: Sum found between indexes 2 and 4 Explanation: Sum of elements between indices 2 and 4 is 20 + 3 + 10 = 33
```python
def subarray(arr,n,s):
    currentsum=arr[0]
    start=0
    i=1
    while(i<=n):
        while currentsum>s and start<=i-1:
            currentsum-=arr[start]
            start+=1
        if(currentsum==s):
            print("Sum found between indexes", start+1," and ",i)
            return 1
        if i<=n:
            currentsum+=arr[i]
        i+=1
    print("No subarray found")
    return 0
    
n=int(input("Enter the number of elements in an array : "))
arr=[]
for i in range(0,n):
    e=int(input("Enter element {}: ".format(i+1)))
    arr.append(e)
s=int(input("Enter the value of sum : "))
subarray(arr,n,s)   
```
```
Enter the number of elements in an array : 6
Enter element 1: 1
Enter element 2: 2
Enter element 3: 3
Enter element 4: 4
Enter element 5: 5
Enter element 6: 9
Enter the value of sum : 7
Sum found between indexes 3  and  4
1
```
Q9. Move all negative numbers to beginning and positive to end with constant extra space
```python
def reArrange(arr, n): 
    low,high = 0, n - 1
    while(low<high): 
        if(arr[low] < 0): 
            low += 1
        elif(arr[high] > 0): 
            high -= 1
        else: 
            arr[low],arr[high] = arr[high],arr[low] 
  
def displayArray(arr, n): 
  
    for i in range(n): 
        print(arr[i],end = " ") 
    
    print('') 
    
    
n=int(input("Enter the number of elements in an array : "))
arr=[]
for i in range(0,n):
    e=int(input("Enter element {}: ".format(i+1)))
    arr.append(e)
reArrange(arr,n)
displayArray(arr,n)
```
```
Enter the number of elements in an array : 6
Enter element 1: 1
Enter element 2: -1
Enter element 3: 2
Enter element 4: 4
Enter element 5: -3
Enter element 6: 5
-3 -1 2 4 1 5 
```
Q10. Given two sorted arrays, find their union and intersection.

Example:

Input: arr1[] = {1, 3, 4, 5, 7} arr2[] = {2, 3, 5, 6} Output: Union : {1, 2, 3, 4, 5, 6, 7} Intersection : {3, 5}

Input: arr1[] = {2, 5, 6} arr2[] = {4, 6, 8, 10} Output: Union : {2, 4, 5, 6, 8, 10} Intersection : {6}
```python
def find_union_and_intersection(arr1, arr2):
    m = len(arr1)
    n = len(arr2)
    union = []
    intersection = []
    i = 0
    j = 0

    while i < m and j < n:
        if arr1[i] == arr2[j]:
            intersection.append(arr1[i])
            union.append(arr1[i])
            i += 1
            j += 1
        elif arr1[i] < arr2[j]:
            union.append(arr1[i])
            i += 1
        else:
            union.append(arr2[j])
            j += 1

    # Add remaining elements of arr1 and arr2 to union
    while i < m:
        union.append(arr1[i])
        i += 1
    while j < n:
        union.append(arr2[j])
        j += 1

    return union, intersection

#Take user input for the arrays
arr1 = list(map(int, input("Enter the first sorted array elements separated by space: ").split()))
arr2 = list(map(int, input("Enter the second sorted array elements separated by space: ").split()))

#Call the function and print the results
union, intersection = find_union_and_intersection(arr1, arr2)
print("Union:", union)
print("Intersection:", intersection)
Enter the first sorted array elements separated by space: 1 2 3 4
Enter the second sorted array elements separated by space: 3 4 5
```
```
Union: [1, 2, 3, 4, 5]
Intersection: [3, 4]
```
Q11. Given an array, the task is to cyclically rotate the array clockwise by one time.

Examples:

Input: arr[] = {1, 2, 3, 4, 5} Output: arr[] = {5, 1, 2, 3, 4}

Input: arr[] = {2, 3, 4, 5, 1} Output: {1, 2, 3, 4, 5}
```python
def rotate(arr, n):
    last_el = arr[n - 1]
 
    for i in range(n - 1, 0, -1):
        arr[i] = arr[i - 1]
 
    arr[0] = last_el
 
 
n=int(input("Enter the number of elements in an array : "))
arr=[]
for i in range(0,n):
    e=int(input("Enter element {}: ".format(i+1)))
    arr.append(e)
print("Given array is :")
for i in range(0, n):
    print(arr[i], end=' ')
 
rotate(arr, n)
 
print("\nRotated array is :")
for i in range(0, n):
    print(arr[i], end=' ')
```
```
Enter the number of elements in an array : 6
Enter element 1: 1
Enter element 2: 4
Enter element 3: 5
Enter element 4: 2
Enter element 5: 3
Enter element 6: 8
Given array is :
1 4 5 2 3 8 
Rotated array is :
8 1 4 5 2 3 
```
### Hackerrank Challenge:
Q1. In this challenge, the user enters a string and a substring. You have to print the number of times that the substring occurs in the given string. String traversal will take place from left to right, not from right to left.

NOTE: String letters are case-sensitive.
```python
def count_substring(string, substring):
    count = 0
    sub_len = len(substring)
    for i in range(len(string) - sub_len + 1):
        if string[i:i+sub_len] == substring:
            count += 1
    return count


if __name__ == '__main__':
    string = input().strip()
    sub_string = input().strip()
    
    count = count_substring(string, sub_string)
    print(count)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/b7059341-8917-40e3-be3a-90f0ae5a1edf)

Q2. You are given a string S .
Your task is to find out if the string S contains: alphanumeric characters, alphabetical characters, digits, lowercase and uppercase characters.

```python
def analyze_string(S):
    is_alphanumeric = False
    is_alphabetical = False
    is_digits = False
    is_lowercase = False
    is_uppercase = False

    for char in S:
        if char.isalnum():
            is_alphanumeric = True
        if char.isalpha():
            is_alphabetical = True
        if char.isdigit():
            is_digits = True
        if char.islower():
            is_lowercase = True
        if char.isupper():
            is_uppercase = True

    return is_alphanumeric, is_alphabetical, is_digits, is_lowercase, is_uppercase


if __name__ == '__main__':
    s = input()
    alphanumeric, alphabetical, digits, lowercase, uppercase = analyze_string(s)

    print(alphanumeric)
    print(alphabetical)
    print(digits)
    print(lowercase)
    print(uppercase)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/a9cf7464-f534-4a8d-aaee-d81628be555e)

## Day 18: Trees (contd.)
Given a binary tree, the task is to find the height of the tree. The height of the tree is the number of vertices in the tree from the root to the deepest node.

```python
class Node:
 
    # Constructor to create a new node
    def __init__(self, data):
        self.data = data
        self.left = None
        self.right = None
 
# Compute the "maxDepth" of a tree -- the number of nodes
# along the longest path from the root node down to the
# farthest leaf node
 
 
def maxDepth(node):
    if node is None:
        return 0
 
    else:
 
        # Compute the depth of each subtree
        lDepth = maxDepth(node.left)
        rDepth = maxDepth(node.right)
 
        # Use the larger one
        if (lDepth > rDepth):
            return lDepth+1
        else:
            return rDepth+1
 
 
# Driver program to test above function
root = Node(1)
root.left = Node(2)
root.right = Node(3)
root.left.left = Node(4)
root.left.right = Node(5)
 
 
print("Height of tree is %d" % (maxDepth(root)))
```
Write a function to determine if two trees are identical or not:

Two trees are identical when they have the same data and the arrangement of data is also the same.
```python
class Node:
    # Constructor to create a new node
    def __init__(self, data):
        self.data = data
        self.left = None
        self.right = None
 
 
# Given two trees, return true if they are structurally
# identical
def identicalTrees(a, b):
 
    # 1. Both empty
    if a is None and b is None:
        return True
 
    # 2. Both non-empty -> Compare them
    if a is not None and b is not None:
        return ((a.data == b.data) and
                identicalTrees(a.left, b.left)and
                identicalTrees(a.right, b.right))
 
    # 3. one empty, one not -- false
    return False
 
 
# Driver code
root1 = Node(1)
root2 = Node(1)
root1.left = Node(2)
root1.right = Node(3)
root1.left.left = Node(4)
root1.left.right = Node(5)
 
root2.left = Node(2)
root2.right = Node(3)
root2.left.left = Node(4)
root2.left.right = Node(5)
 
# Function call
if __name__ == "__main__":
  if identicalTrees(root1, root2):
      print("Both trees are identical")
  else:
      print("Trees are not identical")
```
### Hackerrank Challenge
Q1. You are given a partial code that is used for generating the HackerRank Logo of variable thickness.
Your task is to replace the blank (______) with rjust, ljust or center.
```python
#Replace all ______ with rjust, ljust or center. 

thickness = int(input()) #This must be an odd number
c = 'H'

#Top Cone
for i in range(thickness):
    print((c*i).rjust(thickness-1)+c+(c*i).ljust(thickness-1))

#Top Pillars
for i in range(thickness+1):
    print((c*thickness).center(thickness*2)+(c*thickness).center(thickness*6))

#Middle Belt
for i in range((thickness+1)//2):
    print((c*thickness*5).center(thickness*6))    

#Bottom Pillars
for i in range(thickness+1):
    print((c*thickness).center(thickness*2)+(c*thickness).center(thickness*6))    

#Bottom Cone
for i in range(thickness):
    print(((c*(thickness-i-1)).rjust(thickness)+c+(c*(thickness-i-1)).ljust(thickness)).rjust(thickness*6))
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/31ae9d1c-19e3-473e-a57d-620d1a0589bc)
Q2. You are given a string S and width W.
Your task is to wrap the string into a paragraph of width w.
```python
import textwrap

def wrap(string, max_width):
    return textwrap.fill(string, max_width)

if __name__ == '__main__':
    string, max_width = input(), int(input())
    result = wrap(string, max_width)
    print(result)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/a3365a17-bacf-4b1b-aceb-b1e4a225ea67)

## Day 19 : Trees (Problems contd.)
Given a binary tree, the task is to convert the binary tree into its Mirror tree. Mirror of a Binary Tree T is another Binary Tree M(T) with left and right children of all non-leaf nodes interchanged. 
```python
class newNode:
    def __init__(self, data):
        self.data = data
        self.left = self.right = None

def mirror(node):
 
    if (node == None):
        return
    else:
 
        temp = node
 
        """ do the subtrees """
        mirror(node.left)
        mirror(node.right)
 
        """ swap the pointers in this node """
        temp = node.left
        node.left = node.right
        node.right = temp
 
 
""" Helper function to print Inorder traversal."""
 
 
def inOrder(node):
 
    if (node == None):
        return
 
    inOrder(node.left)
    print(node.data, end=" ")
    inOrder(node.right)
 
 
# Driver code
if __name__ == "__main__":
 
    root = newNode(1)
    root.left = newNode(2)
    root.right = newNode(3)
    root.left.left = newNode(4)
    root.left.right = newNode(5)
 
    """ Print inorder traversal of
        the input tree """
    print("Inorder traversal of the",
          "constructed tree is")
    inOrder(root)
 
    """ Convert tree to its mirror """
    mirror(root)
 
    """ Print inorder traversal of 
        the mirror tree """
    print("\nInorder traversal of",
          "the mirror tree is ")
    inOrder(root)
```
### Hackerrank Challenge:
Q1. Mr. Vincent works in a door mat manufacturing company. One day, he designed a new door mat with the following specifications:

Mat size must be N*M. (N is an odd natural number, and M is 3 times N.)
The design should have 'WELCOME' written in the center.
The design pattern should only use |, . and - characters.
```python
def create_door_mat(N, M):
    # Top design
    for i in range(N // 2):
        pattern = '.|.' * (2 * i + 1)
        print(pattern.center(M, '-'))

    # Welcome message
    print('WELCOME'.center(M, '-'))

    # Bottom design (similar to top but reversed)
    for i in range(N // 2 - 1, -1, -1):
        pattern = '.|.' * (2 * i + 1)
        print(pattern.center(M, '-'))

N,M = map(int,input().split())
create_door_mat(N, M)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/bbe69871-046e-473b-8cc4-3a2492eaa9f0)

Q2.Given an integer,n , print the following values for each integer i from 1 to n:

Decimal
Octal
Hexadecimal (capitalized)
Binary
```python
def print_formatted(number):
    width = len("{0:b}".format(number))
    for i in range(1, number + 1):
        decimal = "{0:{width}d}".format(i, width=width)
        octal = "{0:{width}o}".format(i, width=width)
        hexadecimal = "{0:{width}X}".format(i, width=width)
        binary = "{0:{width}b}".format(i, width=width)
        print(decimal, octal, hexadecimal, binary)
if __name__ == '__main__':
    n = int(input())
    print_formatted(n)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/2bd54455-f8a6-4291-a246-9c1f14758fab)

## Day 21 : Trees (Problems contd.)
Diameter of Tree in O(n)
```python
class TreeNode:
    def __init__(self, val):
        self.val = val
        self.left = None
        self.right = None

def build_tree():
    val = input("Enter the value of the node (or type 'None' if it's a null node): ")
    if val.lower() == 'none':
        return None
    node = TreeNode(int(val))
    node.left = build_tree()
    node.right = build_tree()
    return node

def height_and_diameter(node):
    if not node:
        return 0, 0
    
    left_height, left_diameter = height_and_diameter(node.left)
    right_height, right_diameter = height_and_diameter(node.right)
    
    current_height = max(left_height, right_height) + 1
    current_diameter = max(left_height + right_height, left_diameter, right_diameter)
    
    return current_height, current_diameter

def diameter_of_binary_tree(root):
    _, diameter = height_and_diameter(root)
    return diameter
# Main function to build the binary tree and calculate its diameter
def main():
    print("Enter the nodes of the binary tree (enter 'None' for null nodes):")
    root = build_tree()
    print("Diameter of the binary tree:", diameter_of_binary_tree(root))

if __name__ == "__main__":
    main()
```

Deletion in a Binary tree:
```python
class Node: 
    def __init__(self, data): 
        self.data = data 
        self.left = None
        self.right = None
  
# Inorder traversal of a binary tree 
  
  
def inorder(temp): 
    if(not temp): 
        return
    inorder(temp.left) 
    print(temp.data, end=" ") 
    inorder(temp.right) 
  
# function to delete the given deepest node (d_node) in binary tree 
  
  
def deleteDeepest(root, d_node): 
    q = [] 
    q.append(root) 
    while(len(q)): 
        temp = q.pop(0) 
        if temp is d_node: 
            temp = None
            return
        if temp.right: 
            if temp.right is d_node: 
                temp.right = None
                return
            else: 
                q.append(temp.right) 
        if temp.left: 
            if temp.left is d_node: 
                temp.left = None
                return
            else: 
                q.append(temp.left) 
  
# function to delete element in binary tree 
  
  
def deletion(root, key): 
    if root == None: 
        return None
    if root.left == None and root.right == None: 
        if root.key == key: 
            return None
        else: 
            return root 
    key_node = None
    q = [] 
    q.append(root) 
    temp = None
    while(len(q)): 
        temp = q.pop(0) 
        if temp.data == key: 
            key_node = temp 
        if temp.left: 
            q.append(temp.left) 
        if temp.right: 
            q.append(temp.right) 
    if key_node: 
        x = temp.data 
        deleteDeepest(root, temp) 
        key_node.data = x 
    return root 
  
  
# Driver code 
if __name__ == '__main__': 
    root = Node(10) 
    root.left = Node(11) 
    root.left.left = Node(7) 
    root.left.right = Node(12) 
    root.right = Node(9) 
    root.right.left = Node(15) 
    root.right.right = Node(8) 
    print("The tree before the deletion: ", end = "") 
    inorder(root) 
    key = 11
    root = deletion(root, key) 
    print(); 
    print("The tree after the deletion: ", end = "") 
    inorder(root) 
```
### Hackerrank Challenge:
Q1. You are given an integer, N. Your task is to print an alphabet rangoli of size N . (Rangoli is a form of Indian folk art based on creation of patterns.)
```python
def print_rangoli(size):
    import string
    
    # Create alphabet list
    alphabet = string.ascii_lowercase
    
    # Create the upper half of the rangoli
    for i in range(size-1, -size, -1):
        row = ['-'] * (2*size-1)
        for j in range(size - abs(i)):
            row[size - 1 - j] = alphabet[abs(i) + j]
            row[size - 1 + j] = alphabet[abs(i) + j]
        print('-'.join(row))

if __name__ == '__main__':
    n = int(input())
    print_rangoli(n)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/962a87e6-cab9-4508-b131-af199040f97d)

Q2.You are asked to ensure that the first and last names of people begin with a capital letter in their passports. For example, alison heck should be capitalised correctly as Alison Heck.
Given a full name, your task is to capitalize the name appropriately.
```python
#!/bin/python3

import math
import os
import random
import re
import sys

# Complete the solve function below.
def solve(s):
    return s.title()

if __name__ == '__main__':
    fptr = open(os.environ['OUTPUT_PATH'], 'w')

    s = input()

    result = solve(s)

    fptr.write(result + '\n')

    fptr.close()

```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/a5cdf9ae-19f1-4180-9def-1df77bd4b796)
## Day 22 : Trees (Problems contd.)
To check if a tree is height-balanced
```python
class Node:
    # Constructor to create a new Node
    def __init__(self, data):
        self.data = data
        self.left = None
        self.right = None
 
# function to find height of binary tree
 
 
def height(root):
 
    # base condition when binary tree is empty
    if root is None:
        return 0
    return max(height(root.left), height(root.right)) + 1
 
# function to check if tree is height-balanced or not
 
 
def isBalanced(root):
 
    # Base condition
    if root is None:
        return True
 
    # for left and right subtree height
    lh = height(root.left)
    rh = height(root.right)
 
    # allowed values for (lh - rh) are 1, -1, 0
    if (abs(lh - rh) <= 1) and isBalanced(
            root.left) is True and isBalanced(root.right) is True:
        return True
 
    # if we reach here means tree is not
    # height-balanced tree
    return False
 
 
# Driver function to test the above function
root = Node(1)
root.left = Node(2)
root.right = Node(3)
root.left.left = Node(4)
root.left.right = Node(5)
root.left.left.left = Node(8)
if isBalanced(root):
    print("Tree is balanced")
else:
    print("Tree is not balanced")
```
### Hackerrank Challenge:
Q1. You are asked to ensure that the first and last names of people begin with a capital letter in their passports. For example, alison heck should be capitalised correctly as Alison Heck.
Given a full name, your task is to capitalize the name appropriately.
```python
#!/bin/python3

import os

# Complete the solve function below.
def solve(s):
    return s.title()

if __name__ == '__main__':
    fptr = open(os.environ['OUTPUT_PATH'], 'w')

    s = input()

    result = solve(s)

    fptr.write(result + '\n')

    fptr.close()

```
Output:
![Screenshot 2024-02-15 212601](https://github.com/bijayaroy/python-daily-learning/assets/93483189/9c003fcf-2158-4f04-be08-54d0d29d607e)

Q2. Kevin and Stuart want to play the 'The Minion Game'.

Game Rules

Both players are given the same string,s .
Both players have to make substrings using the letters of the string s .
Stuart has to make words starting with consonants.
Kevin has to make words starting with vowels.
The game ends when both players have made all possible substrings.

Scoring
A player gets +1 point for each occurrence of the substring in the string s.

For Example:
String  = BANANA
Kevin's vowel beginning word = ANA
Here, ANA occurs twice in BANANA. Hence, Kevin will get 2 Points
```python
def minion_game(string):
    vowels = 'AEIOU'
    kevin_score = 0
    stuart_score = 0
    length = len(string)

    for i in range(length):
        if string[i] in vowels:
            kevin_score += length - i
        else:
            stuart_score += length - i

    if kevin_score > stuart_score:
        print("Kevin", kevin_score)
    elif kevin_score < stuart_score:
        print("Stuart", stuart_score)
    else:
        print("Draw")


if __name__ == '__main__':
    s = input()
    minion_game(s)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/d5db4d47-f284-4ac7-a1ab-89c40b464f1a)

## Day 23: Trees (Problems contd.)
### Hackerrank Challenge:
Q1. Consider the following:


A string, s, of length n where s = c0c1. . . . cn-1.

An integer, k, where k is a factor of n.

We can split s into n/k substrings where each subtring, ti, consists of a contiguous block of k characters in s. Then, use each ti to create string ui such that:

The characters in ui are a subsequence of the characters in ti.

Any repeat occurrence of a character is removed from the string such that each character in ui occurs exactly once. In other words, if the character at some index j in ti occurs at a previous index < j in ti, then do not include the character in string ui.

Given s and k, print n/k lines where each line i denotes string ui.

Example

s = “AAABCADDE”

k = 3

There are three substrings of length 3 to consider: ‘AAA’, ‘BCA’ and ‘DDE’. The first substring is all ‘A’ characters, so u1 = ‘A’. The second substring has all distinct characters, so u2 = ‘BCA’. The third substring has 2 different characters, so u3 = ‘DE’. Note that a subsequence maintains the original order of characters encountered. The order of characters in each subsequence shown is important.
```python
def merge_the_tools(string, k):
    temp = []
    len_temp = 0
    for item in string:
        len_temp += 1
        if item not in temp:
            temp.append(item)
        if len_temp == k:
            print (''.join(temp))
            temp = []
            len_temp = 0
if __name__ == '__main__':
    string, k = input(), int(input())
    merge_the_tools(string, k)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/e86c6c16-1ef9-4767-9b74-066b9ca60e2f)

Q2. Raghu is a shoe shop owner. His shop has X number of shoes.

He has a list containing the size of each shoe he has in his shop.

There are N number of customers who are willing to pay xi amount of money only if they get the shoe of their desired size.

Your task is to compute how much money Raghu earned.
```python
# Enter your code here. Read input from STDIN. Print output to STDOUT
#First we imported the counter from collections.
from collections import Counter
#then we have taken the input of x i.e, the total number of shoes.
x = int(input())
#and we have taken the input of y i.e, the list of all shoe sizes. Then we used counter to arrange our list as a dictionary.
y = Counter(map(int, input().split()))
#we’ve also taken the input of z i.e, the total number of customers.
z = int(input())
#then we created a variable to store the total.
total = 0
# then we created a for loop in the range of z(total number of customers)
for i in range(z):
    #inside for loop, we have taken the input of size and rate from each customer. Then we used an if condition to verify the input size is in y.
    size, rate = map(int, input().split())
    if y[size]: 
        y[size] -= 1
        #then we added all the rates in our total and printed it.
        total += rate
print(total)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/dd29056c-7a08-435c-bc42-31c1dee461b7)

## Day 24: Queue :
A queue is a linear data structure that follows the First In First Out (FIFO) principle. This means that elements are added to the rear (back) of the queue and removed from the front (head). Queues are often used to implement buffers, job scheduling, and other systems where elements need to be processed in a specific order.
There are several different ways to implement a queue. One common approach is to use a linked list. In this implementation, each element in the queue is represented by a node in the linked list. The rear of the queue is the last node in the linked list, and the front of the queue is the first node in the linked list.
Another common approach to implementing a queue is to use an array. In this implementation, the elements of the queue are stored in an array. The rear of the queue is the index of the last element in the array, and the front of the queue is the index of the first element in the array.


FIFO Principle of Queue:
A Queue is like a line waiting to purchase tickets, where the first person in line is the first person served. (i.e. First come first serve).
Position of the entry in a queue ready to be served, that is, the first entry that will be removed from the queue, is called the front of the queue(sometimes, head of the queue), similarly, the position of the last entry in the queue, that is, the one most recently added, is called the rear (or the tail) of the queue. See the below figure.


Characteristics of Queue:
- Queue can handle multiple data.
- We can access both ends.
- They are fast and flexible.


Here are some of the operations that can be performed on a queue:
Enqueue: Adds an element to the rear of the queue.
Dequeue: Removes an element from the front of the queue.
Peek: Returns the element at the front of the queue without removing it.
IsEmpty: Returns true if the queue is empty, and false otherwise.


Q. Implement a queue using an array
```python
class Queue:

	# To initialize the object.
	def __init__(self, c):

		self.queue = []
		self.front = self.rear = 0
		self.capacity = c

	# Function to insert an element
	# at the rear of the queue
	def queueEnqueue(self, data):

		# Check queue is full or not
		if(self.capacity == self.rear):
			print("\nQueue is full")

		# Insert element at the rear
		else:
			self.queue.append(data)
			self.rear += 1

	# Function to delete an element
	# from the front of the queue
	def queueDequeue(self):

		# If queue is empty
		if(self.front == self.rear):
			print("Queue is empty")

		# Pop the front element from list
		else:
			x = self.queue.pop(0)
			self.rear -= 1

	# Function to print queue elements
	def queueDisplay(self):

		if(self.front == self.rear):
			print("\nQueue is Empty")

		# Traverse front to rear to
		# print elements
		for i in self.queue:
			print(i, "<--", end='')

	# Print front of queue
	def queueFront(self):

		if(self.front == self.rear):
			print("\nQueue is Empty")

		print("\nFront Element is:",
			self.queue[self.front])


# Driver code
if __name__ == '__main__':

	# Create a new queue of
	# capacity 4
	q = Queue(4)

	# Print queue elements
	q.queueDisplay()

	# Inserting elements in the queue
	q.queueEnqueue(20)
	q.queueEnqueue(30)
	q.queueEnqueue(40)
	q.queueEnqueue(50)

	# Print queue elements
	q.queueDisplay()

	# Insert element in queue
	q.queueEnqueue(60)

	# Print queue elements
	q.queueDisplay()

	q.queueDequeue()
	q.queueDequeue()
	print("\n\nafter two node deletion\n")

	# Print queue elements
	q.queueDisplay()

	# Print front of queue
	q.queueFront()
```


### Hackerrank Challenge:
Q1. In this challenge, you will be given 2 integers, n and m. There are n words, which might repeat, in word group A. There are m words belonging to word group B. For each m words, check whether the word has appeared in group A or not. Print the indices of each occurrence of m in group A. If it does not appear, print -1.
Steps Used in solving the problem -
Step 1: First we imported defaultdict from collections.
Step 2: then we have taken the input of input_n and input_m.
Step 3: then we defined defaultdict as d.
Step 4: In the fourth line, we create a for loop in the range of input_n.
Step 5: Inside for loop, we have taken input and appended it into d. 
Step 6: then we created another for loop in the range of input_m.
Step 7: Inside for loop, we have taken input. Then we used an if condition to check if ans2 is in d then print the index value of ans2 else print -1.
```python
from collections import defaultdict
input_n, input_m = map(int, input().split())
d = defaultdict(list)
for i in range(input_n):
    ans1 = input()
    d[ans1].append(i+1)
for j in range(input_m):
    ans2 = input()
    if ans2 in d:
        print(*d[ans2])
    else:
        print(-1)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/a1eb52e1-0e1b-4e0c-b254-62c4c2aa39b4)

Q2. Dr. John Wesley has a spreadsheet containing a list of student’s IDs, marks, class and name.

Your task is to help Dr. Wesley calculate the average marks of the students.

Average = Sum of all marks / Total Students

Note:
1. Columns can be in any order. IDs, marks, class and name can be written in any order in the spreadsheet.
2. Column names are ID, MARKS, CLASS and NAME. (The spelling and case type of these names won’t change.)
```python
from collections import namedtuple
input_ = int(input())
my_fields = input().split()
total_marks = 0
for _ in range(input_):
    students = namedtuple('my_student', my_fields)
    MARKS, CLASS, NAME, ID = input().split()
    my_student = students(MARKS, CLASS, NAME, ID)
    total_marks += int(my_student.MARKS)
print((total_marks / input_))
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/14afb45e-8bde-4615-9aaf-1245b19e5985)
## Day 25: Stack
A stack is a fundamental data structure in computer science that follows the Last In, First Out (LIFO) principle. This means that the last element added to the stack is the first one to be removed. It operates much like a stack of plates in a cafeteria, where you can only add or remove plates from the top of the stack.

The stack data structure supports two primary operations: push and pop.

Push: This operation adds an element to the top of the stack.
Pop: This operation removes the element at the top of the stack.
Additionally, there are two other common operations associated with stacks:

Peek (or Top): This operation retrieves the element at the top of the stack without removing it.
isEmpty: This operation checks if the stack is empty or not.
```python
class Stack:
    def __init__(self):
        self.items = []

    def push(self, item):
        """Add an element to the top of the stack."""
        self.items.append(item)

    def pop(self):
        """Remove and return the element at the top of the stack."""
        if not self.is_empty():
            return self.items.pop()
        else:
            raise IndexError("pop from empty stack")

    def peek(self):
        """Return the element at the top of the stack without removing it."""
        if not self.is_empty():
            return self.items[-1]
        else:
            return None

    def is_empty(self):
        """Check if the stack is empty."""
        return len(self.items) == 0

    def size(self):
        """Return the number of elements in the stack."""
        return len(self.items)

```
```python
stack = Stack()

stack.push(1)
stack.push(2)
stack.push(3)

print("Stack size:", stack.size())  # Output: 3
print("Top of the stack:", stack.peek())  # Output: 3

print("Popped item:", stack.pop())  # Output: 3
print("Popped item:", stack.pop())  # Output: 2

print("Is the stack empty?", stack.is_empty())  # Output: False

print("Popped item:", stack.pop())  # Output: 1
print("Is the stack empty?", stack.is_empty())  # Output: True

# Trying to pop from an empty stack will raise an IndexError
# print("Popped item:", stack.pop())  # Output: IndexError: pop from empty stack

```
### Hackerrank Challenge:
Q1. You are the manager of a supermarket.
You have a list of N items together with their prices that consumers bought on a particular day.
Your task is to print each item_name and net_price in order of its first occurrence.

item_name = Name of the item.
net_price = Quantity of the item sold multiplied by the price of each item.

```python
from collections import OrderedDict
a = OrderedDict()
input_ = int(input())
for _ in range(input_):
    item, space, price = input().rpartition(' ')
    a[item] = a.get(item, 0) + int(price)
for item, price in a.items():
    print(item, price)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/caf8d043-d670-43d1-ad1c-15f9cd915ad7)

Q2. You are given n words. Some words may repeat. For each word, output its number of occurrences. The output order should correspond with the input order of appearance of the word. See the sample input/output for clarification. Note: Each input line ends with a "\n" character.
Steps Followed:

In the first line of code we have imported counter from collections.
As the problem statement suggests we need to find the count of words. So for that, we have created a list of words.
In the next step we convert that list to a unique list using the counter module in python. 
Next in the step we printed the count of unique words in the list using len method.
Lastly we .values() method to find and print all the values of words inside res variable
```python
from collections import Counter
n = int(input())
l1 = [input().strip() for _ in range(n)]
res = Counter(l1)
print(len(res))
print(*res.values())
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/fd9f3045-6ca6-4cff-8de9-28d496a3224a)

## Day 26: Stack and Queue (contd.)
Q. Given an expression string exp, write a program to examine whether the pairs and the orders of “{“, “}”, “(“, “)”, “[“, “]” are correct in the given expression.
```python
def areBracketsBalanced(expr):
    stack = []
 
    # Traversing the Expression
    for char in expr:
        if char in ["(", "{", "["]:
 
            # Push the element in the stack
            stack.append(char)
        else:
 
            # IF current character is not opening
            # bracket, then it must be closing.
            # So stack cannot be empty at this point.
            if not stack:
                return False
            current_char = stack.pop()
            if current_char == '(':
                if char != ")":
                    return False
            if current_char == '{':
                if char != "}":
                    return False
            if current_char == '[':
                if char != "]":
                    return False
 
    # Check Empty Stack
    if stack:
        return False
    return True
 
 
# Driver Code
if __name__ == "__main__":
    expr = "{()}[]"
 
    # Function call
    if areBracketsBalanced(expr):
        print("Balanced")
    else:
        print("Not Balanced")
```
Q.Implementation of Deque using circular array
```python
MAX = 100
 
 
class Deque:
    def __init__(self, size):
        self.arr = [0] * MAX
        self.front = -1
        self.rear = 0
        self.size = size
 
    ''' Operations on Deque:
    void  insertfront(int key);
    void  insertrear(int key);
    void  deletefront();
    void  deleterear();
    bool  isFull();
    bool  isEmpty();
    int  getFront();
    int  getRear(); '''
 
    # Checks whether Deque is full or not.
    def isFull(self):
        return ((self.front == 0 and self.rear == self.size-1) or self.front == self.rear + 1)
 
    # Checks whether Deque is empty or not.
 
    def isEmpty(self):
        return (self.front == -1)
 
    # Inserts an element at front
    def insertfront(self, key):
 
        # check whether Deque if  full or not
        if (self.isFull()):
            print("Overflow")
            return
 
        # If queue is initially empty
        if (self.front == -1):
            self.front = 0
            self.rear = 0
 
        # front is at first position of queue
        elif (self.front == 0):
            self.front = self.size - 1
 
        else:  # decrement front end by '1'
            self.front = self.front-1
 
        # insert current element into Deque
        self.arr[self.front] = key
 
    # function to inset element at rear end
    # of Deque.
 
    def insertrear(self, key):
        if (self.isFull()):
            print(" Overflow")
            return
 
        # If queue is initially empty
        if (self.front == -1):
            self.front = 0
            self.rear = 0
 
        # rear is at last position of queue
        elif (self.rear == self.size-1):
            self.rear = 0
 
        # increment rear end by '1'
        else:
            self.rear = self.rear+1
 
        # insert current element into Deque
        self.arr[self.rear] = key
 
    # Deletes element at front end of Deque
 
    def deletefront(self):
        # check whether Deque is empty or not
        if (self.isEmpty()):
            print("Queue Underflow")
            return
 
        # Deque has only one element
        if (self.front == self.rear):
            self.front = -1
            self.rear = -1
 
        else:
            # back to initial position
            if (self.front == self.size - 1):
                self.front = 0
 
            else:  # increment front by '1' to remove current
                # front value from Deque
                self.front = self.front+1
 
    # Delete element at rear end of Deque
 
    def deleterear(self):
        if (self.isEmpty()):
            print(" Underflow")
            return
 
        # Deque has only one element
        if (self.front == self.rear):
            self.front = -1
            self.rear = -1
 
        elif (self.rear == 0):
            self.rear = self.size-1
        else:
            self.rear = self.rear-1
 
    # Returns front element of Deque
 
    def getFront(self):
        # check whether Deque is empty or not
        if (self.isEmpty()):
            print(" Underflow")
            return -1
 
        return self.arr[self.front]
 
    # function return rear element of Deque
 
    def getRear(self):
        # check whether Deque is empty or not
        if(self.isEmpty() or self.rear < 0):
            print(" Underflow")
            return -1
 
        return self.arr[self.rear]
 
 
# Driver code
if __name__ == "__main__":
  dq = Deque(5)
 
  # Function calls
  print("Insert element at rear end  : 5 ")
  dq.insertrear(5)
 
  print("insert element at rear end : 10 ")
  dq.insertrear(10)
 
  print(f"get rear element : {dq.getRear()}")
 
  dq.deleterear()
  print(f"After delete rear element new rear become : {dq.getRear()}")
 
  print("inserting element at front end")
  dq.insertfront(15)
 
  print(f"get front element: {dq.getFront()}")
 
  dq.deletefront()
 
  print(f"After delete front element new front become : {dq.getFront()}")
```
Q.Check if a queue can be sorted into another queue using a stack
```python
from queue import Queue 
 
# Function to check if given queue element 
# can be sorted into another queue using a 
# stack. 
def checkSorted(n, q):
    st = [] 
    expected = 1
    fnt = None
 
    # while given Queue is not empty. 
    while (not q.empty()): 
        fnt = q.queue[0] 
        q.get() 
 
        # if front element is the 
        # expected element 
        if (fnt == expected): 
            expected += 1
 
        else:
             
            # if stack is empty, put the element 
            if (len(st) == 0):
                st.append(fnt)
 
            # if top element is less than element which 
            # need to be puted, then return false. 
            elif (len(st) != 0 and st[-1] < fnt): 
                return False
 
            # else put into the stack. 
            else:
                st.append(fnt)
 
        # while expected element are coming 
        # from stack, pop them out. 
        while (len(st) != 0 and
                   st[-1] == expected): 
            st.pop() 
            expected += 1
 
    # if the final expected element value is equal 
    # to initial Queue size and the stack is empty. 
    if (expected - 1 == n and len(st) == 0): 
        return True
 
    return False
 
# Driver Code
if __name__ == '__main__':
    q = Queue()
    q.put(5) 
    q.put(1) 
    q.put(2) 
    q.put(3) 
    q.put(4) 
 
    n = q.qsize() 
 
    if checkSorted(n, q):
        print("Yes")
    else:
        print("No")
```
### Hackerrank Challenge:
Q1.You are given a string .
Your task is to print all possible permutations of size k of the string in lexicographic sorted order.
```python
from itertools import permutations
str1, int1 = input().split()

for i in sorted(permutations(str1, int(int1))):
    print (''.join(i))
```
Output:
![Screenshot 2024-02-26 200512](https://github.com/bijayaroy/python-daily-learning/assets/93483189/384d7743-06ea-4b1f-92fa-9f03ca7e489d)

Q2.You are given a string .
Your task is to print all possible combinations, up to size , of the string in lexicographic sorted order.
```python
from itertools import combinations
word , length  = input().split()
for i in range(1, int(length)+1):
    for j in combinations(sorted(word), i):
        print (''.join(j))
```
Output:
![Screenshot 2024-02-26 200809](https://github.com/bijayaroy/python-daily-learning/assets/93483189/e9e6cd7a-26c9-445e-9725-56495644c831)

## Day 27: Stack and Queue:
Q.How to Reverse a String using Stack
```python
def createStack():
    stack = []
    return stack
 
# Function to determine the size of the stack
 
 
def size(stack):
    return len(stack)
 
# Stack is empty if the size is 0
 
 
def isEmpty(stack):
    if size(stack) == 0:
        return true
 
# Function to add an item to stack .
# It increases size by 1
 
 
def push(stack, item):
    stack.append(item)
 
# Function to remove an item from stack.
# It decreases size by 1
 
 
def pop(stack):
    if isEmpty(stack):
        return
    return stack.pop()
 
# A stack based function to reverse a string
 
 
def reverse(string):
    n = len(string)
 
    # Create a empty stack
    stack = createStack()
 
    # Push all characters of string to stack
    for i in range(0, n, 1):
        push(stack, string[i])
 
    # Making the string empty since all
    # characters are saved in stack
    string = ""
 
    # Pop all characters of string and
    # put them back to string
    for i in range(0, n, 1):
        string += pop(stack)
 
    return string
# Driver program to test above functions
string = "GeeksQuiz"
string = reverse(string)
print("Reversed string is " + string)
```
Q2.Implement Circular Queue using Array:
```python
class CircularQueue():
 
    # constructor
    def __init__(self, size): # initializing the class
        self.size = size
         
        # initializing queue with none
        self.queue = [None for i in range(size)] 
        self.front = self.rear = -1
 
    def enqueue(self, data):
         
        # condition if queue is full
        if ((self.rear + 1) % self.size == self.front): 
            print(" Queue is Full\n")
             
        # condition for empty queue
        elif (self.front == -1): 
            self.front = 0
            self.rear = 0
            self.queue[self.rear] = data
        else:
             
            # next position of rear
            self.rear = (self.rear + 1) % self.size 
            self.queue[self.rear] = data
             
    def dequeue(self):
        if (self.front == -1): # condition for empty queue
            print ("Queue is Empty\n")
             
        # condition for only one element
        elif (self.front == self.rear): 
            temp=self.queue[self.front]
            self.front = -1
            self.rear = -1
            return temp
        else:
            temp = self.queue[self.front]
            self.front = (self.front + 1) % self.size
            return temp
 
    def display(self):
     
        # condition for empty queue
        if(self.front == -1): 
            print ("Queue is Empty")
 
        elif (self.rear >= self.front):
            print("Elements in the circular queue are:", 
                                              end = " ")
            for i in range(self.front, self.rear + 1):
                print(self.queue[i], end = " ")
            print ()
 
        else:
            print ("Elements in Circular Queue are:", 
                                           end = " ")
            for i in range(self.front, self.size):
                print(self.queue[i], end = " ")
            for i in range(0, self.rear + 1):
                print(self.queue[i], end = " ")
            print ()
 
        if ((self.rear + 1) % self.size == self.front):
            print("Queue is Full")
 
# Driver Code
ob = CircularQueue(5)
ob.enqueue(14)
ob.enqueue(22)
ob.enqueue(13)
ob.enqueue(-6)
ob.display()
print ("Deleted value = ", ob.dequeue())
print ("Deleted value = ", ob.dequeue())
ob.display()
ob.enqueue(9)
ob.enqueue(20)
ob.enqueue(5)
ob.display()
```
Q.Implement Stack using Queues
```python
from _collections import deque
 
 
class Stack:
 
    def __init__(self):
 
        # Two inbuilt queues
        self.q1 = deque()
        self.q2 = deque()
 
    def push(self, x):
 
        # Push x first in empty q2
        self.q2.append(x)
 
        # Push all the remaining
        # elements in q1 to q2.
        while (self.q1):
            self.q2.append(self.q1.popleft())
 
        # swap the names of two queues
        self.q1, self.q2 = self.q2, self.q1
 
    def pop(self):
 
        # if no elements are there in q1
        if self.q1:
            self.q1.popleft()
 
    def top(self):
        if (self.q1):
            return self.q1[0]
        return None
 
    def size(self):
        return len(self.q1)
 
 
# Driver Code
if __name__ == '__main__':
    s = Stack()
    s.push(1)
    s.push(2)
    s.push(3)
 
    print("current size: ", s.size())
    print(s.top())
    s.pop()
    print(s.top())
    s.pop()
    print(s.top())
 
    print("current size: ", s.size())
```
### Hackerrank Challenge:
Q1.You are given a string .
Your task is to print all possible size  replacement combinations of the string in lexicographic sorted order.
```python
from itertools import combinations_with_replacement

io = input().split();
char = sorted(io[0]);
N = int(io[1]);

for i in combinations_with_replacement(char,N):
    print(''.join(i));

```
Output:
![Screenshot 2024-02-26 201015](https://github.com/bijayaroy/python-daily-learning/assets/93483189/7f5db6e6-db0a-4a29-8f3f-06c8a2c3de0f)

Q2.You are given a string S. Suppose a character 'c' occurs consecutively X times in the string. Replace these consecutive occurrences of the character 'c' with (X,c)
in the string.
```python
from itertools import *

io = input()
for i,j in groupby(map(int,list(io))):
    print(tuple([len(list(j)), i]) ,end = " ")
```
Output:
![Screenshot 2024-02-26 201308](https://github.com/bijayaroy/python-daily-learning/assets/93483189/30232612-e561-49ea-9f55-5d6482bc9bf8)

## Day 28 : Searching Algorithm
Linear Search:
Linear Search is defined as a sequential search algorithm that starts at one end and goes through each element of a list until the desired element is found, otherwise the search continues till the end of the data set.


How Does Linear Search Algorithm Work?
- Every element is considered as a potential match for the key and checked for the same.
- If any element is found equal to the key, the search is successful and the index of that element is returned.
- If no element is found equal to the key, the search yields “No match found”.
Implementation:
```python
def search(arr, N, x):
 
    for i in range(0, N):
        if (arr[i] == x):
            return i
    return -1
 
 
# Driver Code
if __name__ == "__main__":
    arr = [2, 3, 4, 10, 40]
    x = 10
    N = len(arr)
 
    # Function call
    result = search(arr, N, x)
    if(result == -1):
        print("Element is not present in array")
    else:
        print("Element is present at index", result)
```
Time Complexity:

- Best Case: In the best case, the key might be present at the first index. So the best case complexity is O(1)
- Worst Case: In the worst case, the key might be present at the last index i.e., opposite to the end from which the search has started in the list. So the worst-case complexity is O(N) where N is the size of the list.
- Average Case: O(N)
Auxiliary Space: O(1) as except for the variable to iterate through the list, no other variable is used. 


Advantages of Linear Search:
- Linear search can be used irrespective of whether the array is sorted or not. It can be used on arrays of any data type.
- Does not require any additional memory.
It is a well-suited algorithm for small datasets.


Drawbacks of Linear Search:
- Linear search has a time complexity of O(N), which in turn makes it slow for large datasets.
- Not suitable for large arrays.

- 
When to use Linear Search?
- When we are dealing with a small dataset.
- When you are searching for a dataset stored in contiguous memory.


### Hackerrank Challenge:
Q1. You are given a complex z. Your task is to convert it to polar coordinates.
```python
import cmath
n = input()
s = complex(n)
print(abs(s))
print(cmath.phase(s))
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/ae14e9de-2b28-47d9-90e9-0de1ef4fda54)

Q2. ABC is a right triangle, 90o at B.
Therefore, angle ABC = 90o.
Point M is the midpoint of hypotenuse AC.

You are given the lengths AB and BC.
Your task is to find the angle MBC in degrees.
```python
from math import degrees, atan2

AB = float(input())
BC = float(input())

MBC = round(degrees(atan2(AB, BC)))
print((str(MBC)), chr(176), sep='')
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/58722500-cae9-4966-9963-304e41e21500)

## Day 29 : Searching Algorithm (contd.)
Sentinel Linear Search:
Sentinel Linear Search as the name suggests is a type of Linear Search where the number of comparisons is reduced as compared to a traditional linear search. In a traditional linear search, only N comparisons are made, and in a Sentinel Linear Search, the sentinel value is used to avoid any out-of-bounds comparisons, but there is no additional comparison made specifically for the index of the element being searched.

Implementation:
```python
def sentinelSearch(arr, n, key):
 
    # Last element of the array
    last = arr[n - 1]
 
    # Element to be searched is
    # placed at the last index
    arr[n - 1] = key
    i = 0
 
    while (arr[i] != key):
        i += 1
 
    # Put the last element back
    arr[n - 1] = last
 
    if ((i < n - 1) or (arr[n - 1] == key)):
        print(key, "is present at index", i)
    else:
        print("Element Not found")
 
 
# Driver code
arr = [10, 20, 180, 30, 60, 50, 110, 100, 70]
n = len(arr)
key = 180
 
sentinelSearch(arr, n, key)
```

Time Complexity: O(N)
Auxiliary Space: O(1)

Binary Search:
Binary Search is defined as a searching algorithm used in a sorted array by repeatedly dividing the search interval in half. The idea of binary search is to use the information that the array is sorted and reduce the time complexity to O(log N). 

Conditions for when to apply Binary Search in a Data Structure:
To apply Binary Search algorithm:

- The data structure must be sorted.
- Access to any element of the data structure takes constant time.

Implementation:
```python
def binarySearch(arr, l, r, x):
 
    while l <= r:
 
        mid = l + (r - l) // 2
 
        # Check if x is present at mid
        if arr[mid] == x:
            return mid
 
        # If x is greater, ignore left half
        elif arr[mid] < x:
            l = mid + 1
 
        # If x is smaller, ignore right half
        else:
            r = mid - 1
 
    # If we reach here, then the element
    # was not present
    return -1
 
 
# Driver Code
if __name__ == '__main__':
    arr = [2, 3, 4, 10, 40]
    x = 10
 
    # Function call
    result = binarySearch(arr, 0, len(arr)-1, x)
    if result != -1:
        print("Element is present at index", result)
    else:
        print("Element is not present in array")
```
### Hackerrank Challenge:
Q1.Now, let's use our knowledge of sets and help Mickey.

Ms. Gabriel Williams is a botany professor at District College. One day, she asked her student Mickey to compute the average of all the plants with distinct heights in her greenhouse.
```python
def average(array):
    my_set = set(array)
    avg = sum(my_set)/len(my_set)
    
    return (avg)
         
if __name__ == '__main__':
    n = int(input())
    arr = list(map(int, input().split()))
    result = average(arr)
    print(result)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/487e3fb3-1562-4cca-a991-2aa3023f1d65)

Q2. Given 2 sets of integers, M and N, print their symmetric difference in ascending order. The term symmetric difference indicates those values that exist in either M or N but do not exist in both.

```python
n1 = int(input())
set_a = set(map(int,input().split()))
n2 = int(input())
set_b = set(map(int,input().split()))
a = (set_a.difference(set_b))
b = (set_b.difference(set_a))
ans = a.union(b)
for i in sorted(ans):
        print (i)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/43244285-6195-4cac-8fac-52eb8ebe01ef)
