# Two Sum (LeetCode 1)

🔗 [Problem Link](https://leetcode.com/problems/two-sum/)

---

## 📝 Problem Statement
Given an array of integers `nums` and an integer `target`, return the indices of the two numbers such that they add up to `target`.  
You may assume that each input would have exactly one solution, and you may not use the same element twice.

---

## 💡 Approach
- Use a **hash map** (`unordered_map`) to store visited numbers and their indices.  
- For each number, calculate the complement (`target - nums[i]`).  
- If the complement already exists in the map → return indices.  
- Otherwise, add the current number to the map.  

---

## ⏱️ Complexity
- **Time Complexity**: O(n)  
  (Each element is checked once, and lookup in a hash map is O(1) on average).  
- **Space Complexity**: O(n)  
  (Hash map stores up to `n` elements in the worst case).  

---

## ✅ Example
**Input**: nums = [2,7,11,15], target = 9  
**Output**: [0,1]  
(Explanation: nums[0] + nums[1] = 2 + 7 = 9)

