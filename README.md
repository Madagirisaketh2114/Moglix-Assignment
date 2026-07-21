# Longest Valid Parentheses

## Language
Java

## Problem Statement

Given a string containing only '(' and ')', return the length of the longest valid (well-formed) parentheses substring.

### Example 1

Input:
(() 

Output:
2

### Example 2

Input:
)()())

Output:
4

### Example 3

Input:
""

Output:
0

## Approach

This solution uses a Stack to store indices of parentheses.

1. Initialize the stack with -1.
2. Push indices of '(' onto the stack.
3. When ')' is encountered:
   - Pop the stack.
   - If the stack becomes empty, push the current index.
   - Otherwise, calculate the length of the current valid substring.
4. Keep track of the maximum valid length.

## Time Complexity

O(n)

## Space Complexity

O(n)

## How to Run

Compile:

```bash
javac LongestValidParentheses.java
```

Run:

```bash
java LongestValidParentheses
```

## Author

Submitted as part of the Moglix Online Shortlisting Round.