# Groovy each() Method Unexpected Null Return

This repository demonstrates a common pitfall in Groovy when using the `each()` method on collections.  Many developers expect `each()` to modify the collection in place and return the modified collection.  However, `each()` in Groovy iterates over the collection and returns `null`.  This example showcases the issue and provides a corrected approach.

## Problem

The Groovy code in `BuggyGroovyEach.groovy` attempts to double each element in a list using `each()`.  The expectation is that the list will be modified and the modified list will be printed. Instead, `null` is printed.

## Solution

The `FixedGroovyEach.groovy` file demonstrates the correct way to achieve the desired result. We use `collect()` to create a new list containing the doubled elements.

## How to run

1. Clone this repository.
2. Navigate to the project directory.
3. Run the Groovy scripts using the Groovy command-line interpreter: `groovy BuggyGroovyEach.groovy` and `groovy FixedGroovyEach.groovy`