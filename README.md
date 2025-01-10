# Kotlin Collection removeIf() Gotcha

This repository demonstrates a subtle issue related to using the `removeIf()` function on collections in Kotlin.  Modifying a collection while iterating can produce unexpected results. This example highlights the differences between how `removeIf()` affects `MutableList`, `MutableSet`, and `MutableMap`. The solution provides a safer alternative.

## Problem
The `removeIf()` function, when used incorrectly, can skip elements or lead to inaccurate results due to the modification of the collection structure while iterating.

## Solution
The suggested solution demonstrates the safest way to remove elements from a collection based on a condition, preventing the problems associated with modifying during iteration.