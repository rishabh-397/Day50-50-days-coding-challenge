# Day50-50-days-coding-challenge

## Problem Statement:
Given a palindromic string `palindrome`, replace exactly **one character** with any lowercase English letter such that the new string:
- Is **not a palindrome**
- Is **lexicographically smallest**

Return the resulting string.  
If no such operation is possible, return `""`.

---

## 🔍 Example:

**Input:**  
palindrome = "abccba"

**Output:**  
"aaccba"  
Explanation: Changing the first 'b' to 'a' makes it no longer a palindrome and is lexicographically smallest.

**Input:**  
palindrome = "a"

**Output:**  
""  
Explanation: No way to break a single-character palindrome.

---

## 🚀 Approach:
1. Traverse from the start to the middle of the string.
2. If any character is not `'a'`, change it to `'a'` to reduce lexicographical value and break symmetry.
3. If all characters are `'a'`, change the **last character** to `'b'`.
4. If the string has **length 1**, return `""`.

---

## ✅ Time & Space Complexity:
- **Time:** O(n), where n is the length of the string
- **Space:** O(n) for the new string (or O(1) if modified in-place)
