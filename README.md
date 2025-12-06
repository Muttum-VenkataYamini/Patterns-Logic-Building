# Patterns-Logic-Building

# 🧠 Patterns & Logic Building  
A collection of core problem-solving patterns used in Data Structures & Algorithms.  
This repository focuses on writing **clean, optimized, pattern-based solutions**.

---

## 🔶 1. Sliding Window

The **Sliding Window** technique is widely used with **arrays** and **strings**, especially when dealing with **consecutive elements**, **subarrays**, or **substrings**.

---

### 🔍 What is a “Window”?

A window is simply a frame that captures part of the array/string.

Example:  
Array: `[1, 2, 3, 4, 5]` (Window size = 3)  
Goal: Find the **maximum sum** of 3 consecutive elements.

- **Brute Force:** Recalculate all subarrays → ❌ Slow  
- **Sliding Window:** Move the window efficiently → ✔️ Fast

Window 1: [1, 2, 3] → sum = 6
Slide → remove 1, add 4
Window 2: [2, 3, 4] → sum = 9
Slide → remove 2, add 5
Window 3: [3, 4, 5] → sum = 12


✨ **Key Idea:**  
Only update the sum by removing the left element and adding the new right element.

---

### 🧩 Types of Sliding Window

#### 1️⃣ **Fixed Size Window**
Window length stays constant.  
Example: "Max sum of window size K".

#### 2️⃣ **Variable Size Window**
Window expands or shrinks based on a condition.  
Example: "Smallest subarray with sum ≥ target".

---

### 🧠 When to Use Sliding Window?

Look for hints like:

- “consecutive elements”
- “subarray / substring”
- “longest / shortest”
- “must contain unique characters”
- “sum ≥ target”

These almost always indicate Sliding Window.

---

### ⭐ Popular LeetCode Problems

- **#3** – Longest Substring Without Repeating Characters  
- **#209** – Minimum Size Subarray Sum  
- **#239** – Sliding Window Maximum  

---

### ⚡ Pros

- **Time:** O(n)  
- **Space:** O(1) or O(k)

### ⚠️ Cons

- Must handle **fixed vs variable size** carefully  
- Watch out for edge cases (e.g., empty array, k > n)

---

