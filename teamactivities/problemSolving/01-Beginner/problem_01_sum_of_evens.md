# Beginner Problem 1: Sum of Even Numbers

## Difficulty Level
Beginner

## Problem Description
Write a function that takes a list of integers and returns the sum of all even numbers in the list.

## Constraints
- List length: 1 to 1000
- Numbers range: -1000 to 1000
- No external libraries required

## Input/Output Format
### Input
A list of integers: `[int, int, ..., int]`

### Output
An integer representing the sum of even numbers

## Examples

### Example 1
**Input:** `[1, 2, 3, 4, 5, 6]`  
**Output:** `12` (2 + 4 + 6 = 12)

### Example 2
**Input:** `[1, 3, 5, 7]`  
**Output:** `0` (no even numbers)

### Example 3
**Input:** `[-2, 0, 2, 4]`  
**Output:** `4` (-2 + 0 + 2 + 4 = 4)

## Hints
- Remember that 0 is an even number
- Use the modulo operator (%) to check if a number is even
- A number is even if `number % 2 == 0`

## Key Concepts
- Iteration
- Conditional statements
- Modulo operator

## Success Criteria
- [ ] Solution correctly identifies even numbers
- [ ] Handles negative numbers correctly
- [ ] Handles empty list edge case
- [ ] Code is clean and readable

## Discussion Points
- Did you handle negative numbers?
- How would you handle an empty list?
- Can you think of alternative approaches?

---
**Difficulty:** Easy | **Time Estimate:** 5-10 minutes  
**Category:** Basic Logic
