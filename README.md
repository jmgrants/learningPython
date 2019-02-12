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
* select multiple including beginning or end: a blank number in slice specifies beginning or end of list
