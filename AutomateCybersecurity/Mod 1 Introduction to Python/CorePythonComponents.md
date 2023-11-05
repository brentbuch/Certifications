# Core Python Components

## Data Types in Python

Data Type - Category for particular type of data

<u>String</u> - data containing an ordered sequence of characters. Can contain letters, numbers, special characters, etc. Numbers in a string cannot be used for calculations. All characters must be enclosed by quotation marks. 

<u>Float</u> - numeric data containing a decimal point. Fractions and whole numbers included. 

<u>Integer</u> - numeric data without a decimal point. 

<u>Boolean</u> - data that can only be true or false.

```py
print(10>5)
```

<u>List</u> - data structure that contains collection of data in sequential order.

```py
# Print a list
print(["mary", "helen", "mark"])
```
### More data type information

- strings can be enclosed in single or double quotations. It is best to choose one or the other and stay consistent.
- lists are contained in brackets and items are separated by commas
- integers are not placed in quotes
- print can be used to run mathematical equations. ex. print(1+5)
- floats are also not placed in quotes
- dividing two integers or floats will result in a float
- to return the whole number from a calculation use '//' This will round down the answer to the nearest whole number

### Additional data types

<u>Tuple</u> - data structure that consists of a collection of data that cannot be changed. Like lists, tuples can contain elements of varying data types. Data is placed inside parenthesis. They are more memory efficient than lists.

```
(hard, soft, bite)
```

<u>Dictionary</u> - data that consists of one or more key-value pairs. Each key is mapped to a value. A colon (:) is placed between the key and value. Commas separate key-value pairs from other key-value pairs, and the dictionary is placed within curly brackets. Useful to store and retrieve data in a predictable way.

```
{ 1: "East",

  2: "West",

  3: "North",

  4: "South" }
  ```

<u>Set</u> - an unordered collection of unique values. No two values can be the same. Sets are placed in curly brackets, and elements are separated by a comma. The elements can be of any data type. 

```
{"harry", "david", "mark"}
```

## Working with variables in Python

- creating a variable is called 'assigning'

```py
# Use a variable to store device id
device_id = "h34dd4"
```

- using a variable is called 'calling.' Using a variable inside a print statement does not require parenthesis, even if the variable contains a string value. 


```py
# Use a variable to store device id
device_id = "h34dd4"

# calling a variable
print(device_id)
```

### The 'type' function

The type function returns the type of data inside a variable. 

```py
# Use a variable to store device id
device_id = "h34dd4"

# using the type function
data_type = type(device_id)
print(data_type)
```

<u>Type Error</u> - an error returned when using an incorrect data type

### Reassignment

The data contained in a variable can be changed at any time. This is called 'reassignment.' Variables can even be reassinged to a different data type.

```py
# Use a variable to store device id
device_id = "h34dd4"

# calling a variable
print(device_id)

# reassign the variable
device_id = "ja364r"
print(device_id)
```

### Best practices for variables

- use only letters, numbers and underscores for variable names
- start name with a letter, not a number
- variables are case sensitive. EX. hat and Hat are two different variables
- don't use Python's built in keywords or functions for variable names. EX. TRUE, FALSE, if
- separate words with underscores
- avoid using simalar names for different variables
- don't use excessively long names
- variable names should describe the data they contain and not random words

