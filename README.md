# ECE-2112-PA-1
Made by: Erin Madeline M. Sumeguin | 2-ECEB

# A. Word Rotation Problem
Create a function named rotate word() that accepts a non-empty string. 
Move the first character of the string to the end while keeping all remaining characters in their original order. 
Preserve the capitalization of every character.

Function Format: rotate_word(text)

def rotate_word(text): #defines rotate_word() as a function.
    return text[1:] + text[0] #returns the second element up until the last element and then adds the first element.


