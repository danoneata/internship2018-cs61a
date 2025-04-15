TODO

- [x] Create Slack channel
- [x] Post resources on the Slack channel
- [x] Fetch SICP book
- [x] Prepare PDFs to print
- [x] Print notes from CS61A website
- [.] Fetch adapter from office?
- [.] Print my notes

---

Title: Python programming
Author: Dan Oneață

xkcd Python comic
https://xkcd.com/353/

---

- Install Python3
- Install a terminal
- Install a text editor

- Once you're done:

    python3
    >>> import antigravity

---

Goals

- Familiarize with Python
- Concepts of programming

> Peter Norvig
> Teach Yourself Programming in Ten Years
> http://norvig.com/21-days.html

- Q How many of you have some experience with Python: wrote more than 100 lines of code in it?
- Q How many of you feel comfortable with the concept of recursion?

---

Motivation

- It is a very widely used language, with among the best software platforms for web development, data science, scientific computing, etc.
- It is "batteries included," i.e. a lot of important functionality is included in the standard libraries
- It is an interpreted language, so you can quickly experiment in an interactive shell
- The core language is clean and simple, and presents fewer hurdles to beginners compared with some of the alternatives
- It is one of the most popular languages for introductory college courses, so there are lots of materials out there

- More short-term goals: machine learning in Python

---

Outline

- Follow Berkeley's CS61a course: Structure and Interpretation of Computer Programs
- The successor of the famous book and course from MIT -- the first course on programming for any MIT student
- Originally taught in Scheme

- Lecture 1: Functions
- Lecture 2: Values
- Lecture 3: Objects
- Lecture 4: TBD (maybe scientific programming: matplotlib, numpy, scipy)

- The CS61a course has videos and many exercises
- Automated testing
- We will do a part in class -- I'll will assign some homeworks
- We will check next time in class

---

Introductory explanations

**Interpreter.**
- Denoted by the prompt `>>>`
- The interpreter reads and executes what we type
- To exit: `exit()` or `CTRL-D`

**Expressions.**
- Primitive expressions: integers, float, booleans (other data types – to be covered later)
- Numbers can be combined to form compound expressions using arithmetic operations (`+`, `-`, `*`, `/`, `//`)
```python
-1 - -1
1 / 2 + 1 / 4 + 1 / 8 + 1 / 16
```
- Booleans can be combined using boolean operators: `and`, `or`, `not`
- Combining integers to obtain booleans

**Call expressions.**
- Apply a function to some arguments
```python
max(7.5, 9.5)
pow(2, 100)
max(1, -2, 3, -4)
max(min(1, -2), min(pow(3, 5), -4))
```

**Importing library functions.**
```python
import math
math.sqrt(100)
from math import sqrt
sqrt(100)
from math import sqrt as s
s(100)
```

**Variables.**
- A name bineds to a value
```python
radius = 10
2 * radius
from math import pi
pi * 71 / 223
```
- Names can also be bound to functions
```python
f = max
f
f(2, 3, 4)
```
- Multiple assignments and swapping (all expression on the left are evaluated before any names to the left are bound to those values):
```python
x, y = 3, 4
y, x = x, y
x
y
```

**Defining functions.**
- Statement to define a function:
```python
def <name>(<parameters>):
    return <expression>
```
- Note the indentation and the keywords: `def`, `return`

**Control.**
- If statement
```python
if <expr>:
    <statement>
    <statement>
    ...
elif <expr>:
    <statement>
    <statement>
    ...
else:
    <statement>
    <statement>
    ...
```
- While loop
```python
while <expr>:
    <statement>
    <statement>
    <statement>
    ...
```

**Special topics.**
- Divison
- Functions: indentation, return, print
- Control: Short-circuiting
- Error messages

- ? Special mention: += operator (L1-Q2)
- ? Doc strings (L1-Q3)

---

Resources

---

Use the `--local` flag when running `ok`.

Plan for today

|       | Q  | Name                           | Status | Notes |
|-------|----|--------------------------------|--------|-------|
| Lab 1 | 1  | WWPD: Veritasiness             |        | Booleans |
| Lab 1 | 2  | WWPD: Loops                    |        | While loops |
| Lab 1 | 3  | Repeated                       |        | Higher-order functions; HW: implement it using recursion |
| Lab 1 | 4  | Sum Digits                     |        | Prereqs: while loop; floor; div |
| Lab 1 | 5  | Double Eights                  |        |       |
| Lab 1 | 6  | WWPD: Truthiness               |        | Booleans |
| Lab 1 | 7  | WWPD: What if?                 |        | If statements |
| Lab 1 | 8  | Fix the Bug                    |        | Easy; if statements |
| Lab 1 | 9  | Falling Factorial              |        |       |
| Lab 1 | 10 | Guess Linear                   |        |       |
| Lab 1 | 11 | Guess Binary                   |        |       |
|-------|----|--------------------------------|--------|-------|
| Hw  1 | 1  | A Plus Abs B                   |        | Higher-order functions; might be tricky |
| Hw  1 | 2  | Two of Three                   |        |       |
| Hw  1 | 3  | Largest Factor                 |        |       |
| Hw  1 | 4  | If Function vs Statement       |        | Might be tricky, give it as HW |
| Hw  1 | 5  | Hailstone                      |        |       |
|-------|----|--------------------------------|--------|-------|
| Lab 2 | 1  | WWPD: Lambda the Free          |        | Lambda functions |
| Lab 2 | 2  | WWPD: Higher Order Functions   |        |       |
| Lab 2 | 3  | Lambdas and Currying           |        |       |
| Lab 2 | 4  | Composite Identity Function    |        |       |
| Lab 2 | 5  | Lambda the Environment Diagram |        |       |
| Lab 2 | 6  | Make Adder                     |        |       |
| Lab 2 | 7  | Count van Count                |        |       |
| Lab 2 | 8  | I Heard You Liked Functons...  |        |       |
|-------|----|--------------------------------|--------|-------|
| Hw 2  | 1  | Product                        |        |       |
| Hw 2  | 2  | Make Adder with Lambda         |        |       |
|-------|----|--------------------------------|--------|-------|
| Lab 3 | 1  | AB+C                           |        |       |
| Lab 3 | 2  | GCD                            |        |       |
| Lab 3 | 3  | Hailstone                      |        |       |
| Lab 3 | 4  | Doge                           |        |       |
| Lab 3 | 5  | Palindrome                     |        |       |
| Lab 3 | 6  | Common Misconception (1)       |        |       |
| Lab 3 | 7  | Common Misconception (2)       |        |       |
| Lab 3 | 8  | Is Prime                       |        |       |
| Lab 3 | 9  | Interleaved Sum                |        |       |
| Lab 3 | 10 | Ten-pairs                      |        |       |
|-------|----|--------------------------------|--------|-------|
| Hw  3 | 1  | Has Seven                      |        |       |
| Hw  3 | 2  | Summation                      |        |       |
| Hw  3 | 3  | Accumulate                     |        |       |
| Hw  3 | 4  | Filtered Accumulate            |        |       |
| Hw  3 | 5  | Make Repeater                  |        |       |
| Hw  3 | 6  | Quine                          |        |       |
| Hw  3 | 7  | Church Numerals                |        |       |

---

TODO

- [x] Prepare computer: Remap Caps Lock to Ctrl
- [ ] Prepare computer: Improve Python color scheme

Last episode:

- Values: integers, floats, booleans
- Statements: if, while
- Functions and higher-order functions

Skipped:

- [Python] Function decorators
- [Programming] Recursion

This episode:

- Sequences (lists and strings)
- Dictionaries

Sequences
=========

- Ordered collection of values

## Lists

- Lists
- The `length` function
- Indexing and slicing
- The `in` operator -- testing membership
- The `*` operator

- Exercises: Lab 04 Q1

## Sequence iteration

- Sequence iteration, or `for` loops
- Sequence unpacking, also example in `for` loops
- Ranges; using `for _ in range(n)` to iterate instead of the while loop

- Exercises: Lab 04 Q2-3

## Sequence processing

- List comprehensions – similar to the mathematical notation
- Examples: simple example, filtering example
- General expression: `[<exp> for <name> in <sequence exp> if <filtering exp>]
- Mapping: `[a] -> [a]`
- Aggregation: `[a] -> a` --> examples include built-in functions like `sum`, `min`, `max`
- Exercises: Lab 05 Q4
    - Implement a function `apply_to_all : (a -> a) -> [a] -> [a]`
    - Implement a function `keep_if : (a -> Bool) -> [a] -> [a]`
    - Implement a function `reduce : (a -> a -> a) -> [a] -> a -> a`
    - Define `prod : [a] -> a` in terms of `reduce`.

## Strings

- Single and double quotes
- Operators: `in`, `+`, `\*`
- Multi-line literals

- Exercises: Lab 04 Q6-12

---

- Lab04 Q11-12 (checking for victory + Winning)
- HW05 Q3-9 (interval) (s-ar putea fi utilă secțiunea 2.2 din carte [1])
- Lab04 Q14 (merge)
- Lab04 Q13 (flatten)
- For fun – de urmărit Wat [2]

[1] http://composingprograms.com/pages/22-data-abstraction.html
[2] https://www.destroyallsoftware.com/talks/wat

---

După cum știți prezentarea proiectului de RoDigits s-a amânat pentur miercuri. Ca să balansez un pic munca pentru săptămâna viitoare,  vă dau de acum assignment-ul final, pe care îl vom discuta joi, la ultima întâlnire. Am ales problema *Maps* al cărei scop este de a construi un sistem de recomandare de restaurante:
http://inst.eecs.berkeley.edu/~cs61a/fa17/proj/maps/maps.zip

Proiectul pornește de la o bucată de cod destul de consistentă pe care v-a trebui să o completăm; cred că e un exercițiu bun în a citi înțelege cod scris de alții. Până luni cred că puteți rezolva fără probleme primele două etape: phase 0 și phase 1; pentru phase 2 sunt niște întrebări se referă la dicționare, un concept pe care-l vom discuta marți, deși nu e dificil. Dacă aveți ceva nelămuriri, nu ezitați să întrebați :-)

---

@here Probabil unii dintre voi știți deja de la @Anna, întâlnirea de marți s-a mutat la ora 14:00.

Un mic indiciu pentru temă. Problemele Q13 (flatten) și Q14 (merge) se rezolvă elegant folosind funcții recursive. Nu am vorbit despre funcții recursive, dar definiția este simplă: o funcție recursivă este o funcție care se apelează pe ea însăși. (Poate știți _Easter egg_-ul de la Google: atunci când căutați "recursion", Google vă întreabă "did you mean: recursion" :troll:)

Mai dificil este de scris o funcție recursivă corectă – mie mi-a luat ceva până să mă obișnuiesc cu stilul lor.
Cred că ar trebui să aveți în vedere trei aspecte: _(i)_ puteți presupune că apelul recursiv returnează valoarea corectă; _(ii)_ apelul recursiv trebuie să se facă pe o valoare "mai mică" a intrării; _(iii)_ nu uitați să tratați cazurile de bază.  Mi se pare că ingredientul cheie este punctul (i), pentru că e o presupunere serioasă că funcția deja funcționează corect pentru valori mai mici.

Să luăm un exemplu simplu: să zicem că vrem să scriem o funcție recursivă `sum` care calculează suma primelor `n` numere naturale. Pornim de la premisa că funcția `sum` poate deja calcula suma respectivă (i) și o aplicăm pe o intrare mai mică, `n - 1` (ii); cazul de bază este `n = 0` pentru care trebuie să obținem 0 (iii).  Astfel obținem următoarea implementare:
```
def sum(n):
    return (
        0 if n == 0
        else sum(n - 1) + n)
```
<<<<<<< HEAD

Aceste idei sunt similare cu ce ați întâlnit la matematică când foloseați princpiul inducției matematice.
Și acolo începeați cu un caz de bază `P(0)` și apoi presupuneați că `P(n)` este adevarăt și demonstrați că `P(n + 1)` este adevărat.

Acestă idee este similară cu princpiul inducției întâlnit în demonstrațiile matematice: începem cu un caz de bază `P(0)` și apoi presupunem că `P(n)` este adevarăt ca să demonstrăm că `P(n + 1)` este adevărat.

---

Dictionaries
============

- Mapping correspondence relationships: key-value pairs
- Examples: roman numerals, month to id
- Indexing
- Methods: keys, values, items, get (takes a default argument)
- Constructing dictionaries from list of pairs
- Restrictions: (i) keys are immutable; (ii) only a single value for a given key
- Dictionary comprehensions
- Common uses of dictionaries: invert a dictionary, count words using a dictionary and the defaultdict approach

- Exercises: Lab 05 Q1, Lab 05 Q9-10

Trees
=====

- PyTunes: Lab 05 Q5-8

Homework
========

- Project: Maps

---

Poate ar fi mai ușor de înțeles exemplul de mai sus dacă ați implementa funcția `min`.
**Puzzle 2.** Implementați o funcție `min` care primește două argumente, o listă și o funcție, și returnează acel element al listei pentru care funcția are valoarea minimă.
Dacă lista e goală puteți arunca `AssertionError`.
Puncte bonus pentru o implementare recursivă :-)

---

# Object oriented programming

- Motivation: layer of abstraction and organization

- Classes are a _template_ to create objects of that type
- Objects are _instances_ of the class

- Syntax

```python
class <name>:
    <suite>
```

- Example:

```python
class Human:
    planet = "Earth"

    def __init__(self, name):
        self.name = name

    def talk(self):
        print("Hello")

ann = Human()
ann.talk()
```

- Instance attributes
- Class attributes
- Methods (they ought to get self as the first argument)

- Dot notation: `<expression>.<name>`
- The expression hast to evaluate to a class or instance

- Secretly, we have already worked with objects – in fact, everything is an object in Python!
- For example, lists, strings, numbers, functions:

```python
xs = [1, 2, 3]; xs.append(4)
(3).__add__(5)
```

- We can list all attributes of an instance using `dir`

- Note the methods starting and ending with double under-scores:
  magic methods – they are called when special syntax is performed
  Examples: `__add__`, `__len__`, `__call__`, `__str__`

- The `__init__` method of a class is automatically invoked whenever an object is constructed.
- The `__str__` method is invoked automatically when printing
- The `__repr__` is invoked in an interactive session to display values.

