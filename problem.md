# Problem.md — Pseudocode for Lab 03 Problems

## Problem 1: Display Student Information Using Different Data Types

```
START
    DECLARE name AS character array
    DECLARE rollNo AS integer
    DECLARE age AS integer
    DECLARE height AS float
    DECLARE gpa AS float
    DECLARE section AS character

    PROMPT and READ name
    PROMPT and READ rollNo
    PROMPT and READ age
    PROMPT and READ height
    PROMPT and READ gpa
    PROMPT and READ section

    PRINT "STUDENT INFORMATION"
    PRINT name, rollNo, age, height, gpa, section
STOP
```

## Problem 2: Read and Display a Character Using getchar() and putchar()

```
START
    DECLARE ch AS character

    PRINT "Enter a character: "
    ch = getchar()

    PRINT "You entered: "
    putchar(ch)
STOP
```

## Problem 3: Display a Floating-Point Value Using Different Precision Settings

```
START
    DECLARE value AS float

    PROMPT and READ value

    PRINT value with default precision
    PRINT value with 2 digits after decimal
    PRINT value with 4 digits after decimal
    PRINT value with 6 digits after decimal
STOP
```
