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


