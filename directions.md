# Practice: Try-Except & Lists

## Overview:

- Students will be able to use a user-defined function to remove items from a Python list
- Students will use a `try-except` block to handle index errors that might occur when working with the list

## Submitting Your Work:

> Save your files to a GitHub repo named: ***manage-list-with-function***

## Sample Output
![Sample output](output.png)

## Resources:

- [Python index ( ) method](https://www.w3schools.com/python/trypython.asp?filename=demo_ref_list_index)
- [Handling errors with try/except block in Python](https://python.land/deep-dives/python-try-except#Catching_exceptions_with_try_except)

## Directions

- Add at least six party guests to a Python list named `guests`   

- Define a function named `remove_guest( )` that takes two parameters, `guest_name` and `response`  

- Add a `try` block to the body of your function:

    - In the `try` block, use the Python `index()` method to get the index number of the guest name passed to the function; save this index number to a variable `guest_index`   

    - If the guest responded *no* or *n* in your `try` block, use the `pop()` method to remove the guest from the `guests` list and print a sentence telling the user that guest RSVP'd no and has been removed from the guest list
          - HINT: The Python `in` operator and a list to store the responses **no** and **n** could be helpful here!
          - HINT: What Python string method coverts the user's input to lowercase?
- Now create an `except` block to handle the `ValueError` exception
    - Your `except` block tells Python what to do when a guest name is not found in your list
    - In your `except` block, use an **f-string** and the `print()` function to tell the user the guest was not found in the `guests` list
 

- Outside your `remove_guest( )` function, call the `remove_guest()` function three times
    - As arguments, use the name of a guest and his/her response to the invitation
    - Example: `remove_guest('Mike', 'No')`
    - Example: `remove_guest('Alyssa', 'Yes')`
- Print the updated guest list at the end of your script
