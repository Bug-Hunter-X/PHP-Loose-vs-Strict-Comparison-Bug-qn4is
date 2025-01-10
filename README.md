# PHP Loose vs Strict Comparison Bug

This example demonstrates a common error in PHP related to loose vs strict comparison operators.

## The Problem
The code uses loose comparison (`==`) which does type coercion before comparison. This can lead to unexpected results where values of different types are considered equal.  Strict comparison (`===`), on the other hand, checks for both value and type equality. 

## How to reproduce
Run the `bug.php` script to see how loose comparison yields unexpected `true` even when comparing different datatypes (integer and string). 

## Solution
The solution file (`bugSolution.php`) shows how using strict comparison (`===`) resolves the issue and prevents such unexpected behavior. Always prefer strict comparison in PHP to avoid these types of bugs.