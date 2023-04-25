--- 
title: Learn Python in 30 minutes. Part 2 - Strings.
date: 2022-10-19 12:25:00 +100
categories: [python, learn-in-30-minutes]
tags: [python, learning, tutorial, programming-language]
mermaid: true
---

## Step 5: Learn how to create and merge Strings

##### Creating Strings

- The text data in Python is called **String**.
- The official name of this data type is denoted as **"str"** 
  ```python
    str()
  ```
- You have to surround a text data by single or double **quotes**
    ```python
    'text'
    "text"
    ```
- Use triple quotes to create a multiline string
    ```python
    '''
    text
    '''
    ```

##### Merging String 

There are three most common ways to merge strings in modern Python:
- We can use "+" sign to merge or **concatenate** two or more strings into one bigger:
```python
string_variable = "string" + " data"
print(string_variable)
```

> There is a whitespace in front of the second string to separate two words.
{: .prompt-warning }

- With format function, the order is important:
```python
greet = 'hello'
eng = 'engineer'
message = '{} {}'.format(greet,  eng)
print(message)
```

- With f-string interpolation ( the most common modern approach, available starting python 3.6).
```python
greet = 'hello'
eng = 'engineer'
message = f'{greet} {eng}'
print(message)
```
> Note there is a letter f sitting right before the quote.
{: .prompt-warning }

#### Exercise

- Create a variable with name "fist_name" and assign your first name to it.
- Create a variable with name "second_name" and assign your family name to it.
- Create three more variables: "full_name1", "full_name2", "full_name3" and use the three methods above to create string which would hold your first and last names together.
- Print the variables on the terminal.

## Step 6: Learn how to modify strings

Before exploring how we can modify strings, we need to learn a bit of a theory.

##### About objects

- The strings are the **objects** in Python.
- An object stores a **data**.
- An object has its own **functions** which can do changes on its data.
- To access a function of an object we use dot "." after a variable or an object itself:

  ```python
  variable_name.function()
  object.function()
  ```
- A function can **return** something. This means it gives **result** data.
- You can also think about the result as an **output**.
- You can access a result in two ways:
  - Create a new variable and assign the result data to it

    ```python
    new_variable = old_variable.function_which_returns_something()
    ```
  - Pass the result data directly into a function

    ```python
    function(old_variable.function_which_returns_something())
    ```

> Below I'm going to show examples of getting results of string functions with both approaches.
{: .prompt-tip }

> We need to remember that the string functions don't modify the original string, instead they **return** a new string. That is because strings are **immutable** objects.  
{: .prompt-info }

##### upper() - Convert lowercase string to uppercase:

Create a new variable and assign the result data to it:
```python
message = 'hello world'
upper_message = message.upper()
print(upper_message)
```

Pass the result data directly into a function:
```python
message = 'hello world'
print(message.upper())
```

##### lower() - Convert uppercase string to lowercase:
Create a new variable and assign the result data to it:
```python
message = 'HELLO WORLD'
lower_message = message.lower()
print(lower_message)
```

Pass the result data directly into a function:
```python
message = 'HELLO WORLD'
print(message.lower())
```

##### count() - Count amount of characters or even words

```python
message = 'hello world'
print(message.count('l'))	
print(message.count('hello'))
```

##### replace() - Replace character by another character

```python
message = 'hello world'
print(message.replace('world', 'engineer'))
```

#### Exercise

- Create a variable with name "fist_name" and assign your first name to it.
- Create a variable with name "second_name" and assign your family name to it.
- Create three more variables: "full_name1", "full_name2", "full_name3" and use the three methods above to create string which would hold your first and last names together.
- Print the variables on the terminal.
