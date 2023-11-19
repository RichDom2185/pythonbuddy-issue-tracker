# Python Buddy Issue Tracker

[Python Buddy](https://learn.richarddominick.me/python/) is a tool to help you learn coding in Python. It explains how to read and better understand Python code in a step-by-step fashion.

This repository is for tracking issues and feature requests for Python Buddy.

## Features and Roadmap

- [x] Step-by-step explanations of Python code
- [x] Code highlighting
- [x] Code editing
- [x] Sharable links
- [ ] Code execution visualization

## Supported Python Features

I'm actively working on supporting more and more features of the language, with the goal of covering the necessary features for basic Python learning first. Here's what's currently supported, as well as the features I'm working on next:

### Basic Features

- [x] Variable assignment: `a = 1`
- [x] Multiple assignment: `a, b = 1, 2`
- [ ] Starred assignment: `a, *b, c = 1, 2, 3, 4`
- [ ] Assignment expressions: `a := 1`
- [x] Operators: `+`, `-`, `*`, `/`, `//`, `%`, `**`
- [x] Comparisons: `==`, `!=`, `>`, `<`, `>=`, `<=`, `in`, `not in`, `is`, `is not`
- [x] Operator assignment: `+=`, `-=`, `*=`, `/=`, `//=`, `%=`, `**=`
- [x] Boolean operators, with short-circuiting: `and`, `or`
- [x] Unary operators: `+3`, `-3`, `not 3`

### Collections of Data 1

- [x] Lists, tuples, and dictionaries: `my_list = [1, 2, 3]`
- [x] Indexing: `my_list[0]`
- [x] Slicing: `my_list[0:2]`
- [x] Extended slicing: `my_list[0:2:2]`

### Control Flow

- [x] Ternary operator: `a if b else c`
- [x] If statements: `if`, `elif`, `else`
- [x] While loops: `while True`
- [x] For loops: `for x in my_list:`
- [ ] Non-standard control flow: `break` and `continue` statements

### Collections of Data 2

- [x] List comprehensions: `[x for x in my_list]`
- [ ] Dictionary comprehensions: `{x: x for x in my_list}`
- [ ] Set comprehensions: `{x for x in my_list}`
- [ ] Generator expressions: `(x for x in my_list)`
- [ ] Nested comprehensions: `[x, y for x in my_list for y in my_list]`

### Functions

- [x] Function definitions: `def my_func(a, b, c):`
- [x] Function calls: `my_func(a, b, c)`
- [ ] Keyword arguments: `my_func(a=1, b=2, c=3)`
- [ ] Early `return` statements
- [x] Attribute/method access: `my_list.append(1)`
- [ ] Lambda expressions: `lambda x: x + 1`

### Others

- [x] Import statements: `import numpy as np`

## Sample Programs

- [List comprehensions vs. For loops](https://share.richarddominick.me/listcomp_vs_for)
- [List indexing and slicing](https://share.richarddominick.me/list_demo)
- [Zoo ticket pricing function](https://share.richarddominick.me/zoo_ticket)
- [Short-circuiting boolean operators](https://share.richarddominick.me/short_circuit)
- [Get all Fibonacci numbers up to a certain number](https://share.richarddominick.me/fib_n)

## Caveats

Caveats describe how Python Buddy's implementation intentionally differs from the official Python language specification.

Any differences not described here should be considered bugs. Please [open an issue](https://github.com/RichDom2185/pythonbuddy-issue-tracker/issues/new) if you find one!

### Assignments

Python Buddy does not support assignment expressions (also known as the "walrus operator") yet.

Until it does so, normal assignments and multiple assignments are value-producing (unlike standard Python). In the case of the latter, a tuple is produced.

This does not mean they can be used as expressions, though, as that would violate python syntax.

### For loops

The iterator of the for loop is evaluated all at once. This is **not meant to be permanent**, and simply a workaround due to time constraints. Until this is fixed, Python Buddy will not be able to support early return, break, or continue statements.

Implication: If your iterator has side effects, they will be evaluated first before the body of the for loop is even executed once.
