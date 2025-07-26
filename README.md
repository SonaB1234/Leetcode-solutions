# 🚀 LeetCode Python Solutions

This repository contains my personal solutions to various [LeetCode](https://leetcode.com) problems written in **Python**. All code is clean, readable, and intended for learning, practice, and interview preparation.

---

## 📌 Why This Repo?

- 📖 To track my DSA progress
- 💻 To showcase problem-solving skills
- 🧠 For revision before interviews
- ✨ Clean and optimized Python code

---

## 📁 Structure

Each problem is saved as a `.py` file named after the problem title or number. Code is tested on LeetCode and follows standard conventions.

---

## ✅ Sample File

```python
# two_sum.py
class Solution:
    def twoSum(self, nums, target):
        hashmap = {}
        for i, num in enumerate(nums):
            diff = target - num
            if diff in hashmap:
                return [hashmap[diff], i]
            hashmap[num] = i
