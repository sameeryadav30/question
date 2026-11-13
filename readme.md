# 9. Palindrome Number

<sub>LeetCode | Easy | Math</sub>

## 📌 Problem Statement

Given an integer `x`, return `true` if `x` is a palindrome, and `false` otherwise.

A **palindrome number** is a number that reads the same from left to right and right to left.

**Problem Link:** [LeetCode – Palindrome Number](https://leetcode.com/problems/palindrome-number/)

## 💡 Examples

**Example 1**

```text
Input: x = 121
Output: true
Explanation: 121 reads the same in both directions.
```

**Example 2**

```text
Input: x = -121
Output: false
Explanation: Reversed number becomes 121-.
```

**Example 3**

```text
Input: x = 10
Output: false
Explanation: Reversed number becomes 01.
```

## ⚙️ Constraints

```text
-2³¹ <= x <= 2³¹ - 1
```

## 🧠 Approach: Reverse the Number

Instead of converting the integer into a string, reverse the number mathematically.

### Algorithm

1. If the number is negative, return `false`.
2. Store the original number.
3. Initialize `reverse = 0`.
4. Extract the last digit using `% 10`.
5. Add the digit to the reversed number.
6. Remove the last digit using `/ 10`.
7. Repeat until the number becomes zero.
8. Compare the reversed number with the original number.


```

## 🔍 Dry Run

**Input:** `x = 121`

| Iteration | Digit | Reverse |
|---|---:|---:|
| 1 | 1 | 1 |
| 2 | 2 | 12 |
| 3 | 1 | 121 |

Final comparison:

```text
Original = 121
Reverse  = 121

121 == 121 → true
```

## 📚 Important Concepts

| Operator | Purpose |
|---|---|
| `% 10` | Extract last digit |
| `/ 10` | Remove last digit |
| `reverse * 10 + digit` | Build reversed number |
| `==` | Compare two numbers |

## ⏱️ Complexity Analysis

- **Time Complexity:** `O(log₁₀ n)` — Each iteration removes one digit.
- **Space Complexity:** `O(1)` — Uses a constant amount of extra memory.

## 🎯 Learning Outcome

- Understanding number manipulation.
- Using modulo and division operators.
- Implementing loops.
- Building a reversed integer.
- Understanding time and space complexity.

## 📊 Problem Information

| Property | Details |
|---|---|
| Problem Number | 9 |
| Problem Name | Palindrome Number |
| Platform | LeetCode |
| Difficulty | Easy |
| Topic | Math |
| Language | java |
| Approach | Mathematical Reversal |
| Status | Solved |

---

**Keep Learning. Keep Solving. 🚀**