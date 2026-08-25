# ECE-2112-PA-1
Made by: Erin Madeline M. Sumeguin | 2-ECEB

# A. Word Rotation Problem
Create a function named rotate word() that accepts a non-empty string. 
Move the first character of the string to the end while keeping all remaining characters in their original order. 
Preserve the capitalization of every character.

Function Format: rotate_word(text)

Slicing was also used to specify which element shall be moved and not. In this problem, slicing was used to return the second until the last characters in the text and then concatenated it with a plus (+) symbol to combine it with the first character at the end.

```python
def rotate_word(text): 
    return text[1:] + text[0]
```

# B. Username Builder Problem
Create a function named make_username() that accepts two strings first_name and last_name.

The function must:
1. convert all letters to lowercase;
2. remove all spaces from the first name;
3. remove all spaces from the last name; and
4. join the processed first and last names using one period (.).

Function format: make_username(first_name, last_name)
Requirement: Use basic string methods and string concatenation. Return the completed username.

The functions used in this problem are the following:
- **`.lower()`** - converts all letters in a string to lowercase.
- **`.replace( , )`** - replaces a certain element from the string. 
- **`+`** - used for string concatenation, combines multiple strings into one string.

```python
def make_username(first_name, last_name): 
    first_name = first_name.lower() 
    first_name = first_name.replace(" ", "") 
    
    last_name = last_name.lower() 
    last_name = last_name.replace(" ", "") 
    
    return first_name + "." + last_name
```

# C. Bookend Swap Problem
Create a function named swap_bookends() that accepts a list containing at least two elements. Unpack the list into three variables:

- first - the first element;
- middle - a list containing everything between first and last elements; and
- last - the last element

Using these variables, return a new list in which the first and last elements have exchanged positions. The elements in the middle must remain in their original order. 

Function format: swap_bookends(items)

```python
def swap_bookends(items): 
    first, *middle, last = items 
    return [last] + middle + [first]
```

Thank you for reading!

To see the main python program for Programming Assignment 1, click this link https://github.com/stroberin/ECE-2112-PA-1/blob/main/Programming%20Assignment%201.ipynb and download. Open on Jupyter Notebook, then run all cells.

**README file Version History:**
- August 23, 2026 - Initial README output uploaded.

- August 23, 2025 - Format in README content was updated.

- August 25, 2026 - More format tweaks in README content.
