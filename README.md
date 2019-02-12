# learningPython
#### Purpose of this repo: notes on learning Python
##### Source: [https://campus.datacamp.com/courses/intro-to-python-for-data-science](https://campus.datacamp.com/courses/intro-to-python-for-data-science)

## Basics
* assigning variables: x = 1
* types of data:
  - float = numbers with decimals
  - integers (int) = numbers without decimals
  - string (str) = character strings, manipulate using "" or ''
  - boolean (bool) = True/False (capitalize 1st letter)
* operators:
  - +, -, /, *
  - exponent: **
  - modulus: %
  - _operators behave differently on different data types, e.g. "+" will paste strings and add numbers_
* converting data types: use functions str(), bool(), int(), float() to convert to that type

## Lists
* create list: use square brackets
* create list of lists: use nested square brackets

## Indexing & subsetting
* __zero-based indexing__: 1st element is element 0
* use listName & square brackets to access list element
* to count index numbers backwards from end of list, use negative index numbers (last = -1)
* select multiple elements to create new list ("slice"): use colon for index numbers, start:end
  - __NOTE__: the "start" index is included, but the "end" is not included in the slice. e.g. 2:5 means element 2, 3, 4
  - __REMEMBER THOUGH...__: ELEMENTS BEGIN AT 0!
* select multiple including beginning or end: a blank number in slice specifies beginning or end of list

## Modifying lists
* modify an element by specifying its index then assigning new value using =
* add a new list element using +
  - you do _not_ have to re-assign the modified list to a variable, this updates the existing variable automatically
* delete element by position using del()
  - this also updates the existing variable automatically
  
## Copying lists
* if you assign list x to a new variably y using '=', then any changes to y will also change x! 
  - this is because of the way python stores lists as a reference to the list, not the list itself
* to _copy_ the list so that x and y are no longer interconnected, use: y = list(x) or y = x\[:]
