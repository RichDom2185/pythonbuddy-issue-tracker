# Python Buddy Issue Tracker

[Python Buddy](https:/pythonbuddy.dev/) is a tool to help you learn coding in Python. It explains how to read and better understand Python code in a step-by-step fashion.

This repository is for tracking issues and feature requests for Python Buddy.

## Features and Roadmap

- [x] Step-by-step, textual explanations of Python code
- [x] Code highlighting
- [x] Code editing
- [x] Sharable links
- [x] Import external modules (see [below](#available-modules))
- [ ] Code execution visualization

## Available Modules

| Type        | Name                                                                | Description                                                                       |
|-------------|---------------------------------------------------------------------|-----------------------------------------------------------------------------------|
| Built-in    | [`collections`](https://docs.python.org/3/library/collections.html) | High-performance container datatypes                                              |
| Built-in    | [`functools`](https://docs.python.org/3/library/functools.html)     | Higher-order functions and operations on callable objects                         |
| Built-in    | [`math`](https://docs.python.org/3/library/math.html)               | Mathematical functions                                                            |
| Third-party | [`numpy`](https://numpy.org/doc/stable/)                            | Scientific computing with Python                                                  |
| Third-party | [`pandas`](https://pandas.pydata.org/docs/)                         | Data analysis and manipulation tool                                               |
| Custom      | (WIP) `cs1010s_runes`                                               | CS1010S-specific functions for rendering runes – ported to work with Python Buddy |

Want more modules? File a [feature request here.](https://github.com/RichDom2185/pythonbuddy-issue-tracker/issues)

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
- [ ] `del` keyword: `del a`

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
- [x] For loops with multiple targets: `for x, y in zip(my_list, reversed(my_list)):`
- [x] Else (normal exit) clauses: `for...else` and `while...else` loops
- [x] Non-standard control flow: `break` and `continue` statements

### Collections of Data 2

- [x] List comprehensions: `[x for x in my_list]`
- [x] Nested list comprehensions: `[x, y for x in my_list for y in my_list]`
- [x] Dictionary comprehensions: `{x: x for x in my_list}`
- [x] Set comprehensions: `{x for x in my_list}`
- [ ] Generator expressions: `(x for x in my_list)`

### Functions

- [x] Function definitions: `def my_func(a, b, c):`
- [x] Function calls: `my_func(a, b, c)`
- [x] Keyword arguments: `my_func(a=1, b=2, c=3)`
- [ ] Positional-only arguments: `def my_func(a, b, c, /)`
- [ ] Keyword-only arguments: `def my_func(*, a, b, c)`
- [x] Early `return` statements
- [ ] Generator `yield` statements
- [x] Attribute/method access: `my_list.append(1)`
- [x] Lambda expressions: `lambda x: x + 1`

### Object-Oriented Programming

- [x] _(BETA)_ Class definitions: `class MyClass:`
- [x] _(BETA)_ Instance attributes: `self.my_attr = 1`
- [ ] Class attributes: `class MyClass: my_attr = 1`
- [x] _(BETA)_ Instance methods: `class MyClass: def my_method(self):`
- [ ] Class methods: `class MyClass: @classmethod def my_method(cls):`
- [ ] Static methods: `class MyClass: @staticmethod def my_method():`
- [ ] Inheritance: `class MyClass(MyParentClass):`
- [ ] Multiple inheritance: `class MyClass(MyParentClass1, MyParentClass2):`

### Others

- [x] Import statements: `import numpy as np`
- [x] Import from statements: `from numpy import array`
- [x] Wildcard import statements: `from numpy import *`
- [ ] f-strings: `f'Hello, {name}!'`

## Sample Programs

- [Simple factorial function](https://pythonbuddy.dev/editor/?code=ZGVmIGZhY3RvcmlhbChuKToKICAgIHJldHVybiBuIGlmIG4gPD0gMSBlbHNlIG4gKiBmYWN0b3JpYWwobi0xKQoKcHJpbnQoZmFjdG9yaWFsKDMpKQ==&filename=factorial.py)
- [List comprehensions vs. For loops](https://pythonbuddy.dev/editor/?code=aSA9IDEwCmEgPSBbaSBmb3IgaSBpbiByYW5nZSg1KV0KaSAgIyAxMApwcmludChhLCBpKQoKaiA9IDEwCmIgPSBbXQpmb3IgaiBpbiByYW5nZSg1KToKICAgICBiLmFwcGVuZChqKQpqICAjIDQKcHJpbnQoYiwgaikKCmEgPT0gYiAgIyBUcnVlCg==&filename=listcomp_vs_for.py)
- [List indexing and slicing](https://pythonbuddy.dev/editor/?code=YSA9IFsyLCAzLCA0XQppID0gMQoKcHJpbnQoYVswXSkgICAgICAjIDIKcHJpbnQoYVtpXSkgICAgICAjIDMKcHJpbnQoYVtpICsgMV0pICAjIDQKCnByaW50KGFbMDoyXSkgICAgIyBbMiwgM10KcHJpbnQoYVtpOl0pICAgICAjIFszLCA0XQpwcmludChhWzotMV0pICAgICMgWzIsIDNdCgpwcmludChhWzo6Ml0pICAgICMgWzIsIDRdCnByaW50KGFbOjotMV0pICAgIyBbNCwgMywgMl0=&filename=list_index_slice.py)
- [Zoo ticket pricing function](https://pythonbuddy.dev/editor/?code=YWdlID0gWzExLCAzNiwgMzcsIDY3XSAgIyBsaXN0IG9mIGFnZXMgb2YgdmlzaXRvcnMgCgpkZWYgem9vX3RpY2tldChhZ2UpOgogICAgIiIiVGhlIGZ1bmN0aW9uIHpvb190aWNrZXQgY2FsY3VsYXRlcyB0aGUgCiAgICBTaW5nYXBvcmUgWm9vIHRpY2tldCBwcmljZXMgZm9yIHZpc2l0b3JzIiIiCgogICAgaWYgYWdlIDwgMzoKICAgICAgICB0aWNrZXQgPSAwCiAgICBlbGlmIGFnZSA8PSAxMjoKICAgICAgICB0aWNrZXQgPSAyOAogICAgZWxpZiBhZ2UgPCA2MDoKICAgICAgICB0aWNrZXQgPSA0MQogICAgZWxzZToKICAgICAgICB0aWNrZXQgPSAxOAoKICAgIHJldHVybiB0aWNrZXQKCiMgY3JlYXRlIGxpc3QgZm9yIHByaWNlcyBvZiB0aWNrZXRzCnRpY2tldCA9IFtdCmZvciBpdGVtIGluIGFnZToKICAgIHRpY2tldC5hcHBlbmQoem9vX3RpY2tldChpdGVtKSkKCnRpY2tldAo=&filename=zoo_ticket.py)
- [Short-circuiting boolean operators](https://pythonbuddy.dev/editor/?code=ZGVmIGdldF90cnVlKCk6CiAgICBwcmludCgnVHJ1ZScpCiAgICByZXR1cm4gVHJ1ZQoKZGVmIGdldF9mYWxzZSgpOgogICAgcHJpbnQoJ0ZhbHNlJykKICAgIHJldHVybiBGYWxzZQoKIyBTaG9ydC1jaXJjdWl0aW5nIGZvciBgYW5kYAphID0gZ2V0X3RydWUoKSBhbmQgZ2V0X3RydWUoKSBhbmQgZ2V0X2ZhbHNlKCkgYW5kIGdldF90cnVlKCkgYW5kIGdldF90cnVlKCkKcHJpbnQoKQoKIyBTaG9ydC1jaXJjdWl0aW5nIGZvciBgb3JgCm8gPSBnZXRfZmFsc2UoKSBvciBnZXRfdHJ1ZSgpIG9yIGdldF90cnVlKCkgb3IgZ2V0X3RydWUoKSBvciBnZXRfZmFsc2UoKQpwcmludCgp&filename=short_circuit.py)
- [Get all Fibonacci numbers up to a certain number](https://pythonbuddy.dev/editor/?code=IyBQcmludCBhbGwgRmlib25hY2NpIG51bWJlcnMgYmVsb3cgbgpkZWYgZmliKG4pOgogICAgYSwgYiA9IDAsIDEKICAgIHdoaWxlIGEgPCBuOgogICAgICAgIHByaW50KGEsIGVuZD0nICcpCiAgICAgICAgYSwgYiA9IGIsIGEgKyBiCiAgICBwcmludCgpCmZpYigyMDAwKQo=&filename=fib_n.py)
- [Rendering pandas DataFrames and intermediates](https://pythonbuddy.dev/editor/?code=aW1wb3J0IG51bXB5IGFzIG5wCmltcG9ydCBwYW5kYXMgYXMgcGQKCmRmID0gcGQuRGF0YUZyYW1lKFsKICAgIHsnYSc6IDI1LCAnYic6IDQ5LCAnYyc6IDEwMH0sCiAgICB7J2EnOiBucC5uYW4sICdiJzogODEsICdjJzogMTIxfSwKXSkKCiMgSW50ZXJtZWRpYXRlIGRhdGFmcmFtZXMgYXJlIHNob3duIQpjb2xfbWFwID0gezI1OiAnaGknLCA0OTogJ2Zyb20nLCAxMDA6ICdQeXRob24gQnVkZHkhJ30KcHJpbnQoZGYuZHJvcG5hKCkudHJhbnNwb3NlKClbMF0ubWFwKGNvbF9tYXApKQ==&filename=pandas.py)
- [Library and Book (OOP) Example](https://pythonbuddy.dev/editor/?code=Y2xhc3MgQm9vazoKICAgIGRlZiBfX2luaXRfXyhzZWxmLCB0aXRsZSwgYXV0aG9yKToKICAgICAgICBzZWxmLnRpdGxlID0gdGl0bGUKICAgICAgICBzZWxmLmF1dGhvciA9IGF1dGhvcgoKICAgIGRlZiBkaXNwbGF5X2luZm8oc2VsZik6CiAgICAgICAgcHJpbnQoIkJvb2sgVGl0bGU6IHt9Ii5mb3JtYXQoc2VsZi50aXRsZSkpCiAgICAgICAgcHJpbnQoIkF1dGhvcjoge30iLmZvcm1hdChzZWxmLmF1dGhvcikpCiAgICAgICAgcHJpbnQoIi0tLS0tLS0tLS0tLS0tLS0tLS0tIikKCgpjbGFzcyBMaWJyYXJ5OgogICAgZGVmIF9faW5pdF9fKHNlbGYpOgogICAgICAgIHNlbGYuYm9va3MgPSBbXQoKICAgIGRlZiBhZGRfYm9vayhzZWxmLCBib29rKToKICAgICAgICBzZWxmLmJvb2tzLmFwcGVuZChib29rKQogICAgICAgIHByaW50KCJCb29rIGFkZGVkIHRvIHRoZSBsaWJyYXJ5LiIpCgogICAgZGVmIGRpc3BsYXlfYm9va3Moc2VsZik6CiAgICAgICAgaWYgbm90IHNlbGYuYm9va3M6CiAgICAgICAgICAgIHByaW50KCJUaGUgbGlicmFyeSBpcyBlbXB0eS4iKQogICAgICAgIGVsc2U6CiAgICAgICAgICAgIHByaW50KCJMaWJyYXJ5IEJvb2tzOiIpCiAgICAgICAgICAgIGZvciBib29rIGluIHNlbGYuYm9va3M6CiAgICAgICAgICAgICAgICBib29rLmRpc3BsYXlfaW5mbygpCgojIEV4YW1wbGUgdXNhZ2UKYm9vazEgPSBCb29rKCJUaGUgQ2F0Y2hlciBpbiB0aGUgUnllIiwgIkouRC4gU2FsaW5nZXIiKQpib29rMiA9IEJvb2soIlRvIEtpbGwgYSBNb2NraW5nYmlyZCIsICJIYXJwZXIgTGVlIikKYm9vazMgPSBCb29rKCIxOTg0IiwgIkdlb3JnZSBPcndlbGwiKQoKbGlicmFyeSA9IExpYnJhcnkoKQpsaWJyYXJ5LmFkZF9ib29rKGJvb2sxKQpsaWJyYXJ5LmFkZF9ib29rKGJvb2syKQpsaWJyYXJ5LmFkZF9ib29rKGJvb2szKQoKbGlicmFyeS5kaXNwbGF5X2Jvb2tzKCkK&filename=library.py)
- [CS1010S runes demo](https://pythonbuddy.dev/editor/?code=ZnJvbSBjczEwMTBzX3J1bmVzIGltcG9ydCAqCgpkZWYgY3ljbGVyKG4pOgogICAgUEFUVEVSTiA9IFsKICAgICAgICBwZW50YWdyYW1fYmIsCiAgICAgICAgc3BpcmFsX2JiLAogICAgICAgIHJjcm9zc19iYiwKICAgICAgICBoZWFydF9iYiwKICAgIF0KICAgIGluZGV4ID0gMAogICAgcm93cyA9IFtdCiAgICBmb3IgXyBpbiByYW5nZShuKToKICAgICAgICByID0gYmxhbmtfYmIKICAgICAgICBmb3IgaSBpbiByYW5nZShuKToKICAgICAgICAgICAgciA9IGJlc2lkZV9mcmFjKGkvKGkgKyAxKSwgciwgUEFUVEVSTltpbmRleF0pCiAgICAgICAgICAgIGluZGV4ID0gKGluZGV4ICsgMSkgJSBsZW4oUEFUVEVSTikKICAgICAgICByb3dzLmFwcGVuZChyKQogICAgciA9IGJsYW5rX2JiCiAgICBmb3IgaSBpbiByYW5nZShsZW4ocm93cykpOgogICAgICAgIHJvdyA9IHJvd3NbaV0KICAgICAgICByID0gc3RhY2tfZnJhYyhpLyhpICsgMSksIHIsIHJvdykKICAgIHJldHVybiByCgpjeWNsZXIoNCk=&filename=runes.py)
- [_That CS1010E question_](https://pythonbuddy.dev/editor/?code=IyBUaGUgbGFtYmRhIGlzIG5ldmVyIGNhbGxlZCwgc28gYGlgIGlzIGp1c3QgYSBuYW1lCmxmID0gW2xhbWJkYSB4OngraSBmb3IgaSBpbiByYW5nZSgwLCAxMCwgMildCnByaW50KGxmWzNdKDcpKQoKIyBJZiB5b3Ugd2FudCwgeW91IHNob3VsZCBjYXB0dXJlIGl0IHZpYSBjbG9zdXJlCmxmID0gWyhsYW1iZGEgaTogbGFtYmRhIHg6eCtpKShpKSBmb3IgaSBpbiByYW5nZSgwLCAxMCwgMildCnByaW50KGxmWzNdKDcpKQo=&filename=the_1010e_question.py)

_Note: CS1010\_ refer to the codes of some courses offered by the National University of Singapore._

## Caveats

Caveats describe how Python Buddy's implementation intentionally differs from the official Python language specification.

Any differences not described here should be considered bugs. Please [open an issue](https://github.com/RichDom2185/pythonbuddy-issue-tracker/issues/new) if you find one!

### Assignments

Python Buddy does not support assignment expressions (also known as the "walrus operator") yet.

Until it does so, normal assignments and multiple assignments are value-producing (unlike standard Python). In the case of the latter, a tuple is produced.

This does not mean they can be used as expressions, though, as that would violate python syntax.

### For loops

The iterator of the for loop is evaluated all at once and coerced to a list. This is **not meant to be permanent**, and simply a workaround due to lack of support for generator expressions for now. As a consequence, there may be some edge cases involving early return, break, or continue statements wher Python Buddy gives an incorrect result.

Implication: If your iterator has side effects, they will be evaluated first before the body of the for loop is even executed once.
