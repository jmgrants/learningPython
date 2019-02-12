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
* modify an element by specifying its index then assigning new value using '='
* add a new list element using +
  - you do _not_ have to re-assign the modified list to a variable, this updates the existing variable automatically
  - to add multiple elements, you can use a second list (square brackets), and the result will _still_ be a single list
* delete element by position using del()
  - this also updates the existing variable automatically
  
## Copying lists
* if you assign list x to a new variably y using '=', then any changes to y will also change x! 
  - this is because of the way python stores lists as a reference to the list, not the list itself
* to _copy_ the list so that x and y are no longer interconnected, use: y = list(x) or y = x\[:]

## Multiple commands on same line
* separate with ;
  - runs them sequentially, not piping I believe

## Functions
* accessing documentation on functions: help(functionName) ...OR ?functionName if using IPython
  - optional arguments are surrounded by square brackets, and default value is given in description
* list of functions covered in intro:
  - max(), len(), sorted(), print(), etc.

## Methods
* specific functions that are used on specific data types (objects)
* to call the method, use __dot notation__: combine variable name with method name using a dot
  - e.g. for list "fam", to use the index("elementName") method, you write: fam.index("elementName")
* _list_ methods examples
  - listName.index()
  - listName.count()
* _str_ methods examples
  - strName.capitalize()
* objects with different types can have methods by the same name, e.g. listName.index("elementName") works on lists to bring up the index name, but strName.index("c") works on strings to bring up the character position in the string
* some methods change the object they are called on (automatically), e.g. listName.append("new") will modify the list

## Packages
* popular packages for data science:
  - Numpy ('NUM-pie'): working with arrays
  - Matplotlib: visualizations
  - Scikit-learn: machine learning
* to install packages:
  - use pip: package maintenance system
  - Structure: pip3 install _packageName_
* to load packages for use:
  - Structure: import _packageName_ as _pn_ (the 'as' statement gives you a nickname to call the functions from that package)
* calling package functions:
  - Strucutre: np.array() where 'np' is the nickname you gave the package (numpy) and array is a function from the package (numpy)
* to import specific function from a package:
  - Structure: from _packageName_ import _functionName_
  - then you _don't_ have to call the function using packageName.functionName() notation, just the function name will do

## NumPy & arrays
* NumPy: numeric python
* arrays: similar to vectors in R (array/array calculates element-wise)
  - can only contain 1 type of data, so mixed types will be converted all to strings
  - note that "+" will behave differently for lists (+ is like paste) vs arrays (+ is an operator, and each element will be added to corresponding element in 2nd array)
  - subsetting works similarly to lists
  - OR can use an array of booleans (i.e. logical subsetting)
    - e.g. bmi[bmi>23]

## 2D numpy arrays
* to make a 2d array, create an array of lists: np.array(\[1, 2, 3], \[1, 2, 3])
* subsetting: np_2d\[r,c]
  - recall that to get all rows or columns, you'd replace it by ':'
  - remember that indexes are 0-based!
