questions.py
-----------

DSL for writing Python quizes in Python

Python Quiz
-----------

TODO

* finish intro questions
  * generators, coroutines
  * objects, classes, methods
  * exceptions, briefly context managers
  * imports
  * dir, help, __doc__, __file__, 

* command line interactive quiz

* render each type of question differently
  * add necessary attributes and methods for display to questions

* server-size render logic

* Do quizes for rest of Python Essential Reference book

* make a "being careful" quiz, with questions from https://alexbers.com/python_quiz/

* annotate quesitons with answers, make them better for learning

* make a quiz based on questions people ask when reading code (like bpython)


references:

* http://docs.python-guide.org/en/latest/ - contribute something to it!
* http://stackoverflow.com/questions/101268/hidden-features-of-python
* Raymond Hettinger Idiomatic Python https://www.youtube.com/watch?v=OSGv2VnC0go


Could just make this the quiz companion to 
The Python Essential Reference 4th edition
(but will need to check that this is ok with ddabeaz if I crib anything more)

other:

how to make multiple expression lambdas?

how to run Python code directly from the command line?

how to exit a program despite having non-daemon threads running? (os._exit())

draw out an object graph (OPT-style) of something complicated

what python statements have else clauses

other useful builtin iterators from Ned's talk: os.path



I think you should know a lot of this stuff within a month of learning Python,
but maybe longer if Python is your first programming language


Following the outline of Python Essential reference:
====================================================

Everything in the next section:  you should know it!

cursory introduction

Tutorial Introduction
---------------------

If you're going to use Python for just one project

draw some object graphs with lists #TODO come back to this, need image

build a structure from a drawing

''.split()

# File containing lines of the form "name,shares,price"
filename = "portfolio.csv"
portfolio = []
for line in open(filename):
    fields = line.split(",") # Split each line into a list
    name = fields[0] # Extract and convert individual fields
    shares = int(fields[1])
    price = float(fields[2])
    stock = (name,shares,price) # Create a tuple (name, shares, price)
    portfolio.append(stock)

tuple unpacking

invoke arguments using names of args

modify global variables in functions

generators - the yield keyword
they have "next"
this works in for loops

how would you write `tail`?

How would you write grep?

tail grep

Coroutines - generators that take data
syntax for this
choose a use case example

write one

objects and classes

list methods etc. with dir

know what type with type

know the + -> __add__ correspondence

write a method

staticmethods



Exceptions

with file

with lock

why are these useful for exceptions?


all the different imports

dir again

help(obj)

.__doc__

pydoc command line tool






