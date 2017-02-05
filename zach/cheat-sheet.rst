Python Cheat Sheet
==================

**Comments**

.. code-block:: python

    # This is a comment. Python will ignore this line.

**Printing**

.. code-block:: python

    print("Hello, world")

**Variable assignment**

.. code-block:: python

    # Reference must be on the left of the equals sign.
     a = 2
     b = "Hello, World!"
     c = 1.5

**Standard data-types**

- ``int`` : integer (no decimal).
- ``float`` : decimal number
- ``str`` : string of characters (between quotations)
- ``bool`` : boolean type. ``True`` or ``False`` in python (notice capitalization).
- ``list`` : container for multiple python elements. Anything can be


**Operators**

- ``+`` : addition
- ``-`` : subtraction
- ``*`` : multiplication
- ``/`` : division
- ``**`` : power
- ``%`` : modulo (remainder from the division)
- ``+=`` : add to value
- ``-=`` : subtract from value
- ``*=`` : multiple to value
- ``/=`` : divide from value

Sequences
---------

**Standard data-structures**

* ``list`` : an ordered, mutable container for a sequence of elements.
* ``tuple`` : an ordered, immutable container for a sequence of elements.
* ``set`` : an unordered, mutable container for a set of unique elements.

.. code-block:: python

    # example list
    >>> x = [2,2,3,3]
    [2, 2, 3, 3]

    # example tuple
    >>> y = (2,2,3,3)
    (2, 2, 3, 3)

    # example set
    >>> z = {2,2,4,4}
    {2,4}

**Indexing/slicing**

Index a sequence using bracket notation.

.. code-block:: python

    >>> x = [1,2,3,4]
    >>> # Index a sequence
    >>> x[2]
    3

    >>> # Slice a sequence
    >>> x[1:3]
    [2, 3]

    >>> # Reverse index
    >>> x[-1]
    4

    # Nested lists
    >>> y = [[0, 1], [2, 3]]
    >>> y[0][0]
    2

Actions
-------

**Conditions**

.. code-block:: python

    # If this statement is True ...
    if x > 10:
        # Execute this code.
        print("x is greater than 10.")
    # If the first condition failed, but this one is True...
    elif x <= 5:
        # Execute this code.
        print("x is less than or equal to 5.")
    # If all the conditions failed above,
    else:
        # Execute this code.
        print("x is between 5 and 10.")

**For-loops**

A for-loop repeats a chunk of a code a fixed/defined number of times.

*example 2*

.. code-block:: python

    # A simple example of a for-loop
    >>> for i in range(3):
    >>>     print(i)

    0
    1
    2


*example 1*

.. code-block:: python

    # Initialize a list
    >>> squares = []
    >>> for i in range(10):
    >>>     val = i ** 2
    >>>     squares.append(val)
    >>>
    >>> print(squares)

    [0, 1, 4, 9, 16, 25, 36, 49, 64, 81, 100]

**While-loops**

A while-loop repeats a chunk of a code until a condition is met.

.. code-block:: python

    >>> i = 0
    >>> while i < 3:
    >>>    print (i)
    >>>    i += 1

    0
    1
    2

Common errors/exceptions
------------------------

Name errors
~~~~~~~~~~~

.. code-block:: python

    >>> x

    NameError: name 'x' is not defined

*possible causes*

1. ``x`` has not beed defined yet. Need to set ``x``.
2. ``x`` is defined outside of the current scope.

Syntax errors
~~~~~~~~~~~~~

.. code-block:: python

    >>> for i in range(10)
    >>>     pass

    SyntaxError: invalid syntax

*possible causes*

Check your colons at the end of the line!! This is true for conditions, functions
loops, etc.
