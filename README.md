# FAANG / MAANG+ Coding Interview Questions

<div align="center">

  <p><strong>A curated collection of coding, system design, and ML interview questions from top tech companies.</strong><br/>Continuously updated with 2025-2026 interview questions.</p>

  <a href="https://github.com/ombharatiya/FAANG-Coding-Interview-Questions/stargazers">
    <img src="https://img.shields.io/github/stars/ombharatiya/FAANG-Coding-Interview-Questions?style=flat" alt="GitHub stars" />
  </a>
  <a href="https://github.com/ombharatiya/FAANG-Coding-Interview-Questions/network/members">
    <img src="https://img.shields.io/github/forks/ombharatiya/FAANG-Coding-Interview-Questions?style=flat" alt="GitHub forks" />
  </a>
  <a href="https://github.com/ombharatiya/FAANG-Coding-Interview-Questions/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/ombharatiya/FAANG-Coding-Interview-Questions?style=flat" alt="License" />
  </a>
  <a href="https://github.com/ombharatiya/FAANG-Coding-Interview-Questions/commits/main">
    <img src="https://img.shields.io/github/last-commit/ombharatiya/FAANG-Coding-Interview-Questions?style=flat" alt="Last Commit" />
  </a>
  <a href="https://github.com/ombharatiya/FAANG-Coding-Interview-Questions/issues">
    <img src="https://img.shields.io/badge/PRs-welcome-brightgreen?style=flat" alt="PRs Welcome" />
  </a>

</div>

## Essential Resources

**Problem Collections**
- [NeetCode 150 - Essential Problems for FAANG Interviews](./NeetCode-150.md)
- [Blind 75 - The Ultimate Interview Preparation List](./Blind-75.md)
- [Top 75 LeetCode Questions to Crack The Coding Interviews](./TopLeetCodeProblems.md)

**Company-Specific Questions**
- [Latest Interview Questions at FAANG/MAANG+ Companies](./FAANG-Recent-Questions.md)
- [System Design Interview Guide](./SYSTEM_DESIGN_INTERVIEW.md)
- [LeakCode](https://leakcode.dev) - Aggregates 23,000+ real interview questions from 7 sources (LeetCode Discuss, Blind, Glassdoor, 1p3a, Reddit, GeeksForGeeks), searchable by company including all FAANG firms, role (SWE, MLE, PM, EM, Quant), and interview round. Free.

**AI & Machine Learning**
- [LLM Papers Cheatsheet - Essential Research Papers](./LLM_PAPERS_CHEATSHEET.md)
- [Complete ML Interview Preparation Guide](./ML_INTERVIEW_PREP.md)
- [Guide to Building AI Agents](./AGENT_BUILDING_GUIDE.md)

**Programming Resources**
- [Python Resources](./PythonResources.md)

## Table of Contents

**Company Questions**

| SNo. | Company |
| ---- | ------- |
| 1. | [FAANG Must Do Problems](#faang-must-do-problems) |
| 2. | [Google](#google) |
| 3. | [Meta (Facebook)](#meta-facebook) |
| 4. | [Amazon](#amazon) |
| 5. | [Apple](#apple) |
| 6. | [Netflix](#netflix) |
| 7. | [Microsoft](#microsoft) |
| 8. | [LinkedIn](#linkedin) |
| 9. | [OpenAI](#openai) |
| 10. | [Anthropic](#anthropic) |
| 11. | [Palantir](#palantir) |
| 12. | [Databricks](#databricks) |
| 13. | [Flipkart](#flipkart) |

## Quick Start Guide

**Beginner Track** (0-3 months)
- Start with [Blind 75](./Blind-75.md) for fundamentals
- Practice 2-3 problems daily focusing on patterns
- Review [Python Resources](./PythonResources.md) for clean code

**Intermediate Track** (1-6 months)
- Complete [NeetCode 150](./NeetCode-150.md) for comprehensive coverage
- Focus on [Recent FAANG/MAANG Questions](./FAANG-Recent-Questions.md)
- Start [System Design](./SYSTEM_DESIGN_INTERVIEW.md) preparation

**Advanced Track** (Targeting specific roles)
- Review company-specific sections below
- Practice [ML Interview Questions](./ML_INTERVIEW_PREP.md) for ML roles
- Study [AI/LLM Papers](./LLM_PAPERS_CHEATSHEET.md) for AI/research roles

## FAANG Must Do Problems

<details>
<summary>View Problems</summary>

| No. | Problem | Difficulty | Time Complexity | Space Complexity |
| --- | ------- | ---------- | --------------- | ---------------- |
| 1 | [Two Sum](https://leetcode.com/problems/two-sum) | Easy | O(n) | O(n) |
| 2 | [Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters) | Medium | O(n) | O(min(m,n)) |
| 3 | [Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring) | Medium | O(n²) | O(1) |
| 4 | [Container With Most Water](https://leetcode.com/problems/container-with-most-water) | Medium | O(n) | O(1) |
| 5 | [3Sum](https://leetcode.com/problems/3sum) | Medium | O(n²) | O(1) |
| 6 | [Remove Nth Node From End of List](https://leetcode.com/problems/remove-nth-node-from-end-of-list) | Medium | O(n) | O(1) |
| 7 | [Valid Parentheses](https://leetcode.com/problems/valid-parentheses) | Easy | O(n) | O(n) |
| 8 | [Merge Two Sorted Lists](https://leetcode.com/problems/merge-two-sorted-lists) | Easy | O(n+m) | O(1) |
| 9 | [Merge k Sorted Lists](https://leetcode.com/problems/merge-k-sorted-lists) | Hard | O(n log k) | O(1) |
| 10 | [Search in Rotated Sorted Array](https://leetcode.com/problems/search-in-rotated-sorted-array) | Medium | O(log n) | O(1) |
| 11 | [Combination Sum](https://leetcode.com/problems/combination-sum) | Medium | O(2ⁿ) | O(n) |
| 12 | [Rotate Image](https://leetcode.com/problems/rotate-image) | Medium | O(n²) | O(1) |
| 13 | [Group Anagrams](https://leetcode.com/problems/group-anagrams) | Medium | O(n k log k) | O(n k) |
| 14 | [Maximum Subarray](https://leetcode.com/problems/maximum-subarray) | Easy | O(n) | O(1) |
| 15 | [Spiral Matrix](https://leetcode.com/problems/spiral-matrix) | Medium | O(m×n) | O(1) |
| 16 | [Jump Game](https://leetcode.com/problems/jump-game) | Medium | O(n) | O(1) |
| 17 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium | O(n log n) | O(n) |
| 18 | [Insert Interval](https://leetcode.com/problems/insert-interval) | Medium | O(n) | O(n) |
| 19 | [Unique Paths](https://leetcode.com/problems/unique-paths) | Medium | O(m×n) | O(m×n) |
| 20 | [Climbing Stairs](https://leetcode.com/problems/climbing-stairs) | Easy | O(n) | O(1) |
| 21 | [Set Matrix Zeroes](https://leetcode.com/problems/set-matrix-zeroes) | Medium | O(m×n) | O(1) |
| 22 | [Minimum Window Substring](https://leetcode.com/problems/minimum-window-substring) | Hard | O(n) | O(k) |
| 23 | [Word Search](https://leetcode.com/problems/word-search) | Medium | O(m×n×4ᵏ) | O(k) |
| 24 | [Decode Ways](https://leetcode.com/problems/decode-ways) | Medium | O(n) | O(n) |
| 25 | [Validate Binary Search Tree](https://leetcode.com/problems/validate-binary-search-tree) | Medium | O(n) | O(h) |
| 26 | [Same Tree](https://leetcode.com/problems/same-tree) | Easy | O(n) | O(h) |
| 27 | [Binary Tree Level Order Traversal](https://leetcode.com/problems/binary-tree-level-order-traversal) | Medium | O(n) | O(n) |
| 28 | [Maximum Depth of Binary Tree](https://leetcode.com/problems/maximum-depth-of-binary-tree) | Easy | O(n) | O(h) |
| 29 | [Construct Binary Tree from Preorder and Inorder Traversal](https://leetcode.com/problems/construct-binary-tree-from-preorder-and-inorder-traversal) | Medium | O(n) | O(n) |
| 30 | [Best Time to Buy and Sell Stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock) | Easy | O(n) | O(1) |

</details>

## Google

<details>
<summary>View 25 Problems (2025-2026 Most Frequent)</summary>

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Two Sum](https://leetcode.com/problems/two-sum) | Easy | Hash Map / Arrays |
| 2 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium | Graph / DFS |
| 3 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium | Intervals / Sorting |
| 4 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium | Design / Linked List |
| 5 | [Validate Binary Search Tree](https://leetcode.com/problems/validate-binary-search-tree) | Medium | Trees / BST |
| 6 | [Course Schedule II](https://leetcode.com/problems/course-schedule-ii) | Medium | Graph / Topological Sort |
| 7 | [Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters) | Medium | Sliding Window |
| 8 | [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water) | Hard | Two Pointers / Stack |
| 9 | [Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree) | Hard | Trees / Design |
| 10 | [Kth Largest Element in an Array](https://leetcode.com/problems/kth-largest-element-in-an-array) | Medium | Heap / Quickselect |
| 11 | [Median of Two Sorted Arrays](https://leetcode.com/problems/median-of-two-sorted-arrays) | Hard | Binary Search |
| 12 | [Group Anagrams](https://leetcode.com/problems/group-anagrams) | Medium | Hashing / Strings |
| 13 | [Word Ladder](https://leetcode.com/problems/word-ladder) | Hard | BFS / Graphs |
| 14 | [Merge K Sorted Lists](https://leetcode.com/problems/merge-k-sorted-lists) | Hard | Heap / Linked List |
| 15 | [Container With Most Water](https://leetcode.com/problems/container-with-most-water) | Medium | Two Pointers |
| 16 | [Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements) | Medium | Heap / Hashing |
| 17 | [Coin Change](https://leetcode.com/problems/coin-change) | Medium | Dynamic Programming |
| 18 | [Search in Rotated Sorted Array](https://leetcode.com/problems/search-in-rotated-sorted-array) | Medium | Binary Search |
| 19 | [Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self) | Medium | Arrays / Prefix |
| 20 | [Binary Tree Level Order Traversal](https://leetcode.com/problems/binary-tree-level-order-traversal) | Medium | Trees / BFS |
| 21 | [Combination Sum](https://leetcode.com/problems/combination-sum) | Medium | Backtracking |
| 22 | [Edit Distance](https://leetcode.com/problems/edit-distance) | Hard | Dynamic Programming |
| 23 | [Minimum Window Substring](https://leetcode.com/problems/minimum-window-substring) | Hard | Sliding Window |
| 24 | [Implement Trie (Prefix Tree)](https://leetcode.com/problems/implement-trie-prefix-tree) | Medium | Trie |
| 25 | [Accounts Merge](https://leetcode.com/problems/accounts-merge) | Medium | Union-Find |

</details>

## Meta (Facebook)

<details>
<summary>View 25 Problems (2025-2026 Most Frequent)</summary>

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Minimum Remove to Make Valid Parentheses](https://leetcode.com/problems/minimum-remove-to-make-valid-parentheses) | Medium | Stack / String |
| 2 | [Binary Tree Vertical Order Traversal](https://leetcode.com/problems/vertical-order-traversal-of-a-binary-tree) | Medium | Tree / BFS |
| 3 | [Basic Calculator II](https://leetcode.com/problems/basic-calculator-ii) | Medium | Stack / Expression Parsing |
| 4 | [Valid Palindrome II](https://leetcode.com/problems/valid-palindrome-ii) | Easy | Two Pointers / String |
| 5 | [Kth Largest Element in an Array](https://leetcode.com/problems/kth-largest-element-in-an-array) | Medium | Heap / Divide & Conquer |
| 6 | [Lowest Common Ancestor of a Binary Tree](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-tree) | Medium | Tree / DFS |
| 7 | [Random Pick with Weight](https://leetcode.com/problems/random-pick-with-weight) | Medium | Binary Search / Prefix Sum |
| 8 | [Subarray Sum Equals K](https://leetcode.com/problems/subarray-sum-equals-k) | Medium | Array / HashMap / Prefix Sum |
| 9 | [Valid Palindrome](https://leetcode.com/problems/valid-palindrome) | Easy | Two Pointers / String |
| 10 | [Two Sum](https://leetcode.com/problems/two-sum) | Easy | Array / HashMap |
| 11 | [Binary Tree Right Side View](https://leetcode.com/problems/binary-tree-right-side-view) | Medium | Tree / BFS |
| 12 | [Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements) | Medium | Heap / HashMap |
| 13 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium | Array / Sorting |
| 14 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium | Design / HashMap / Linked List |
| 15 | [Clone Graph](https://leetcode.com/problems/clone-graph) | Medium | Graph / BFS / DFS |
| 16 | [Merge k Sorted Lists](https://leetcode.com/problems/merge-k-sorted-lists) | Hard | Linked List / Heap |
| 17 | [Maximum Swap](https://leetcode.com/problems/maximum-swap) | Medium | Math / Greedy |
| 18 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium | Graph / DFS / BFS |
| 19 | [Accounts Merge](https://leetcode.com/problems/accounts-merge) | Medium | Union-Find / Graph |
| 20 | [Diameter of Binary Tree](https://leetcode.com/problems/diameter-of-binary-tree) | Easy | Tree / DFS |
| 21 | [Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self) | Medium | Array / Prefix Sum |
| 22 | [Word Break](https://leetcode.com/problems/word-break) | Medium | Dynamic Programming |
| 23 | [Copy List with Random Pointer](https://leetcode.com/problems/copy-list-with-random-pointer) | Medium | Linked List / Hash Table |
| 24 | [Making a Large Island](https://leetcode.com/problems/making-a-large-island) | Hard | Graph / DFS / Union-Find |
| 25 | [Expression Add Operators](https://leetcode.com/problems/expression-add-operators) | Hard | Backtracking / Math |

</details>

## Amazon

<details>
<summary>View 25 Problems (2025-2026 Most Frequent)</summary>

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Two Sum](https://leetcode.com/problems/two-sum) | Easy | Array / Hash Table |
| 2 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium | Graph / DFS / BFS |
| 3 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium | Design / Hash + Linked List |
| 4 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium | Array / Sorting |
| 5 | [Group Anagrams](https://leetcode.com/problems/group-anagrams) | Medium | Hashing / Strings |
| 6 | [Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements) | Medium | Heap / Hashing |
| 7 | [Task Scheduler](https://leetcode.com/problems/task-scheduler) | Medium | Heap / Greedy |
| 8 | [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water) | Hard | Two Pointers / Stack |
| 9 | [Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self) | Medium | Array / Prefix Sum |
| 10 | [Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters) | Medium | Sliding Window |
| 11 | [Minimum Window Substring](https://leetcode.com/problems/minimum-window-substring) | Hard | Sliding Window |
| 12 | [Kth Largest Element in an Array](https://leetcode.com/problems/kth-largest-element-in-an-array) | Medium | Heap / Quickselect |
| 13 | [Merge k Sorted Lists](https://leetcode.com/problems/merge-k-sorted-lists) | Hard | Heap / Linked List |
| 14 | [Course Schedule](https://leetcode.com/problems/course-schedule) | Medium | Graph / Topological Sort |
| 15 | [Rotting Oranges](https://leetcode.com/problems/rotting-oranges) | Medium | Graph / BFS |
| 16 | [Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree) | Hard | Trees / Design |
| 17 | [Lowest Common Ancestor of a Binary Tree](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-tree) | Medium | Trees / DFS |
| 18 | [Coin Change](https://leetcode.com/problems/coin-change) | Medium | Dynamic Programming |
| 19 | [Best Time to Buy and Sell Stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock) | Easy | Array / DP |
| 20 | [Sliding Window Maximum](https://leetcode.com/problems/sliding-window-maximum) | Hard | Deque / Sliding Window |
| 21 | [Reorganize String](https://leetcode.com/problems/reorganize-string) | Medium | Heap / Greedy |
| 22 | [Insert Delete GetRandom O(1)](https://leetcode.com/problems/insert-delete-getrandom-o1) | Medium | Design / Hash Table |
| 23 | [Decode String](https://leetcode.com/problems/decode-string) | Medium | Stack / Strings |
| 24 | [Koko Eating Bananas](https://leetcode.com/problems/koko-eating-bananas) | Medium | Binary Search |
| 25 | [Largest Rectangle in Histogram](https://leetcode.com/problems/largest-rectangle-in-histogram) | Hard | Monotonic Stack |

</details>

## Apple

<details>
<summary>View 20 Problems (2025-2026 Most Frequent)</summary>

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Two Sum](https://leetcode.com/problems/two-sum) | Easy | Array / Hash Table |
| 2 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium | Design / Hash + Linked List |
| 3 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium | Graph / DFS / BFS |
| 4 | [Reverse Linked List](https://leetcode.com/problems/reverse-linked-list) | Easy | Linked List |
| 5 | [Group Anagrams](https://leetcode.com/problems/group-anagrams) | Medium | String / Hash Table |
| 6 | [Valid Parentheses](https://leetcode.com/problems/valid-parentheses) | Easy | Stack / String |
| 7 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium | Array / Sorting |
| 8 | [Word Break](https://leetcode.com/problems/word-break) | Medium | Dynamic Programming |
| 9 | [Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self) | Medium | Array / Prefix Sum |
| 10 | [Best Time to Buy and Sell Stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock) | Easy | Array / DP |
| 11 | [3Sum](https://leetcode.com/problems/3sum) | Medium | Array / Two Pointers |
| 12 | [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water) | Hard | Two Pointers / Stack |
| 13 | [Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements) | Medium | Heap / Hash Table |
| 14 | [Course Schedule](https://leetcode.com/problems/course-schedule) | Medium | Graph / Topological Sort |
| 15 | [Lowest Common Ancestor of a Binary Tree](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-tree) | Medium | Tree / DFS |
| 16 | [Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree) | Hard | Tree / Design |
| 17 | [Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters) | Medium | Sliding Window |
| 18 | [Median of Two Sorted Arrays](https://leetcode.com/problems/median-of-two-sorted-arrays) | Hard | Binary Search |
| 19 | [Maximum Profit in Job Scheduling](https://leetcode.com/problems/maximum-profit-in-job-scheduling) | Hard | Binary Search / DP |
| 20 | [Bus Routes](https://leetcode.com/problems/bus-routes) | Hard | Graph / BFS |

</details>

## Netflix

<details>
<summary>View 15 Problems (2025-2026 Most Frequent)</summary>

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium | Design / Hash + Linked List |
| 2 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium | Array / Sorting |
| 3 | [Course Schedule II](https://leetcode.com/problems/course-schedule-ii) | Medium | Graph / Topological Sort |
| 4 | [Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements) | Medium | Heap / Hash Table |
| 5 | [Network Delay Time](https://leetcode.com/problems/network-delay-time) | Medium | Graph / Dijkstra |
| 6 | [Daily Temperatures](https://leetcode.com/problems/daily-temperatures) | Medium | Monotonic Stack |
| 7 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium | Graph / DFS / BFS |
| 8 | [Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree) | Hard | Tree / Design |
| 9 | [Find Median from Data Stream](https://leetcode.com/problems/find-median-from-data-stream) | Hard | Heap / Design |
| 10 | [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water) | Hard | Two Pointers / Stack |
| 11 | [Edit Distance](https://leetcode.com/problems/edit-distance) | Medium | Dynamic Programming |
| 12 | [Minimum Window Substring](https://leetcode.com/problems/minimum-window-substring) | Hard | Sliding Window |
| 13 | [Meeting Rooms II](https://leetcode.com/problems/meeting-rooms-ii) | Medium | Intervals / Heap |
| 14 | [Koko Eating Bananas](https://leetcode.com/problems/koko-eating-bananas) | Medium | Binary Search |
| 15 | [Implement Trie (Prefix Tree)](https://leetcode.com/problems/implement-trie-prefix-tree) | Medium | Trie / Design |

</details>

## Microsoft

<details>
<summary>View 20 Problems (2025-2026 Most Frequent)</summary>

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Two Sum](https://leetcode.com/problems/two-sum) | Easy | Array / Hash Table |
| 2 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium | Design / Hash + Linked List |
| 3 | [Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters) | Medium | Sliding Window |
| 4 | [Add Two Numbers](https://leetcode.com/problems/add-two-numbers) | Medium | Linked List / Math |
| 5 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium | Graph / DFS / BFS |
| 6 | [Maximum Subarray](https://leetcode.com/problems/maximum-subarray) | Medium | Array / DP |
| 7 | [Merge Two Sorted Lists](https://leetcode.com/problems/merge-two-sorted-lists) | Easy | Linked List |
| 8 | [Copy List with Random Pointer](https://leetcode.com/problems/copy-list-with-random-pointer) | Medium | Linked List / Hash Table |
| 9 | [Rotate Image](https://leetcode.com/problems/rotate-image) | Medium | Array / Matrix |
| 10 | [Set Matrix Zeroes](https://leetcode.com/problems/set-matrix-zeroes) | Medium | Array / Matrix |
| 11 | [Clone Graph](https://leetcode.com/problems/clone-graph) | Medium | Graph / DFS / BFS |
| 12 | [Binary Tree Level Order Traversal](https://leetcode.com/problems/binary-tree-level-order-traversal) | Medium | Tree / BFS |
| 13 | [Median of Two Sorted Arrays](https://leetcode.com/problems/median-of-two-sorted-arrays) | Hard | Binary Search |
| 14 | [Regular Expression Matching](https://leetcode.com/problems/regular-expression-matching) | Hard | DP / Recursion |
| 15 | [Reverse Nodes in k-Group](https://leetcode.com/problems/reverse-nodes-in-k-group) | Hard | Linked List |
| 16 | [Asteroid Collision](https://leetcode.com/problems/asteroid-collision) | Medium | Stack |
| 17 | [Cheapest Flights Within K Stops](https://leetcode.com/problems/cheapest-flights-within-k-stops) | Medium | Graph / DP / BFS |
| 18 | [Construct Binary Tree from Preorder and Inorder Traversal](https://leetcode.com/problems/construct-binary-tree-from-preorder-and-inorder-traversal) | Medium | Tree / Divide and Conquer |
| 19 | [Largest Rectangle in Histogram](https://leetcode.com/problems/largest-rectangle-in-histogram) | Hard | Monotonic Stack |
| 20 | [Sudoku Solver](https://leetcode.com/problems/sudoku-solver) | Hard | Backtracking / Matrix |

</details>

## LinkedIn

<details>
<summary>View 20 Problems (2025-2026 Most Frequent)</summary>

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Nested List Weight Sum](https://leetcode.com/problems/nested-list-weight-sum) | Medium | DFS / Recursion |
| 2 | [Nested List Weight Sum II](https://leetcode.com/problems/nested-list-weight-sum-ii) | Medium | Stack / DFS |
| 3 | [Can Place Flowers](https://leetcode.com/problems/can-place-flowers) | Easy | Array / Greedy |
| 4 | [Find Leaves of Binary Tree](https://leetcode.com/problems/find-leaves-of-binary-tree) | Medium | Tree / DFS |
| 5 | [Max Stack](https://leetcode.com/problems/max-stack) | Hard | Stack / Linked List / Design |
| 6 | [All O'one Data Structure](https://leetcode.com/problems/all-oone-data-structure) | Hard | Hash Table / Linked List / Design |
| 7 | [Shortest Word Distance II](https://leetcode.com/problems/shortest-word-distance-ii) | Medium | Hash Table / Design |
| 8 | [Find the Celebrity](https://leetcode.com/problems/find-the-celebrity) | Medium | Two Pointers / Graph |
| 9 | [Maximum Subarray](https://leetcode.com/problems/maximum-subarray) | Medium | Array / DP |
| 10 | [Maximum Product Subarray](https://leetcode.com/problems/maximum-product-subarray) | Medium | Array / DP |
| 11 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium | Array / Sorting |
| 12 | [Edit Distance](https://leetcode.com/problems/edit-distance) | Medium | Dynamic Programming |
| 13 | [Design Add and Search Words Data Structure](https://leetcode.com/problems/design-add-and-search-words-data-structure) | Medium | Trie / Design |
| 14 | [Word Ladder](https://leetcode.com/problems/word-ladder) | Hard | BFS / Graphs |
| 15 | [Insert Delete GetRandom O(1)](https://leetcode.com/problems/insert-delete-getrandom-o1) | Medium | Design / Hash Table |
| 16 | [Valid Parentheses](https://leetcode.com/problems/valid-parentheses) | Easy | Stack / String |
| 17 | [Isomorphic Strings](https://leetcode.com/problems/isomorphic-strings) | Easy | String / Hash Table |
| 18 | [Decode Ways](https://leetcode.com/problems/decode-ways) | Medium | Dynamic Programming |
| 19 | [House Robber II](https://leetcode.com/problems/house-robber-ii) | Medium | Dynamic Programming |
| 20 | [Combination Sum II](https://leetcode.com/problems/combination-sum-ii) | Medium | Backtracking |

</details>

## OpenAI

<details>
<summary>View 20 Problems (2025-2026 -- Production-Oriented)</summary>

OpenAI interviews focus on practical engineering over LeetCode puzzles. Problems are drawn from a bank of ~8 core challenges with progressive difficulty layers. Python is strongly recommended.

**Core Custom Problems (Most Frequently Reported)**

| No. | Problem | Difficulty | Category | Context |
| --- | ------- | ---------- | -------- | ------- |
| 1 | KV Store Serialize/Deserialize | Hard | Design / Strings | Multi-part: basic serialization, file persistence, multithreading, versioned store |
| 2 | CD Directory Navigation | Hard | String / Path Resolution | Implement `cd()` with relative/absolute paths, `..`, `.`, `~`, symlink cycle detection |
| 3 | Excel/Spreadsheet Engine | Hard | Graph / Design | `getCell()` O(1), `setCell()` with formula dependencies, circular dependency detection |
| 4 | In-Memory Database | Hard | Database Design | `select()` with WHERE, AND, ORDER BY, comparison operators -- no SQL parsing |
| 5 | Resumable Iterator | Hard | Iterator / State | Stateful iterator with `getState()`/`setState()`, nested structures, async variants |
| 6 | Async Node Counting | Hard | Distributed / Trees | Count tree nodes using only async parent-child messaging |

**LeetCode-Equivalent Problems**

| No. | Problem | Difficulty | Category | Context |
| --- | ------- | ---------- | -------- | ------- |
| 7 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium | Design | Inference KV cache -- most frequently reported |
| 8 | [Time Based Key-Value Store](https://leetcode.com/problems/time-based-key-value-store) | Medium | Design / Binary Search | Model checkpoint storage |
| 9 | [Snapshot Array](https://leetcode.com/problems/snapshot-array) | Medium | Design / Binary Search | Model state checkpointing |
| 10 | [Alien Dictionary](https://leetcode.com/problems/alien-dictionary) | Hard | Graph / Topological Sort | Tokenizer ordering |
| 11 | [Web Crawler Multithreaded](https://leetcode.com/problems/web-crawler-multithreaded) | Medium | Concurrency / BFS | Training data crawling |
| 12 | [LFU Cache](https://leetcode.com/problems/lfu-cache) | Hard | Design | Advanced caching |
| 13 | [Decode String](https://leetcode.com/problems/decode-string) | Medium | Stack / Strings | String processing |
| 14 | [Word Ladder](https://leetcode.com/problems/word-ladder) | Hard | BFS / Graphs | NLP transformations |
| 15 | [Design Memory Allocator](https://leetcode.com/problems/design-memory-allocator) | Medium | Design / Simulation | GPU memory management |
| 16 | [Game of Life](https://leetcode.com/problems/game-of-life) | Medium | Simulation / Matrix | Extended to infinite board |
| 17 | [Meeting Rooms II](https://leetcode.com/problems/meeting-rooms-ii) | Medium | Intervals / Heap | Interval scheduling |
| 18 | [Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree) | Hard | Trees / Design | Data persistence |
| 19 | [Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements) | Medium | Heap / Hash | ML preprocessing |
| 20 | [Course Schedule II](https://leetcode.com/problems/course-schedule-ii) | Medium | Graph / Topological Sort | Dependency resolution |

</details>

## Anthropic

<details>
<summary>View Interview Guide (2025-2026 -- Custom Problems + Concurrency Round)</summary>

Anthropic uses CodeSignal OA (60-90 min) followed by a 4-6 hour onsite with 4-6 rounds. Python expected. AI tools strictly prohibited. Problems are drawn from a bank of ~6 core custom challenges with progressive difficulty layers.

**Core Custom Coding Problems (Most Frequently Reported)**

| No. | Problem | Difficulty | Category | Context |
| --- | ------- | ---------- | -------- | ------- |
| 1 | In-Memory Database | Hard | Design | 4 levels: SET/GET/DELETE -> filtered scans -> TTL -> backup/restore |
| 2 | Web Crawler | Hard | BFS / Concurrency | BFS crawl -> multithreaded/async optimization |
| 3 | LRU Cache (Bugfix + Extend) | Hard | Design / Debugging | Fix bugs, add persistence, handle `*args`/`**kwargs` |
| 4 | Stack Trace / Profiler | Hard | Parsing / Design | Convert sampling data to chronological events |
| 5 | Tokenization Engine | Hard | String / NLP | Code review, tokenize/detokenize with vocabulary coverage |
| 6 | Distributed Mode/Median | Hard | Distributed Systems | Compute across 10 nodes with bandwidth constraints |

**LeetCode Practice Problems (Mapped to Anthropic's Focus Areas)**

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium | Design |
| 2 | [Web Crawler Multithreaded](https://leetcode.com/problems/web-crawler-multithreaded) | Medium | Concurrency / BFS |
| 3 | [Implement Trie (Prefix Tree)](https://leetcode.com/problems/implement-trie-prefix-tree) | Medium | Trie / NLP |
| 4 | [Word Break](https://leetcode.com/problems/word-break) | Medium | DP / Strings |
| 5 | [Design Hit Counter](https://leetcode.com/problems/design-hit-counter) | Medium | Design |
| 6 | [Time Based Key-Value Store](https://leetcode.com/problems/time-based-key-value-store) | Medium | Design / Binary Search |
| 7 | [Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree) | Hard | Trees / Design |
| 8 | [Merge k Sorted Lists](https://leetcode.com/problems/merge-k-sorted-lists) | Hard | Heap / Distributed |
| 9 | [Course Schedule II](https://leetcode.com/problems/course-schedule-ii) | Medium | Graph / Topological Sort |
| 10 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium | Graph / DFS |

**Key Focus Areas**: AI safety/alignment (Constitutional AI, RLHF, red-teaming), systems engineering (distributed training, inference optimization), concurrency/parallel programming, Transformer architecture depth

</details>

## Palantir

<details>
<summary>View 20 Problems + Unique Interview Format (2025-2026)</summary>

Palantir's onsite gives you 3 of 4 round types: **Decomposition**, **System Design**, **Re-engineering (Debugging)**, and **Coding**. Each round includes 20 min of behavioral questions.

**Most Frequently Asked Coding Problems**

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium | Intervals / Sorting |
| 2 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium | Graph / DFS / BFS |
| 3 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium | Design / Hash Map |
| 4 | [Course Schedule](https://leetcode.com/problems/course-schedule) | Medium | Graph / Topological Sort |
| 5 | [Course Schedule II](https://leetcode.com/problems/course-schedule-ii) | Medium | Graph / Topological Sort |
| 6 | [All Ancestors of a Node in DAG](https://leetcode.com/problems/all-ancestors-of-a-node-in-a-directed-acyclic-graph) | Medium | Graph / DFS |
| 7 | [Merge k Sorted Lists](https://leetcode.com/problems/merge-k-sorted-lists) | Hard | Heap / Linked List |
| 8 | [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water) | Hard | Two Pointers / Stack |
| 9 | [Regular Expression Matching](https://leetcode.com/problems/regular-expression-matching) | Hard | DP / String |
| 10 | [Subdomain Visit Count](https://leetcode.com/problems/subdomain-visit-count) | Medium | Hash Map / String |
| 11 | [Find the Celebrity](https://leetcode.com/problems/find-the-celebrity) | Medium | Array / Logic |
| 12 | [UTF-8 Validation](https://leetcode.com/problems/utf-8-validation) | Medium | Bit Manipulation |
| 13 | [Container With Most Water](https://leetcode.com/problems/container-with-most-water) | Medium | Two Pointers |
| 14 | [Max Area of Island](https://leetcode.com/problems/max-area-of-island) | Medium | Graph / DFS |
| 15 | [Rotate Image](https://leetcode.com/problems/rotate-image) | Medium | Array / Matrix |
| 16 | [Integer to English Words](https://leetcode.com/problems/integer-to-english-words) | Hard | String / Math |
| 17 | [Shortest Path to Get All Keys](https://leetcode.com/problems/shortest-path-to-get-all-keys) | Hard | BFS / Bitmask |
| 18 | [Construct Quad Tree](https://leetcode.com/problems/construct-quad-tree) | Medium | Tree / Recursion |
| 19 | [Inorder Successor in BST](https://leetcode.com/problems/inorder-successor-in-bst) | Medium | Tree / BST |
| 20 | [Contains Duplicate III](https://leetcode.com/problems/contains-duplicate-iii) | Hard | BST / Bucket Sort |

**Unique Interview Rounds**
- **Decomposition**: Break down open-ended real-world problems (e.g., "Design tech to help elderly cook safely"). Non-coding.
- **Re-engineering (Debugging)**: Debug 500-1000 lines of buggy code with red herrings
- **System Design**: Focus on data integration, ontology design, access control (ABAC)
- **FDSE vs SWE**: Forward-deployed roles emphasize client-facing scenarios; backend roles emphasize scale

</details>

## Databricks

<details>
<summary>View 25 Problems (2025-2026 Most Frequent -- includes dedicated concurrency round)</summary>

Databricks has a unique **dedicated concurrency/multithreading round** (1 hour). OA is 4 problems in 70 minutes on CodeSignal.

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Capacity To Ship Packages Within D Days](https://leetcode.com/problems/capacity-to-ship-packages-within-d-days) | Medium | Binary Search |
| 2 | [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water) | Hard | Two Pointers / Stack |
| 3 | [Max Stack](https://leetcode.com/problems/max-stack) | Hard | Stack / Linked List / Design |
| 4 | [All O'one Data Structure](https://leetcode.com/problems/all-oone-data-structure) | Hard | Hash Table / Design |
| 5 | [Word Break](https://leetcode.com/problems/word-break) | Medium | DP / Trie |
| 6 | [Rotting Oranges](https://leetcode.com/problems/rotting-oranges) | Medium | BFS / Matrix |
| 7 | [All Nodes Distance K in Binary Tree](https://leetcode.com/problems/all-nodes-distance-k-in-binary-tree) | Medium | Tree / BFS / DFS |
| 8 | [Decode String](https://leetcode.com/problems/decode-string) | Medium | Stack / Recursion |
| 9 | [K Closest Points to Origin](https://leetcode.com/problems/k-closest-points-to-origin) | Medium | Heap / Math |
| 10 | [Asteroid Collision](https://leetcode.com/problems/asteroid-collision) | Medium | Stack |
| 11 | [Design Hit Counter](https://leetcode.com/problems/design-hit-counter) | Medium | Design / Queue |
| 12 | [Time Based Key-Value Store](https://leetcode.com/problems/time-based-key-value-store) | Medium | Design / Binary Search |
| 13 | [Snapshot Array](https://leetcode.com/problems/snapshot-array) | Medium | Design / Binary Search |
| 14 | [Find All Anagrams in a String](https://leetcode.com/problems/find-all-anagrams-in-a-string) | Medium | Sliding Window |
| 15 | [Cheapest Flights Within K Stops](https://leetcode.com/problems/cheapest-flights-within-k-stops) | Medium | Graph / BFS / DP |
| 16 | [Binary Search Tree Iterator](https://leetcode.com/problems/binary-search-tree-iterator) | Medium | Stack / Tree / Design |
| 17 | [House Robber](https://leetcode.com/problems/house-robber) | Medium | Dynamic Programming |
| 18 | [Interval List Intersections](https://leetcode.com/problems/interval-list-intersections) | Medium | Two Pointers |
| 19 | [Print in Order](https://leetcode.com/problems/print-in-order) | Easy | Concurrency |
| 20 | [Print FooBar Alternately](https://leetcode.com/problems/print-foobar-alternately) | Medium | Concurrency |
| 21 | [Building H2O](https://leetcode.com/problems/building-h2o) | Medium | Concurrency |
| 22 | [The Dining Philosophers](https://leetcode.com/problems/the-dining-philosophers) | Medium | Concurrency |
| 23 | [Course Schedule II](https://leetcode.com/problems/course-schedule-ii) | Medium | Graph / Topological Sort |
| 24 | [Alien Dictionary](https://leetcode.com/problems/alien-dictionary) | Hard | Graph / Topological Sort |
| 25 | [Median of Two Sorted Arrays](https://leetcode.com/problems/median-of-two-sorted-arrays) | Hard | Binary Search |

</details>

## Flipkart

<details>
<summary>View Problems</summary>

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Add Two Numbers](https://leetcode.com/problems/add-two-numbers) | Medium | Linked List / Math |

</details>

---

## About This Repository

This repository covers 500+ coding problems across 13+ companies, organized by company and topic. Includes NeetCode 150, Blind 75, system design guides, and ML/AI interview resources.

**[Complete System Design Interview Guide](SYSTEM_DESIGN_INTERVIEW.md)** - 25 system design problems with complexity ratings and company tags.

## Contributing

Contributions are welcome. Please feel free to submit a pull request with new questions, corrections, or additional company coverage.

## Maintainer

[@ombharatiya](https://github.com/ombharatiya) -- [Twitter](https://twitter.com/ombharatiya) | [LinkedIn](https://linkedin.com/in/ombharatiya)

## License

GPL-3.0 -- see [LICENSE](LICENSE) for details.
