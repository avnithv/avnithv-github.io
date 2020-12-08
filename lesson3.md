# Mutable vs. Immutable
There are two types of datatypes: mutable, and immutable. These determine what properties the datatype may have and how you can manipulate it. 

What is the difference? 

The short answer is that mutable data is changeable while immutable data is not. The actual reason why is because of how the data is stored by the computer. Data is assigned to an ID which corresponds to a place in the computer's memory. Immutable data is assigned an ID that changes after each operation. In other words, it is assigned an new place in the memory each time it is changed. This means you have to assign it to a new variable or reassign it to the same variable after each operation. Mutable datatypes are always stored in the same spot in the memory and the same variable. After an operation, the changes are made to the data itself, and there is no need to reassign it. 

It is important to know which datatypes are immutable and which are mutable. Ints, floats, strings, and boolean data are all immutable. Lists and Dictionaries, which we will learn about in this chapter, are mutable.

# Lists

## What are lists?
Lists are ways to store a lot of data in one variable. They are an ordered and mutable sequence of values. These values can be any data; ints, floats, strings, boolean, even other lists. Lists are similar to strings in the way that they are stored. Lists are stored as a sequence of individual values, not as a whole, like strings are stored as a sequence of characters and not one whole string. Each item inside of a list is accessed the same way as strings, starting from zero and increasing moving right, or starting at -1 and decreasing moving left. The only difference is that list can contain any item, while strings can only contain single characters. Also, lists are mutable while strings are not.

Lists are defined by a pair of square brackets around it with each item inside separated by a comma, similar to string being defined by a pair of quotes around it.

## Creating and Changing Lists
There are three main ways to create lists:
- `list(iterable)` constructor: Changes a string into a list of characters or any number of arguments into a list. **Example:** `list('Hello')` gives `['H', 'e', 'l', 'l', 'o']` and `list(1, 2, 3)` gives `[1, 2, 3]`
- Directly with `[]` and`,`: Like other datatypes we have previously learned, lists can be directly assigned to a variable. You have to use the form discussed with square brackets and commas
- Using the `split(string)` method: Splits a string into a list of substrings that do not overlap whenever a substring appears. For example, splitting a sentence with the substring `' '`, which is the default value, will return a list of words because each word is separated by a space.

The two most common ways that lists are created in practice are the second and third ways. The second is for lists made by the progammer and the third is more for processing the input into a list.

There are two ways to add items to a list:
- `list.append(item)` method: Adds an item to the back of a list
- `list.insert(index, item) method: Adds item into list such that the item is in the `index`th index.

Append is used more because you want to add an item to the end of a list most of the time. Insert is used less.

There are two ways to remove items from a list:
- `del list[start:stop:step]` with **del** keyword: Removes item at an index or all items in a slice.
- `list.pop(index)` method: Remove item at index as well as returning its value.

## Operations with lists
Here are some of the most common operations with lists:
- Slice - `list[start:stop:step]` - Similar to strings, it returns a sublist starting with the item at index `start` ending with the item before the one at `stop`, and by every `step` items.
- Change an item's value - `list[index] = new_value` - Directly changes an item's value
- Sort the list - `list.sort()` - Sorts the list into ascending order. Works only with ints, floats, and strings, and orders string based on **ASCII** values.
- Reverse the list order - `list.reverse() ` - Reverses the order of the list so that the last item is now first, and vice versa.
- Find length of list - `len(list)` - Returns the length of the list
- Find if item is in list - `if item in list` - **if** and **in** are keywords, and this returns `True` if the item is in the list.
- Find how many times an item appears in a list - `list.count(item)` - Returns the number of times an item appears in a list.

In a list of all ints or floats:
- Find sum of all items in list - `sum(list)` - Returns the sum of all items in list
- Find maximum/minimum of the items in the list - `max(list)`/`min(list)` - Returns the maximum/minimum item in list.
