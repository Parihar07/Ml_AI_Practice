# Intermediate Problem 1: Longest Substring Without Repeating Characters

## Difficulty Level
Intermediate

## Problem Description
Given a string, find the length of the longest substring without repeating characters.

## Constraints
- String length: 0 to 50,000
- Characters: ASCII letters, digits, and symbols
- Case-sensitive (a ≠ A)

## Input/Output Format
### Input
A string `s`

### Output
An integer representing the length of the longest substring without repeating characters

## Examples

### Example 1
**Input:** `"abcabcbb"`  
**Output:** `3` (Substring: "abc")

### Example 2
**Input:** `"bbbbb"`  
**Output:** `1` (Substring: "b")

### Example 3
**Input:** `"pwwkew"`  
**Output:** `3` (Substring: "wke")

### Example 4
**Input:** `""`  
**Output:** `0` (Empty string)

## Hints
- Use a sliding window approach with two pointers
- Maintain a set or dictionary to track characters in current window
- When you encounter a duplicate, move the left pointer

## Key Concepts
- Sliding window technique
- Hash map/dictionary
- Two-pointer approach
- String manipulation

## Success Criteria
- [ ] Handles all test cases correctly
- [ ] Time complexity: O(n) where n is string length
- [ ] Space complexity: O(min(m, n)) where m is character set size
- [ ] Code is readable with comments

## Discussion Points
- Why is sliding window efficient here?
- How does the two-pointer approach help?
- What data structure did you use and why?
- Can you explain your solution to others?

---
**Difficulty:** Medium | **Time Estimate:** 20-30 minutes  
**Category:** Sliding Window, String Manipulation
