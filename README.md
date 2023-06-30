# Python Cheatsheet

## Data Types in Python

 **Checking Dat types in python:**
  ```py
 print(type(10))                  # Int
print(type(3.14))                # Float
print(type(1 + 3j))              # Complex
print(type('Umer'))          # String
print(type([1, 2, 3]))           # List
print(type({'name':'Umer'})) # Dictionary
print(type({9.8, 3.14, 2.7}))    # Set
print(type((9.8, 3.14, 2.7)))    # Tuple
   ```

## Built in Functions in Python

 **print() - Used to display output to the console:**
  ```py
print('Hello! Dev')
   ```
 **input() - Reads input from the user through the console:**
  ```py
name = input("Enter your name: ")
print(f"Hello! {name}")
   ```

 **len() - Returns the length of an object (such as a string, list, or tuple):**
  ```py
language = 'Python'
print(len(language))
   ```


 **int() - Converts a value to an integer:**
  ```py
my_string = "42"
my_int = int(my_string)
print(my_int)  # Output: 42
   ```

 **float() - Converts a value to a floating-point number:**
  ```py
my_string = "3.14"
my_float = float(my_string)
print(my_float)  # Output: 3.14
   ```

**str() - Converts a value to a string:**
  ```py
my_number = 42
my_string = str(my_number)
print(my_string)  # Output: "42"
   ```



**list() - Creates a list from an iterable (e.g., a string or tuple):**
  ```py
my_string = "Hello"
my_list = list(my_string)
print(my_list)  # Output: ['H', 'e', 'l', 'l', 'o']
   ```

**dict() - Creates a dictionary:**
  ```py
my_dict = dict(firstName="Muhammad", lastName="Umer")
print(my_dict)  # Output: {'firstName': 'Muhammad', 'lastName': 'Umer'}
   ```



**min() - Returns the minimum value from an iterable or multiple arguments:**
  ```py
numbers = [5, 2, 7, 1, 9]
print(min(numbers))  # Output: 1

   ```




**max() - Returns the maximum value from an iterable or multiple arguments:**
  ```py
numbers = [5, 2, 7, 1, 9]
print(max(numbers))  # Output: 9
   ```
   

**sum() - Returns the sum of all elements in an iterable:**
  ```py
numbers = [1, 2, 3, 4, 5]
print(sum(numbers))  # Output: 15

   ```


**sorted() - Returns a new sorted list from the items in an iterable:**
  ```py
numbers = [5, 2, 7, 1, 9]
sorted_numbers = sorted(numbers)
print(sorted_numbers)  # Output: [1, 2, 5, 7, 9]

   ```


**open() - Opens a file and returns a file object:**
  ```py
file = open('sample.txt','r')
content = file.read()
print(content)
file.close()
   ```

**dir() - Returns a list of valid attributes and methods of an object:**
  ```py
my_list = [1, 2, 3]
print(dir(my_list))  # Output: ['append', 'clear', 'copy', 'count', 'extend', 'index', 'insert', 'pop', 'remove', 'reverse', 'sort']
   ```

## Print Format in Python

 **String Interpolation / f-Strings or string literals:**
  ```py
a = 3, b= 5
print(f"{a} + {b} is {a+b}")
   ```


 **New Style String Formatting (str.format):**
  ```py
a = 3
b= 5
print("The sum of {} + {} is {}".format(a,b,a+b))
print('{} / {} = {:.2f}'.format(a, b, a / b)) # limits it to two digits 
   ```


## Strings and its methods in Python

 **Unpacking Characters:**
  ```py
language =  'Python'
a,b,c,d,e,f  = language
print(a)
print(b)
print(c)
print(d)
print(e)
print(f)
   ```

 **Accessing Characters in Strings by Index:**
  ```py
language =  'Python'
print(language[0])
print(language[1])
   ```

 **Accessing Characters in Strings by Index:**
  ```py
language =  'Python'
print(language[0])
print(language[1])
   ```

 **Accessing Characters in Strings by Index:**
  ```py
language =  'Python'
print(language[0])
print(language[1])
   ```

 **Accessing Characters in Strings by Index:**
  ```py
language =  'Python'
print(language[0])
print(language[1])

# accessing last index
lastIndex = len(language)-1
print(language[lastIndex])

# other way to access last index
last_index = language[-1]
print(last_index)

# accessing second last index
second_last_index = language[-2]
print(second_last_index)
   ```

 **Strings Slice into substrings:**
  ```py
language = 'Python'
first_three = language[0:3] # starts at zero index and up to 3 but not include 3
print(first_three) #Pyt
last_three = language[-3:]
print(last_three) #hon
print(language[:-1]) #Pytho
   ```


 **Slicing with a step:**
  ```py
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
even_numbers = numbers[1:10:2]  # Starts at index 1, ends at index 10, step of 2
print(even_numbers)  # Output: [2, 4, 6, 8, 10]

# odd numbers from list
odd_numbers = numbers[0:10:2]
print(odd_numbers)
   ```


 **Slicing to copy a list:**
  ```py
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
copy_numbers = numbers[:]  
print(copy_numbers)  
   ```


 **Slicing strings with negative indices:**
  ```py
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
my_string = "Hello, World!"
sub_string = my_string[-6:-1]  # Slices from the 6th last character up to the 1st last character
print(sub_string)  # Output: World
   ```

 **Slicing with omitted start or end indices:**
  ```py
numbers = [1, 2, 3, 4, 5]
sliced_numbers = numbers[:3]  # Starts from the beginning and ends at index 3 (exclusive)
print(sliced_numbers)  # Output: [1, 2, 3]

sliced_numbers = numbers[2:]  # Starts from index 2 and goes till the end
print(sliced_numbers)  # Output: [3, 4, 5]
   ```

 **Reverse number with negative index:**
  ```py
numbers = [1, 2, 3, 4, 5]
reversed_numbers = numbers[::-1]  # Reverses the order of the list
print(reversed_numbers)  # Output: [5, 4, 3, 2, 1]
   ```
 **Reverse string with negative index:**
  ```py
my_string = "Hello, World!"
resversed_string = my_string[::-1] 
print(resversed_string)
   ```


 **isalnum() method is a built-in string method in Python that checks whether all the characters in a string are alphanumeric (consists of letters and numbers):**
  ```py
string1 = "Hello123"
string2 = "Hello, World!"

print(string1.isalnum())  # Output: True (all characters are alphanumeric)
print(string2.isalnum())  # Output: False (comma and space are non-alphanumeric characters)
   ```


 **isalpha() Checks if all string elements are alphabet characters (a-z and A-Z):**
  ```py
string1 = "Hello"
string2 = "123"

print(string1.isalpha())  
print(string2.isalpha()) 
   ```


 **isidentifier(): Checks for a valid identifier - it checks if a string is a valid variable name:**
  ```py
string1 = "Hello"
string2 = "123Hello"

print(string1.isidentifier())   # True
print(string2.isidentifier())   # False bcz it starts with 123
   ```

 **islower(): Checks if all alphabet characters in the string are lowercase:**
  ```py
string1 = "hello"
string2 = "Hello"

print(string1.islower())   # True
print(string2.islower())   # False
   ```

 **isupper(): Checks if all alphabet characters in the string are uppercase:**
  ```py
string1 = "hello"
string2 = "HELLO"

print(string1.isupper())   # False
print(string2.isupper())   # True
   ```

 **join(): Returns a concatenated string:**
  ```py
web_tech = ['HTML', 'CSS', 'JavaScript', 'React']
result = ' '.join(web_tech)
print(result) # 'HTML CSS JavaScript React'
   ```


 **Different string method:**
  ```py

  # replace(): Replaces substring with a given string
  string1 = 'I love mang'
  replaced_string = string1.replace('man','mangoes')
  print(replaced_string)

  # count(): returns occurrences of substring in string
my_string = "Hello, World"
print(my_string.count('o'))

# endswith(): Checks if a string ends with a specified ending
print(my_string.endswith('ld')) # true
print(my_string.endswith('od')) # false

# find(): Returns the index of the first occurrence of a substring, if not found returns -1
challenge = 'thirty days of python'
print(challenge.find('y'))  # 5
print(challenge.find('th')) # 0


# split(): Splits the string, using given string or space as a separator
web_tech = 'HTML CSS JS REACTJS NEXJS NODEJS'
print(web_tech.split())

# startswith(): Checks if String Starts with the Specified String
web_tech = 'HTML CSS JS REACTJS NEXJS NODEJS'
print(web_tech.startswith('HTML'))  #True
print(web_tech.startswith('CSS'))  #False
   ```



### Lists in Python

 **Accessing List Items Using Positive Indexing:**
  ```py
fruits = ['banana', 'orange', 'mango', 'lemon']
first_fruit = fruits[0] # we are accessing the first item using its index
print(first_fruit)      # banana
second_fruit = fruits[1]
print(second_fruit)     # orange

# Last index
last_index = len(fruits) - 1
last_fruit = fruits[last_index]
   ```

 **Accessing List Items Using Positive Indexing:**
  ```py
fruits = ['banana', 'orange', 'mango', 'lemon']
first_fruit = fruits[0] # we are accessing the first item using its index
print(first_fruit)      # banana
second_fruit = fruits[1]
print(second_fruit)     # orange

# Last index
last_index = len(fruits) - 1
last_fruit = fruits[last_index]
   ```



 **Accessing List Items Using Negative Indexing:**
  ```py
fruits = ['banana', 'orange', 'mango', 'lemon']
first_fruit = fruits[-4]
last_fruit = fruits[-1]
second_last = fruits[-2]
print(first_fruit)      # banana
print(last_fruit)       # lemon
print(second_last)      # mango
   ```



 **Unpacking List Items:**
  ```py
fruits = ['banana', 'orange', 'mango', 'lemon', 'peach', 'watermelon','apple']
first_item, second_item, *rest = fruits
print(first_item)
print(second_item)
print(rest)
   ```



 **Slicing Items from a List:**
  ```py
fruits = ['banana', 'orange', 'mango', 'lemon', 'peach', 'watermelon']
print(fruits[0:]) # copy list
print(fruits[0:4])
print(fruits[:2])  # ['banana', 'orange']
print(fruits[1:])  # ['orange', 'mango', 'lemon', 'peach', 'watermelon']
print(fruits[::2]) #every 2nd element from list
print(fruits[::3]) #every 3rd element from list


# negative indexing
fruits = ['banana', 'orange', 'mango', 'lemon']
all_fruits = fruits[-4:] # it returns all the fruits
orange_and_mango = fruits[-3:-1] # it does not include the last index,['orange', 'mango']
orange_mango_lemon = fruits[-3:] # this will give starting from -3 to the end,['orange', 'mango', 'lemon']
reverse_fruits = fruits[::-1] # a negative step will take the list in reverse order,['lemon', 'mango', 'orange', 'banana']
   ```

 **Modifying Lists:**
 *List is a mutable or modifiable ordered collection of items. Lets modify the fruit list.*
  ```py
fruits = ['banana', 'orange', 'mango', 'lemon']
fruits[0] = 'avocado'
print(fruits)       #  ['avocado', 'orange', 'mango', 'lemon']
fruits[1] = 'apple'
print(fruits)       #  ['avocado', 'apple', 'mango', 'lemon']
last_index = len(fruits) - 1
fruits[last_index] = 'lime'
print(fruits)        #  ['avocado', 'apple', 'mango', 'lime']
   ```

 **Checking Items in a List:**
 *Checking an item if it is a member of a list using *in* operator.*
  ```py
fruits = ['banana', 'orange', 'mango', 'lemon']
does_exist_01 = 'banana' in fruits 
print(does_exist_01) # True
does_exist_02 = 'mango' in fruits 
print(does_exist_02)  # True
does_not_exits = 'apple' in fruits
print(does_not_exits)  # False
   ```


 **Adding Items to a List:**
  ```py

 # using append 
fruits = ['banana', 'orange', 'mango', 'lemon']
fruits.append('apple')
print(fruits)           # ['banana', 'orange', 'mango', 'lemon', 'apple']
   

  # The insert() fruits = ['banana', 'orange', 'mango', 'lemon']
fruits.insert(2, 'apple') # insert apple between orange and mango
print(fruits)           # ['banana', 'orange', 'apple', 'mango', 'lemon']
fruits.insert(3, 'lime')   # ['banana', 'orange', 'apple', 'lime', 'mango', 'lemon']
print(fruits)methods takes two arguments:index and an item to insert.
   ```


 **Removing Items from a List:**
  ```py
  
  # using remove() method
fruits = ['banana', 'orange', 'mango', 'lemon', 'banana']
fruits.remove('banana')
print(fruits)  # ['orange', 'mango', 'lemon', 'banana'] - this method removes the first occurrence of the item in the list
fruits.remove('lemon')
print(fruits)  # ['orange', 'mango', 'banana']

# using pop() method
fruits = ['banana', 'orange', 'mango', 'lemon']
fruits.pop()
print(fruits)       # ['banana', 'orange', 'mango']
fruits.pop(0)
print(fruits)       # ['orange', 'mango']


# using del keyword, it removes the specified index.
fruits = ['banana', 'orange', 'mango', 'lemon', 'kiwi', 'lime']
del fruits[0]
print(fruits)       # ['orange', 'mango', 'lemon', 'kiwi', 'lime']
del fruits[1]
print(fruits)       # ['orange', 'lemon', 'kiwi', 'lime']

web_tech = ['HTML', 'CSS', 'JS', 'NextJS', 'ReactJS', 'Nodejs']
del web_tech[1:4] # ['HTML', 'ReactJS', 'Nodejs']
# del web_tech[:-1] # return last item
# del web_tech[-1:] #remove last item
print(web_tech)

# clear() remove all elements
web_tech.clear()
print(web_tech)
   ```


 **Copying a List:**
  ```py
fruits = ['banana', 'orange', 'mango', 'lemon']
fruits_copy = fruits.copy()
print(fruits_copy)       # ['banana', 'orange', 'mango', 'lemon']
   ```


 **Joining Lists:**
 *There are several ways to join, or concatenate, two or more lists in Python.*
  ```py
language =  'Python'
print(language[0])
print(language[1])
   ```

