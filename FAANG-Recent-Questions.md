# FAANG / MAANG+ Most Recently Asked Coding Interview Questions

> A comprehensive list of the most recently asked coding interview questions at top tech companies (2025-2026). Questions are organized by company and topic to help you prepare effectively.
>
> **Looking for AI labs?** DeepMind, xAI, Mistral, Perplexity, Scale AI, Cohere, Cursor, Waymo, Sierra, Glean and more live in the companion [AI Labs & AI Companies guide](./AI-Companies-Interview-Questions.md).

## The Single Biggest Change in 2026: AI-Assisted Rounds

The format shifted more in the last year than in the previous five. What changed, and where:

| Company | AI policy in interviews |
| ------- | ----------------------- |
| **Meta** | AI-enabled coding round rolling out to all SWE roles, 3-panel CoderPad, AI reads files but can't edit. For E6+ it *is* the coding round. |
| **Google** | Piloting an AI-assisted "code comprehension" round with Gemini; simultaneously reinstated an in-person round to curb cheating. |
| **LinkedIn** | AI-enabled round is now standard: one of two coding rounds, scored 1-4, where 3 passes. |
| **DoorDash** | Publicly rebuilding interviews around AI: a 60-min AI-assisted working session in your own IDE. |
| **OpenAI** | Agentic coding round in beta (drive an AI agent on a real codebase). The *only* round where AI is allowed. |
| **Anthropic** | Split policy: AI permitted on the performance take-home, strictly prohibited in live interviews. |
| **Sierra** | Removed algorithm interviews entirely. Plan -> Build (2h with any AI) -> Review. |
| **Microsoft** | Team-dependent (CoreAI/Copilot teams may allow GitHub Copilot). Ask your recruiter. |
| **Tesla** | Googling allowed; LLM use at interviewer discretion. |
| **Amazon, Apple, ByteDance, Palantir, Uber, Airbnb** | No AI-assisted round reported; ByteDance and Palantir explicitly ban AI use. |

Where AI is allowed, the rubric moved to **verification**: test before you trust, and explain the output. Where it's banned, expect proctoring, in-person rounds, and debug-the-supplied-code formats instead.

## Table of Contents

- [Meta (formerly Facebook)](#meta-formerly-facebook)
  - [Arrays and Strings](#meta-arrays-and-strings)
  - [Linked Lists](#meta-linked-lists)
  - [Trees and Graphs](#meta-trees-and-graphs)
  - [Recursion and Backtracking](#meta-recursion-and-backtracking)
  - [Sorting and Searching](#meta-sorting-and-searching)
  - [Dynamic Programming](#meta-dynamic-programming)
  - [Design](#meta-design)
- [Amazon](#amazon)
  - [Arrays and Strings](#amazon-arrays-and-strings)
  - [Sliding Window and Two Pointers](#amazon-sliding-window-and-two-pointers)
  - [Trees and Graphs](#amazon-trees-and-graphs)
  - [Heaps and Priority Queues](#amazon-heaps-and-priority-queues)
  - [Dynamic Programming](#amazon-dynamic-programming)
  - [Design](#amazon-design)
- [Apple](#apple)
  - [Arrays and Strings](#apple-arrays-and-strings)
  - [Trees and Graphs](#apple-trees-and-graphs)
  - [Design and System Coding](#apple-design-and-system-coding)
- [Netflix](#netflix)
  - [System Design Coding](#netflix-system-design-coding)
  - [Algorithms](#netflix-algorithms)
- [Google](#google)
  - [Arrays and Strings](#google-arrays-and-strings)
  - [Trees and Graphs](#google-trees-and-graphs)
  - [Dynamic Programming](#google-dynamic-programming)
  - [Binary Search and Special Topics](#google-binary-search-and-special-topics)
- [Microsoft](#microsoft)
  - [Arrays and Strings](#microsoft-arrays-and-strings)
  - [Linked Lists](#microsoft-linked-lists)
  - [Trees and Graphs](#microsoft-trees-and-graphs)
  - [Design and Hard Problems](#microsoft-design-and-hard-problems)
- [LinkedIn](#linkedin)
  - [Data Structure Design](#linkedin-data-structure-design)
  - [Trees and Graphs](#linkedin-trees-and-graphs)
  - [Arrays and DP](#linkedin-arrays-and-dp)
- [OpenAI](#openai)
  - [Core Custom Problems](#openai-core-custom-problems)
  - [LeetCode-Equivalent Problems](#openai-leetcode-equivalent-problems)
  - [System Design](#openai-system-design)
  - [ML and AI Technical](#openai-ml-and-ai-technical)
- [Anthropic](#anthropic)
  - [Core Custom Coding Problems](#anthropic-core-custom-coding-problems)
  - [LeetCode Practice](#anthropic-leetcode-practice-mapped-to-focus-areas)
  - [System Design](#anthropic-system-design)
  - [ML and AI Safety](#anthropic-ml-and-ai-safety)
- [Palantir](#palantir)
  - [Coding Problems](#palantir-coding-problems)
  - [OA Problems](#palantir-oa-problems-2026-hackerrank-3-part)
  - [System Design](#palantir-system-design)
  - [Unique Rounds](#palantir-unique-rounds)
- [Tesla](#tesla)
  - [Algorithms](#tesla-algorithms)
  - [System Design](#tesla-system-design)
  - [Embedded Systems](#tesla-embedded-systems)
- [Databricks](#databricks)
  - [Algorithms and Design](#databricks-algorithms-and-design)
  - [Custom Problems](#databricks-custom-problems)
  - [Concurrency (Dedicated Round)](#databricks-concurrency-dedicated-round)
  - [System Design](#databricks-system-design)
- [Stripe](#stripe)
  - [Coding and Integration](#stripe-coding-and-integration)
  - [Bug Squash and API Design](#stripe-bug-squash-and-api-design)
- [NVIDIA](#nvidia)
  - [Algorithms](#nvidia-algorithms)
  - [GPU and Systems](#nvidia-gpu-and-systems)
- [Uber](#uber)
  - [Algorithms](#uber-algorithms)
  - [System Design](#uber-system-design)
- [ByteDance / TikTok](#bytedance--tiktok)
  - [Algorithms](#bytedance-algorithms)
  - [System Design](#bytedance-system-design)
- [Airbnb](#airbnb)
  - [Algorithms](#airbnb-algorithms)
  - [System Design](#airbnb-system-design)
- [DoorDash](#doordash)
  - [Algorithms](#doordash-algorithms)
  - [AI-Assisted and Custom Rounds](#doordash-ai-assisted-and-custom-rounds)
- [AI Labs & AI Companies](./AI-Companies-Interview-Questions.md), separate guide: DeepMind, xAI, Mistral, Perplexity, Scale AI, Cohere, Cursor, Waymo, and 10+ more
- [Topic-wise Questions](#topic-wise-questions)

---

## Meta (formerly Facebook)

> **2025-2026 Trends**: De-emphasis of DP, rise of expression parsing/stack problems, streaming and sparse data, speed and clean code prioritized over brute force. ~26% Easy, 60% Medium, 14% Hard. **New in 2026**: AI-Enabled Coding Round rolling out to all SWE roles, 60 min in a 3-panel CoderPad (file explorer, editor, AI chat; GPT-5, Claude Sonnet, Gemini, Llama 4 available; AI reads files but cannot edit). Three phases: (1) fix a non-algorithmic bug, (2) build a 120+ line feature with AI expected, (3) optimize for larger datasets. Scored on problem solving, code quality, **verification of AI output**, and communication, for E4-E5 it randomly replaces one coding round; for E6+ it IS the coding round. Candidates report the in-interview AI is weaker than in practice mode. Behavioral round weight increased, it can single-handedly downlevel E5 to E4. Candidates increasingly get *variants* of tagged problems rather than the originals. Two problems in 35 minutes for traditional rounds -- speed is king.

### Meta Arrays and Strings

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Minimum Remove to Make Valid Parentheses](https://leetcode.com/problems/minimum-remove-to-make-valid-parentheses) | Medium |
| 2 | [Valid Palindrome II](https://leetcode.com/problems/valid-palindrome-ii) | Easy |
| 3 | [Valid Palindrome](https://leetcode.com/problems/valid-palindrome) | Easy |
| 4 | [Subarray Sum Equals K](https://leetcode.com/problems/subarray-sum-equals-k) | Medium |
| 5 | [Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self) | Medium |
| 6 | [Move Zeroes](https://leetcode.com/problems/move-zeroes) | Easy |
| 7 | [Basic Calculator II](https://leetcode.com/problems/basic-calculator-ii) | Medium |
| 8 | [Buildings With an Ocean View](https://leetcode.com/problems/buildings-with-an-ocean-view) | Medium |
| 9 | [Custom Sort String](https://leetcode.com/problems/custom-sort-string) | Medium |
| 10 | [Continuous Subarray Sum](https://leetcode.com/problems/continuous-subarray-sum) | Medium |
| 11 | [Add Strings](https://leetcode.com/problems/add-strings) | Easy |
| 12 | [Maximum Swap](https://leetcode.com/problems/maximum-swap) | Medium |
| 13 | [Valid Word Abbreviation](https://leetcode.com/problems/valid-word-abbreviation) | Easy |
| 14 | [Merge Strings Alternately](https://leetcode.com/problems/merge-strings-alternately) | Easy |
| 15 | [Diagonal Traverse](https://leetcode.com/problems/diagonal-traverse) | Medium |
| 16 | [Next Permutation](https://leetcode.com/problems/next-permutation) | Medium |
| 17 | [Interval List Intersections](https://leetcode.com/problems/interval-list-intersections) | Medium |
| 18 | [Validate IP Address](https://leetcode.com/problems/validate-ip-address) | Medium |
| 19 | [Remove All Adjacent Duplicates in String II](https://leetcode.com/problems/remove-all-adjacent-duplicates-in-string-ii) | Medium |
| 20 | [Greatest Common Divisor of Strings](https://leetcode.com/problems/greatest-common-divisor-of-strings) | Easy |
| 21 | [Toeplitz Matrix](https://leetcode.com/problems/toeplitz-matrix) | Easy |
| 22 | [Find the Length of the Longest Common Prefix](https://leetcode.com/problems/find-the-length-of-the-longest-common-prefix) | Medium |
| 23 | [Longest Substring with At Most K Distinct Characters](https://leetcode.com/problems/longest-substring-with-at-most-k-distinct-characters) | Medium |
| 24 | [Range Sum Query 2D - Immutable](https://leetcode.com/problems/range-sum-query-2d-immutable) | Medium |
| 25 | [First Missing Positive](https://leetcode.com/problems/first-missing-positive) | Hard |
| 26 | [Integer to English Words](https://leetcode.com/problems/integer-to-english-words) | Hard |

### Meta Linked Lists

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Merge Two Sorted Lists](https://leetcode.com/problems/merge-two-sorted-lists) | Easy |
| 2 | [Copy List with Random Pointer](https://leetcode.com/problems/copy-list-with-random-pointer) | Medium |
| 3 | [Reorder List](https://leetcode.com/problems/reorder-list) | Medium |
| 4 | [Insert into a Sorted Circular Linked List](https://leetcode.com/problems/insert-into-a-sorted-circular-linked-list) | Medium |
| 5 | [Remove Nth Node From End of List](https://leetcode.com/problems/remove-nth-node-from-end-of-list) | Medium |

### Meta Trees and Graphs

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Binary Tree Vertical Order Traversal](https://leetcode.com/problems/binary-tree-vertical-order-traversal) | Medium |
| 2 | [Lowest Common Ancestor of a Binary Tree](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-tree) | Medium |
| 3 | [Binary Tree Right Side View](https://leetcode.com/problems/binary-tree-right-side-view) | Medium |
| 4 | [Diameter of Binary Tree](https://leetcode.com/problems/diameter-of-binary-tree) | Easy |
| 5 | [Clone Graph](https://leetcode.com/problems/clone-graph) | Medium |
| 6 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium |
| 7 | [Accounts Merge](https://leetcode.com/problems/accounts-merge) | Medium |
| 8 | [Shortest Path in Binary Matrix](https://leetcode.com/problems/shortest-path-in-binary-matrix) | Medium |
| 9 | [Making a Large Island](https://leetcode.com/problems/making-a-large-island) | Hard |
| 10 | [Range Sum of BST](https://leetcode.com/problems/range-sum-of-bst) | Easy |
| 11 | [Lowest Common Ancestor of a Binary Tree III](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-tree-iii) | Medium |
| 12 | [All Nodes Distance K in Binary Tree](https://leetcode.com/problems/all-nodes-distance-k-in-binary-tree) | Medium |
| 13 | [Convert BST to Sorted Doubly Linked List](https://leetcode.com/problems/convert-binary-search-tree-to-sorted-doubly-linked-list) | Medium |
| 14 | [K Closest Points to Origin](https://leetcode.com/problems/k-closest-points-to-origin) | Medium |
| 15 | [Sum Root to Leaf Numbers](https://leetcode.com/problems/sum-root-to-leaf-numbers) | Medium |
| 16 | [Max Area of Island](https://leetcode.com/problems/max-area-of-island) | Medium |
| 17 | [Course Schedule II](https://leetcode.com/problems/course-schedule-ii) | Medium |
| 18 | [Diagonal Traverse II](https://leetcode.com/problems/diagonal-traverse-ii) | Medium |

### Meta Recursion and Backtracking

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Letter Combinations of a Phone Number](https://leetcode.com/problems/letter-combinations-of-a-phone-number) | Medium |
| 2 | [Permutations](https://leetcode.com/problems/permutations) | Medium |
| 3 | [Subsets](https://leetcode.com/problems/subsets) | Medium |
| 4 | [Remove Invalid Parentheses](https://leetcode.com/problems/remove-invalid-parentheses) | Hard |
| 5 | [Expression Add Operators](https://leetcode.com/problems/expression-add-operators) | Hard |
| 6 | [Strobogrammatic Number II](https://leetcode.com/problems/strobogrammatic-number-ii) | Medium |

### Meta Sorting and Searching

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Random Pick with Weight](https://leetcode.com/problems/random-pick-with-weight) | Medium |
| 2 | [Kth Largest Element in an Array](https://leetcode.com/problems/kth-largest-element-in-an-array) | Medium |
| 3 | [Find Peak Element](https://leetcode.com/problems/find-peak-element) | Medium |
| 4 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium |
| 5 | [Pow(x, n)](https://leetcode.com/problems/powx-n) | Medium |
| 6 | [Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements) | Medium |

### Meta Dynamic Programming

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Best Time to Buy and Sell Stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock) | Easy |
| 2 | [Word Break](https://leetcode.com/problems/word-break) | Medium |
| 3 | [Decode Ways](https://leetcode.com/problems/decode-ways) | Medium |
| 4 | [Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring) | Medium |

### Meta Design

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium |
| 2 | [Dot Product of Two Sparse Vectors](https://leetcode.com/problems/dot-product-of-two-sparse-vectors) | Medium |
| 3 | [Design Tic-Tac-Toe](https://leetcode.com/problems/design-tic-tac-toe) | Medium |
| 4 | [Nested List Weight Sum](https://leetcode.com/problems/nested-list-weight-sum) | Medium |

### Meta Custom and AI-Round Problems (2026)

| No. | Problem | Category | Description |
| --- | ------- | -------- | ----------- |
| 1 | Maze Solver with Path Printing | AI-Enabled Round | Multi-phase build with directional gates; ~9 problems in rotation |
| 2 | Maximize Unique Characters from Word List | AI-Enabled Round | Staged build + optimization (greedy -> trie switch forced by tests) |
| 3 | Card Game: Find Three Cards Summing to 15 | AI-Enabled Round | Feature build with progressive test cases |
| 4 | Friend Recommendation System | AI-Enabled Round / Graphs | Build then optimize for larger datasets |
| 5 | Task Management System | OOP / Design | Design and implement a small task manager class |
| 6 | Merge 3 Sorted Arrays | Arrays | Merge-k variant restricted to 3 arrays; follow-ups on duplicates |
| 7 | Minimum element per binary-tree level | Trees / BFS | Reported in late-2025 infra screens with matrix distance calculation |

---

## Amazon

> **2025-2026 Trends**: Practical, real-world framing. Heap-based reasoning emphasized. OA structure: Q1 is Array/String/Sliding Window, Q2 is Graph/Trees/DP/Heap. ~19% Easy, 60% Medium, 21% Hard. **New in 2026**: HackerRank OA = 2 coding problems (~70 min) + Work Simulation (~20 min) + Work Style Assessment (~10-20 min); the SDE II OA adds a 20-minute System Design scenario section. ~75-80% of OA problems are Medium, wrapped in Amazon-themed framing (servers, warehouses, parcels). Onsite is ~50/50 coding vs Leadership Principles in every round, plus Bar Raiser. Rising: weighted-shortest-path/Dijkstra problems; system design now probes deployment topology and on-call readiness. **No AI-assisted round reported**: Amazon instead rotates custom OA problem sets aggressively, so pattern prep beats memorization. Under-prepared LPs to watch: "Have Backbone, Disagree & Commit", "Are Right A Lot", "Frugality".

### Amazon Arrays and Strings

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Two Sum](https://leetcode.com/problems/two-sum) | Easy |
| 2 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium |
| 3 | [Group Anagrams](https://leetcode.com/problems/group-anagrams) | Medium |
| 4 | [Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self) | Medium |
| 5 | [Maximum Subarray](https://leetcode.com/problems/maximum-subarray) | Medium |
| 6 | [Rotate Image](https://leetcode.com/problems/rotate-image) | Medium |
| 7 | [3Sum](https://leetcode.com/problems/3sum) | Medium |
| 8 | [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water) | Hard |
| 9 | [Integer to English Words](https://leetcode.com/problems/integer-to-english-words) | Hard |
| 10 | [Subarray Sum Equals K](https://leetcode.com/problems/subarray-sum-equals-k) | Medium |
| 11 | [Maximum Frequency After Subarray Operation](https://leetcode.com/problems/maximum-frequency-after-subarray-operation) | Medium |
| 12 | [Max Difference You Can Get From Changing an Integer](https://leetcode.com/problems/max-difference-you-can-get-from-changing-an-integer) | Medium |
| 13 | [Analyze User Website Visit Pattern](https://leetcode.com/problems/analyze-user-website-visit-pattern) | Medium |
| 14 | [Find First and Last Position of Element in Sorted Array](https://leetcode.com/problems/find-first-and-last-position-of-element-in-sorted-array) | Medium |
| 15 | [Max Points on a Line](https://leetcode.com/problems/max-points-on-a-line) | Hard |

### Amazon Sliding Window and Two Pointers

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters) | Medium |
| 2 | [Minimum Window Substring](https://leetcode.com/problems/minimum-window-substring) | Hard |
| 3 | [Container With Most Water](https://leetcode.com/problems/container-with-most-water) | Medium |
| 4 | [Longest Repeating Character Replacement](https://leetcode.com/problems/longest-repeating-character-replacement) | Medium |
| 5 | [Sliding Window Maximum](https://leetcode.com/problems/sliding-window-maximum) | Hard |

### Amazon Trees and Graphs

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium |
| 2 | [Course Schedule](https://leetcode.com/problems/course-schedule) | Medium |
| 3 | [Rotting Oranges](https://leetcode.com/problems/rotting-oranges) | Medium |
| 4 | [Word Ladder](https://leetcode.com/problems/word-ladder) | Hard |
| 5 | [Making a Large Island](https://leetcode.com/problems/making-a-large-island) | Hard |
| 6 | [Lowest Common Ancestor of a Binary Tree](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-tree) | Medium |
| 7 | [Binary Tree Zigzag Level Order Traversal](https://leetcode.com/problems/binary-tree-zigzag-level-order-traversal) | Medium |
| 8 | [Diameter of Binary Tree](https://leetcode.com/problems/diameter-of-binary-tree) | Easy |
| 9 | [Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree) | Hard |
| 10 | [Word Search II](https://leetcode.com/problems/word-search-ii) | Hard |
| 11 | [Alien Dictionary](https://leetcode.com/problems/alien-dictionary) | Hard |
| 12 | [Word Search](https://leetcode.com/problems/word-search) | Medium |

### Amazon Heaps and Priority Queues

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Kth Largest Element in an Array](https://leetcode.com/problems/kth-largest-element-in-an-array) | Medium |
| 2 | [Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements) | Medium |
| 3 | [Merge k Sorted Lists](https://leetcode.com/problems/merge-k-sorted-lists) | Hard |
| 4 | [Find Median from Data Stream](https://leetcode.com/problems/find-median-from-data-stream) | Hard |
| 5 | [Reorganize String](https://leetcode.com/problems/reorganize-string) | Medium |
| 6 | [Task Scheduler](https://leetcode.com/problems/task-scheduler) | Medium |
| 7 | [Maximize Y-Sum by Picking a Triplet of Distinct X-Values](https://leetcode.com/problems/maximize-ysum-by-picking-a-triplet-of-distinct-xvalues) | Medium |
| 8 | [Minimum Cost to Connect Sticks](https://leetcode.com/problems/minimum-cost-to-connect-sticks) | Medium |
| 9 | [The Skyline Problem](https://leetcode.com/problems/the-skyline-problem) | Hard |
| 10 | [Count of Smaller Numbers After Self](https://leetcode.com/problems/count-of-smaller-numbers-after-self) | Hard |

### Amazon Dynamic Programming

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring) | Medium |
| 2 | [Coin Change](https://leetcode.com/problems/coin-change) | Medium |
| 3 | [Maximum Product Subarray](https://leetcode.com/problems/maximum-product-subarray) | Medium |
| 4 | [Jump Game](https://leetcode.com/problems/jump-game) | Medium |
| 5 | [Best Time to Buy and Sell Stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock) | Easy |
| 6 | [Word Break II](https://leetcode.com/problems/word-break-ii) | Hard |
| 7 | [Burst Balloons](https://leetcode.com/problems/burst-balloons) | Hard |
| 8 | [Decode Ways](https://leetcode.com/problems/decode-ways) | Medium |
| 9 | [Word Break](https://leetcode.com/problems/word-break) | Medium |

### Amazon Design

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium |
| 2 | [Insert Delete GetRandom O(1)](https://leetcode.com/problems/insert-delete-getrandom-o1) | Medium |
| 3 | [LFU Cache](https://leetcode.com/problems/lfu-cache) | Hard |
| 4 | [Design In-Memory File System](https://leetcode.com/problems/design-in-memory-file-system) | Hard |
| 5 | [Design Search Autocomplete System](https://leetcode.com/problems/design-search-autocomplete-system) | Hard |
| 6 | [Design Hit Counter](https://leetcode.com/problems/design-hit-counter) | Medium |
| 7 | [Reorder List](https://leetcode.com/problems/reorder-list) | Medium |

### Amazon Custom OA Problems (2026, HackerRank)

Amazon rotates a large bank of themed OA problems. Reported in 2026:

| No. | Problem | Difficulty | Pattern |
| --- | ------- | ---------- | ------- |
| 1 | Server Allocation Cost, customers pick servers with most idle instances; cost = max + min idle before selection | Medium | Heap simulation |
| 2 | Warehouse Distribution, maximize sum of the k/2 least-stocked warehouses from allocation logs | Medium | Binary search + greedy |
| 3 | Minimum Array Operations, min ops so every subarray of length > 1 has non-negative sum | Medium | Prefix-sum state reset |
| 4 | Bug Sorting by Frequency & Code, sort bug reports by frequency desc, then code asc | Medium | Hash + custom comparator |
| 5 | Server Security Level Grouping. Minimize groups of equal/near-equal size per security level | Medium | Greedy / counting |
| 6 | Get DNA Sequence | Medium | Pattern matching |
| 7 | Distribute Parcels / Minimize Maximum Parcels | Medium | Load balancing / binary search |
| 8 | Suitable Warehouse Locations | Medium | Greedy / sorting |
| 9 | Check Similar Passwords | Medium | Strings / hashing |
| 10 | Min Cost To Add New Roads | Hard | MST / Union-Find |
| 11 | Dropped Requests | Hard | Sliding window / rate limiting |
| 12 | Checksum Logic | Hard | Simulation |
| 13 | Longest Match | Hard | Strings / DP |
| 14 | Min Subsegments | Hard | Greedy / partitioning |

### Amazon System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Design a URL shortener | Hashing, storage, redirects (most-reported) |
| 2 | Design Amazon's recommendation system | Collaborative filtering, ranking, scale |
| 3 | Design a distributed rate limiter | Token bucket, distributed counters |
| 4 | Design a notification service | Fan-out, delivery guarantees |
| 5 | Design a parking lot (OOD) | Object modeling |
| 6 | Real-time error-log monitoring, 1M+ writes/sec with sub-second alerting | Kafka/Flink/Elasticsearch |
| 7 | Planet-scale storage; 100x traffic-spike handling; active-active global systems | Senior/Staff prompts |

---

## Apple

> **2025-2026 Trends**: Practical/applied problems over pure algo puzzles, real Apple workload framing (file dedup, iOS task simulation, API throttling). Stricter expectations on edge cases and memory behavior. Design-oriented coding (LRU Cache is most frequently reported). **Still radically team-dependent. No unified loop**: some teams ask standard LC mediums, embedded/hardware teams ask C/C++ memory/optimization, services teams ask API design or debug-broken-code, some skip LeetCode entirely for architecture or take-homes. **New in 2026**: design-style coding questions are disproportionately common (Time Based KV Store, Design Hit Counter, BST iterators); loops for experienced hires are getting longer, 8-9 rounds over several weeks reported; ICT4 candidates report up to 3 phone screens before onsite. **No AI-assisted rounds reported** as of mid-2026. All experiences describe human-only interviews graded on correctness, memory behavior, and boundary handling rather than Hards.

### Apple Arrays and Strings

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Two Sum](https://leetcode.com/problems/two-sum) | Easy |
| 2 | [3Sum](https://leetcode.com/problems/3sum) | Medium |
| 3 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium |
| 4 | [Valid Parentheses](https://leetcode.com/problems/valid-parentheses) | Easy |
| 5 | [Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self) | Medium |
| 6 | [Group Anagrams](https://leetcode.com/problems/group-anagrams) | Medium |
| 7 | [Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters) | Medium |
| 8 | [Longest Repeating Character Replacement](https://leetcode.com/problems/longest-repeating-character-replacement) | Medium |
| 9 | [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water) | Hard |
| 10 | [Best Time to Buy and Sell Stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock) | Easy |
| 11 | [Subarray Sum Equals K](https://leetcode.com/problems/subarray-sum-equals-k) | Medium |
| 12 | [Rotate Image](https://leetcode.com/problems/rotate-image) | Medium |
| 13 | [H-Index](https://leetcode.com/problems/h-index) | Medium |
| 14 | [Minimum Unique Word Abbreviation](https://leetcode.com/problems/minimum-unique-word-abbreviation) | Hard |
| 15 | [Find Minimum in Rotated Sorted Array](https://leetcode.com/problems/find-minimum-in-rotated-sorted-array) | Medium |
| 16 | [Search in Rotated Sorted Array](https://leetcode.com/problems/search-in-rotated-sorted-array) | Medium |
| 17 | [Permutations](https://leetcode.com/problems/permutations) | Medium |

### Apple Trees and Graphs

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium |
| 2 | [Lowest Common Ancestor of a Binary Tree](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-tree) | Medium |
| 3 | [Course Schedule](https://leetcode.com/problems/course-schedule) | Medium |
| 4 | [Sum Root to Leaf Numbers](https://leetcode.com/problems/sum-root-to-leaf-numbers) | Medium |
| 5 | [Check Completeness of a Binary Tree](https://leetcode.com/problems/check-completeness-of-a-binary-tree) | Medium |
| 6 | [Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree) | Hard |
| 7 | [Bus Routes](https://leetcode.com/problems/bus-routes) | Hard |
| 8 | [Vertical Order Traversal of a Binary Tree](https://leetcode.com/problems/vertical-order-traversal-of-a-binary-tree) | Hard |
| 9 | [Flood Fill](https://leetcode.com/problems/flood-fill) (both BFS and DFS required) | Easy |
| 10 | [Word Ladder](https://leetcode.com/problems/word-ladder) | Hard |
| 11 | [Coin Change](https://leetcode.com/problems/coin-change) | Medium |
| 12 | [Longest Increasing Subsequence](https://leetcode.com/problems/longest-increasing-subsequence) | Medium |
| 13 | [House Robber](https://leetcode.com/problems/house-robber) (circular II extension probed) | Medium |

### Apple Design and System Coding

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium |
| 2 | [Word Break](https://leetcode.com/problems/word-break) | Medium |
| 3 | [Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements) | Medium |
| 4 | [Maximum Profit in Job Scheduling](https://leetcode.com/problems/maximum-profit-in-job-scheduling) | Hard |
| 5 | [Median of Two Sorted Arrays](https://leetcode.com/problems/median-of-two-sorted-arrays) | Hard |
| 6 | [Search a 2D Matrix](https://leetcode.com/problems/search-a-2d-matrix) | Medium |
| 7 | [Time Based Key-Value Store](https://leetcode.com/problems/time-based-key-value-store) | Medium |
| 8 | [Design Hit Counter](https://leetcode.com/problems/design-hit-counter) | Medium |
| 9 | [Design Add and Search Words Data Structure](https://leetcode.com/problems/design-add-and-search-words-data-structure) | Medium |
| 10 | [Binary Search Tree Iterator](https://leetcode.com/problems/binary-search-tree-iterator) (lazy inorder traversal) | Medium |
| 11 | [Implement Queue using Stacks](https://leetcode.com/problems/implement-queue-using-stacks) | Easy |

### Apple Custom Problems

| No. | Problem | Category | Description |
| --- | ------- | -------- | ----------- |
| 1 | Memory-efficient ProRAW image decoder | Systems (ICT4) | Decode for iOS devices with <=1GB RAM |
| 2 | Lock-free queue for real-time watchOS sensor data | Concurrency (ICT4) | Lock-free implementation |
| 3 | Debug a PyTorch U-Net shape mismatch | ML Debugging | ML Engineer round |
| 4 | Bag-of-Words similarity search | ML Coding | ML Engineer round |
| 5 | Find Minimum Processing Rate | Binary Search | Koko-style binary search on answer (ML Engineer) |
| 6 | Minimum Cells to Bridge a Magic Grid | Graph / BFS | Islands/bridging grid hard |
| 7 | Library Management System | OOP Design | Actual class structure expected |

### Apple System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Redesign iCloud conflict resolution for 10M concurrent document edits | CRDTs / OT / version vectors (ICT4) |
| 2 | Unified privacy framework for HealthKit data across iOS/watchOS/ResearchKit | Encryption, compliance, sync (ICT4) |
| 3 | Monolith-to-microservices migration with data migration at scale | ICT3/4 |
| 4 | "Redesign Xcode for the next decade of platforms" / "Design a feature for 2030" | Open-ended innovation rounds |

---

## Netflix

> **2025-2026 Trends**: Streaming/recommendation-themed problem wrappers. Graph-heavy focus (topological sort, shortest path, CDN routing). System design is the pass/fail determinant. Concurrency and rate limiting emphasized. Code must compile and run with unit tests. **Biggest 2026 change: formal engineering levels.** Netflix moved away from the single "Senior Engineer" rung to an explicit multi-band ladder (roughly E1/L4-E7). The same coding answer is now scored against the target level, so an answer that passes at E4 can fail at E6 for being "too tactical." Loops are decentralized and team-owned: hiring manager is involved from the first screen; 4-6 rounds; tech screen is 45 min on CodeSignal or 60 min on CoderPad depending on team; 1-2 directors often sit in onsites. Coding style favors practical mediums over puzzles, streaming aggregation, rate limiting, caching/TTL behavior, parsing, concurrency, frequently re-skinned with Netflix domain (shows, playlists, watch history). The culture/Keeper Test round remains mandatory in every loop.

### Netflix System Design Coding

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium |
| 2 | [Design Hit Counter](https://leetcode.com/problems/design-hit-counter) | Medium |
| 3 | [Implement Trie (Prefix Tree)](https://leetcode.com/problems/implement-trie-prefix-tree) | Medium |
| 4 | [Find Median from Data Stream](https://leetcode.com/problems/find-median-from-data-stream) | Hard |
| 5 | [Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree) | Hard |
| 6 | [Time Based Key-Value Store](https://leetcode.com/problems/time-based-key-value-store) | Medium |
| 7 | [Logger Rate Limiter](https://leetcode.com/problems/logger-rate-limiter) | Easy |
| 8 | [Min Stack](https://leetcode.com/problems/min-stack) | Medium |

### Netflix Algorithms

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium |
| 2 | [Meeting Rooms II](https://leetcode.com/problems/meeting-rooms-ii) | Medium |
| 3 | [Course Schedule II](https://leetcode.com/problems/course-schedule-ii) | Medium |
| 4 | [Network Delay Time](https://leetcode.com/problems/network-delay-time) | Medium |
| 5 | [Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements) | Medium |
| 6 | [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water) | Hard |
| 7 | [Daily Temperatures](https://leetcode.com/problems/daily-temperatures) | Medium |
| 8 | [Edit Distance](https://leetcode.com/problems/edit-distance) | Medium |
| 9 | [Minimum Window Substring](https://leetcode.com/problems/minimum-window-substring) | Hard |
| 10 | [Koko Eating Bananas](https://leetcode.com/problems/koko-eating-bananas) | Medium |
| 11 | [Rotating the Box](https://leetcode.com/problems/rotating-the-box) | Medium |
| 12 | [Merge k Sorted Lists](https://leetcode.com/problems/merge-k-sorted-lists) | Hard |
| 13 | [Word Search II](https://leetcode.com/problems/word-search-ii) | Hard |
| 14 | [Reconstruct Itinerary](https://leetcode.com/problems/reconstruct-itinerary) | Hard |
| 15 | [Alien Dictionary](https://leetcode.com/problems/alien-dictionary) | Hard |
| 16 | [Parallel Courses](https://leetcode.com/problems/parallel-courses) | Medium |
| 17 | [Clone Graph](https://leetcode.com/problems/clone-graph) | Medium |
| 18 | [Course Schedule](https://leetcode.com/problems/course-schedule) | Medium |
| 19 | [Recover Binary Search Tree](https://leetcode.com/problems/recover-binary-search-tree) | Medium |
| 20 | [Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self) | Medium |
| 21 | [Container With Most Water](https://leetcode.com/problems/container-with-most-water) | Medium |
| 22 | [Department Top Three Salaries](https://leetcode.com/problems/department-top-three-salaries) (data-adjacent roles) | Hard |

### Netflix Custom Problems

Netflix's custom set skews heavily toward caches and watch-history/domain re-skins:

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | Simulate a TTL Cache with LRU Eviction | Medium-Hard | Design / Caching |
| 2 | Implement a Weighted Eviction Cache, eviction by weight/score | Hard | Design / Caching |
| 3 | Implement a Versioned Key-Value Store | Hard | Design (Senior+) |
| 4 | Implement Streaming Word Counter | Medium | Streaming aggregation |
| 5 | Group users with overlapping last-K watched movies | Medium | Hashing / Sets |
| 6 | Design playlist with add/remove/shuffle | Medium | Design |
| 7 | Find longest run of identical consecutive shows | Medium | Arrays |
| 8 | Dedupe titles in a per-shelf viewport; rotating homepage title selector | Medium | Domain simulation |
| 9 | Compute Minimum Task Completion Time | Medium | Scheduling |
| 10 | Implement ordering and undo executor | Medium | Command pattern / undo |
| 11 | Rate limiter for microservices, with graceful degradation when the limiter itself fails | Medium-Hard | Concurrency |
| 12 | Real-Time "Currently Watching" Tracker | Medium | LLD |
| 13 | Binary Array Partition, split binary array into 3 equal-value parts | Medium | Arrays |

### Netflix System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Design the Netflix streaming pipeline (upload -> playable on all devices) | Encoding, storage, delivery |
| 2 | Design a recommendation system including cold-start | ML / ranking |
| 3 | Design a CDN with edge caching / ISP partnerships | Open Connect-flavored |
| 4 | Design a real-time A/B testing platform | Experiment assignment + metrics |
| 5 | Distributed counter abstraction | Based on Netflix's own Counter service, rising prompt |
| 6 | "Reverse system design", deep-dive on a system you built | Plus security/DDoS and multi-region failover |

---

## Google

> **2025-2026 Trends**: Graphs appear in 76% of onsite loops at L4+. Sliding window and binary search on answer are top-tier patterns. Trie and Union-Find questions rising. Roughly 19% of reported problems are Hard. Follow-up questions are standard. **New in 2026**: AI-assisted "Code Comprehension" round piloting. Candidates read, debug, and optimize an existing codebase with **Gemini available** in a CoderPad-style environment (file explorer + editor + AI chat); interviewers explicitly score "AI fluency": prompt engineering, output validation, and debugging of AI output. Pilot targets junior/mid-level roles on select US teams; full transition expected within 12-18 months (context: Pichai's April 2026 statement that 75% of new Google code is AI-generated). **In-person round reinstated** for technical hires to combat AI-assisted cheating. Google Hiring Assessment (GHA) mandatory before the phone screen. The Googleyness & Leadership round is now part-technical. A design conversation about a real system you built, defended under scrutiny. Reports emphasize deliberately ambiguous problem framing (you must derive the problem structure) and strict production-ready-code grading at L4. No system design round below L5.

### Google Arrays and Strings

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Two Sum](https://leetcode.com/problems/two-sum) | Easy |
| 2 | [Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters) | Medium |
| 3 | [Container With Most Water](https://leetcode.com/problems/container-with-most-water) | Medium |
| 4 | [3Sum](https://leetcode.com/problems/3sum) | Medium |
| 5 | [Group Anagrams](https://leetcode.com/problems/group-anagrams) | Medium |
| 6 | [Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self) | Medium |
| 7 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium |
| 8 | [Minimum Window Substring](https://leetcode.com/problems/minimum-window-substring) | Hard |
| 9 | [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water) | Hard |
| 10 | [Find And Replace in String](https://leetcode.com/problems/find-and-replace-in-string) | Medium |
| 11 | [Maximum Points You Can Obtain from Cards](https://leetcode.com/problems/maximum-points-you-can-obtain-from-cards) | Medium |
| 12 | [Longest String Chain](https://leetcode.com/problems/longest-string-chain) | Medium |
| 13 | [Minimum Area Rectangle](https://leetcode.com/problems/minimum-area-rectangle) | Medium |
| 14 | [Detect Squares](https://leetcode.com/problems/detect-squares) | Medium |
| 15 | [Number of Unequal Triplets in Array](https://leetcode.com/problems/number-of-unequal-triplets-in-array) | Easy |
| 16 | [Pour Water](https://leetcode.com/problems/pour-water) | Medium |
| 17 | [Best Meeting Point](https://leetcode.com/problems/best-meeting-point) | Hard |
| 18 | [Decode String](https://leetcode.com/problems/decode-string) | Medium |
| 19 | [H-Index](https://leetcode.com/problems/h-index) | Medium |
| 20 | [Amount of New Area Painted Each Day](https://leetcode.com/problems/amount-of-new-area-painted-each-day) | Hard |

### Google Trees and Graphs

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium |
| 2 | [Course Schedule II](https://leetcode.com/problems/course-schedule-ii) | Medium |
| 3 | [Validate Binary Search Tree](https://leetcode.com/problems/validate-binary-search-tree) | Medium |
| 4 | [Binary Tree Maximum Path Sum](https://leetcode.com/problems/binary-tree-maximum-path-sum) | Hard |
| 5 | [Word Ladder](https://leetcode.com/problems/word-ladder) | Hard |
| 6 | [Clone Graph](https://leetcode.com/problems/clone-graph) | Medium |
| 7 | [Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree) | Hard |
| 8 | [Accounts Merge](https://leetcode.com/problems/accounts-merge) | Medium |
| 9 | [Evaluate Division](https://leetcode.com/problems/evaluate-division) | Medium |
| 10 | [Alien Dictionary](https://leetcode.com/problems/alien-dictionary) | Hard |
| 11 | [The Earliest Moment When Everyone Become Friends](https://leetcode.com/problems/the-earliest-moment-when-everyone-become-friends) | Medium |
| 12 | [Checking Existence of Edge Length Limited Paths](https://leetcode.com/problems/checking-existence-of-edge-length-limited-paths) | Hard |
| 13 | [Step-By-Step Directions From a Binary Tree Node to Another](https://leetcode.com/problems/step-by-step-directions-from-a-binary-tree-node-to-another) | Medium |
| 14 | [Swim in Rising Water](https://leetcode.com/problems/swim-in-rising-water) | Hard |
| 15 | [Path With Minimum Effort](https://leetcode.com/problems/path-with-minimum-effort) | Medium |
| 16 | [Find Leaves of Binary Tree](https://leetcode.com/problems/find-leaves-of-binary-tree) | Medium |
| 17 | [Pacific Atlantic Water Flow](https://leetcode.com/problems/pacific-atlantic-water-flow) | Medium |
| 18 | [Longest Word in Dictionary](https://leetcode.com/problems/longest-word-in-dictionary) | Medium |

### Google Dynamic Programming

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Coin Change](https://leetcode.com/problems/coin-change) | Medium |
| 2 | [Edit Distance](https://leetcode.com/problems/edit-distance) | Medium |
| 3 | [Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring) | Medium |
| 4 | [Longest Increasing Subsequence](https://leetcode.com/problems/longest-increasing-subsequence) | Medium |
| 5 | [Longest Increasing Path in a Matrix](https://leetcode.com/problems/longest-increasing-path-in-a-matrix) | Hard |
| 6 | [Burst Balloons](https://leetcode.com/problems/burst-balloons) | Hard |
| 7 | [Split Array Largest Sum](https://leetcode.com/problems/split-array-largest-sum) | Hard |
| 8 | [Longest Arithmetic Subsequence of Given Difference](https://leetcode.com/problems/longest-arithmetic-subsequence-of-given-difference) | Medium |
| 9 | [Maximum Number of Points with Cost](https://leetcode.com/problems/maximum-number-of-points-with-cost) | Medium |
| 10 | [Count Square Submatrices with All Ones](https://leetcode.com/problems/count-square-submatrices-with-all-ones) | Medium |

### Google Binary Search and Special Topics

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Search in Rotated Sorted Array](https://leetcode.com/problems/search-in-rotated-sorted-array) | Medium |
| 2 | [Koko Eating Bananas](https://leetcode.com/problems/koko-eating-bananas) | Medium |
| 3 | [Median of Two Sorted Arrays](https://leetcode.com/problems/median-of-two-sorted-arrays) | Hard |
| 4 | [Implement Trie (Prefix Tree)](https://leetcode.com/problems/implement-trie-prefix-tree) | Medium |
| 5 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium |
| 6 | [Kth Largest Element in an Array](https://leetcode.com/problems/kth-largest-element-in-an-array) | Medium |
| 7 | [Find Median from Data Stream](https://leetcode.com/problems/find-median-from-data-stream) | Hard |
| 8 | [Task Scheduler](https://leetcode.com/problems/task-scheduler) | Medium |
| 9 | [Logger Rate Limiter](https://leetcode.com/problems/logger-rate-limiter) | Easy |
| 10 | [Range Sum Query - Mutable](https://leetcode.com/problems/range-sum-query-mutable) | Medium |
| 11 | [Count of Range Sum](https://leetcode.com/problems/count-of-range-sum) | Hard |

Segment tree / BIT problems are a Google-distinctive category rarely seen at other FAANG companies.

### Google Custom Problems

| No. | Problem | Round | Description |
| --- | ------- | ----- | ----------- |
| 1 | Restaurant waitlist data structure | L4 phone screen | addGroup, group leaves anytime, seat best group for a table size by arrival order + size |
| 2 | Number of lakes on an island | L4 phone screen | Grid of water/land; given one land coordinate, count enclosed lakes (flood-fill variant) |
| 3 | Root an undirected acyclic graph as a binary tree | Phone screen | Nodes have <=3 edges; find a node that, when rooted, yields a valid binary tree |
| 4 | Alternating-color tree root | Phone screen | Graph nodes colored black/white; choose root so colors alternate per layer |
| 5 | Top-K most talkative users | L4 onsite | Parse chat-log files at given paths, return K users by word count |
| 6 | Network of teleporters | L4 onsite | Graph reachability over teleporter nodes/connections |
| 7 | Car rental bookings overlap | Coding | Batch of pickup/return times; find peak concurrent bookings |
| 8 | Guess-the-word sequence validation | Coding | Decide if guessed sequences produce a valid ordering (topological sort / cycle detection) |
| 9 | Coin collection on a board | 2026 OA | Grid DP / simulation |
| 10 | Text editor / book-keeping system | Phone screen | Implementation + language-fundamentals problem |

### Google System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Connection-degree system for a social network | Degrees of separation, graph scale |
| 2 | Near-real-time logs and metrics pipeline | Streaming ingestion |
| 3 | Task scheduler for long-running opaque video-generation jobs ("Design Sora") | Async jobs, queuing |
| 4 | Security monitoring framework for cloud infrastructure | Detection, scale |
| 5 | Design Google Drive / Maps / YouTube / Search | Classics still rotating (crawl/index/serve) |
| 6 | AI/ML system design | Increasingly woven into L5+ loops |

---

## Microsoft

> **2025-2026 Trends**: Depth over speed. Higher proportion of backtracking and linked list problems (~29% linked lists). Design-heavy follow-ups standard. **New in 2026**: Process is stable but compressed. Codility/HackerRank-style OA (2 mediums) then 4 virtual onsite rounds usually on a single day; SDE2 loops = 2-3 DSA rounds + LLD + HLD + hiring-manager round. The **"As Appropriate" (AA) round** is formalized, run by Principal EMs, routing candidates into gap-probe / behavioral deep-dive / sell-Microsoft modes; ~85% of candidates reaching AA get offers, but it retains veto power. Behavioral "growth mindset" scoring is now level-banded (L60-62 vs L63-64 vs L65+). **AI-assisted coding rounds are org-specific, not universal**: mostly CoreAI/Copilot-adjacent teams, where you get a dev environment with GitHub Copilot and are evaluated on whether you validate suggestions, keep code readable, and debug incomplete AI output. Ask your recruiter whether your loop includes it. Post-2025 layoffs: junior SDE openings compressed; AI Engineer (Foundry), M365 Copilot Developer, and Azure Architect tracks expanded, adding ML fundamentals, RAG/grounding, multi-agent orchestration, and responsible-AI scenarios.

### Microsoft Arrays and Strings

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Two Sum](https://leetcode.com/problems/two-sum) | Easy |
| 2 | [Merge Sorted Array](https://leetcode.com/problems/merge-sorted-array) | Easy |
| 3 | [Maximum Subarray](https://leetcode.com/problems/maximum-subarray) | Medium |
| 4 | [Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters) | Medium |
| 5 | [Set Matrix Zeroes](https://leetcode.com/problems/set-matrix-zeroes) | Medium |
| 6 | [Rotate Image](https://leetcode.com/problems/rotate-image) | Medium |
| 7 | [Sort Colors](https://leetcode.com/problems/sort-colors) | Medium |
| 8 | [Permutation in String](https://leetcode.com/problems/permutation-in-string) | Medium |
| 9 | [Asteroid Collision](https://leetcode.com/problems/asteroid-collision) | Medium |
| 10 | [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water) | Hard |
| 11 | [Container With Most Water](https://leetcode.com/problems/container-with-most-water) | Medium |
| 12 | [Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring) | Medium |
| 13 | [Next Permutation](https://leetcode.com/problems/next-permutation) | Medium |
| 14 | [Search in Rotated Sorted Array](https://leetcode.com/problems/search-in-rotated-sorted-array) | Medium |
| 15 | [Spiral Matrix](https://leetcode.com/problems/spiral-matrix) | Medium |
| 16 | [Word Search](https://leetcode.com/problems/word-search) | Medium |
| 17 | [First Missing Positive](https://leetcode.com/problems/first-missing-positive) | Hard |
| 18 | [Jump Game II](https://leetcode.com/problems/jump-game-ii) | Medium |
| 19 | [3Sum](https://leetcode.com/problems/3sum) | Medium |
| 20 | [Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self) | Medium |
| 21 | [String to Integer (atoi)](https://leetcode.com/problems/string-to-integer-atoi) | Medium |

### Microsoft Linked Lists

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Add Two Numbers](https://leetcode.com/problems/add-two-numbers) | Medium |
| 2 | [Merge Two Sorted Lists](https://leetcode.com/problems/merge-two-sorted-lists) | Easy |
| 3 | [Copy List with Random Pointer](https://leetcode.com/problems/copy-list-with-random-pointer) | Medium |
| 4 | [Reverse Nodes in k-Group](https://leetcode.com/problems/reverse-nodes-in-k-group) | Hard |
| 5 | [Merge k Sorted Lists](https://leetcode.com/problems/merge-k-sorted-lists) | Hard |

### Microsoft Trees and Graphs

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium |
| 2 | [Binary Tree Level Order Traversal](https://leetcode.com/problems/binary-tree-level-order-traversal) | Medium |
| 3 | [Clone Graph](https://leetcode.com/problems/clone-graph) | Medium |
| 4 | [Symmetric Tree](https://leetcode.com/problems/symmetric-tree) | Easy |
| 5 | [Cheapest Flights Within K Stops](https://leetcode.com/problems/cheapest-flights-within-k-stops) | Medium |
| 6 | [Construct Binary Tree from Preorder and Inorder Traversal](https://leetcode.com/problems/construct-binary-tree-from-preorder-and-inorder-traversal) | Medium |
| 7 | [Generate Parentheses](https://leetcode.com/problems/generate-parentheses) | Medium |
| 8 | [Letter Combinations of a Phone Number](https://leetcode.com/problems/letter-combinations-of-a-phone-number) | Medium |

### Microsoft Design and Hard Problems

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium |
| 2 | [Median of Two Sorted Arrays](https://leetcode.com/problems/median-of-two-sorted-arrays) | Hard |
| 3 | [Regular Expression Matching](https://leetcode.com/problems/regular-expression-matching) | Hard |
| 4 | [Largest Rectangle in Histogram](https://leetcode.com/problems/largest-rectangle-in-histogram) | Hard |
| 5 | [Sudoku Solver](https://leetcode.com/problems/sudoku-solver) | Hard |
| 6 | [Interleaving String](https://leetcode.com/problems/interleaving-string) | Medium |
| 7 | [Kth Largest Element in an Array](https://leetcode.com/problems/kth-largest-element-in-an-array) | Medium |
| 8 | [Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements) (asked as "Top K Frequent Error Codes") | Medium |

### Microsoft Custom Problems (2025-2026)

| No. | Problem | Category | Description |
| --- | ------- | -------- | ----------- |
| 1 | Assemble/Reconstruct DNA payload strings | Strings | Order tagged fragments to rebuild a string |
| 2 | Build a CSV Query Engine | Parsing / Design | Parse CSV and support filtered queries |
| 3 | In-Memory URL Shortener: encode/decode | Design | Classic, framed as a product story |
| 4 | Implement Memory Allocation and In-Memory Records | Systems | Allocator-style simulation |
| 5 | Implement concurrent structures and debug queue code | Concurrency / Debugging | Broken queue code supplied |
| 6 | Throughput, Rate Limiting, and LFU | Design | Combined rate-limiter + LFU cache round |
| 7 | Traverse an Org Chart by Level | Trees | N-ary level-order on employee hierarchy |
| 8 | Return Top K Open Businesses / Retain Top K Elements | Heap | Heap-under-constraints variants |
| 9 | Minimum Moves on a Grid with k-Cell Jumps | BFS | BFS with jump moves |
| 10 | Shortest path in weighted grid with constraints | Graph | Dijkstra/BFS hybrid |
| 11 | LRU Cache as a HackerRank-style product story | Design | Standard SDE2 Round-1 opener with optimization + edge-case follow-ups |

### Microsoft System Design

**LLD** (SOLID + State/Strategy patterns explicitly probed): Vending Machine, Parking Lot, Snake & Ladder, Residential Elevator Control System.

**HLD**: Distributed Key-Value Store (Redis-like); Typeahead at scale (storage + precomputation); Microsoft Teams presence service; multi-tenant rate limiter; SharePoint at scale; multi-region failover; VPN/ExpressRoute hybrid-connectivity scenarios (Azure tracks).

**AI Engineer track**: Copilot-style grounding with Microsoft Graph data to reduce hallucination; deploy/secure ML models on Azure ML; implement part of an LLM post-training/eval pipeline in Python (Copilot team "AI Exercise").

---

## LinkedIn

> **2025-2026 Trends**: The **AI-enabled coding interview is now part of the standard SWE loop**: one of the two coding rounds is replaced by an AI-assisted round on CoderPad with an AI chat panel (choice of models, typically Claude/Opus tiers). The AI **cannot edit code directly**: you paste and verify. Graded on a **4-point scale where 3 passes**, relative to other candidates; interviewers score whether you direct and verify the AI (prompt -> review -> run -> confirm), not whether you can avoid it. **Follow-ups are the real bar**: after working code, questioning pivots to concurrency/thread safety (most common), scaling behavior, malformed input, and production readiness. That's where candidates struggle. Loop: screening (often LC medium + SQL for some roles) -> onsite of 2 coding (1 AI-enabled) + system design + "craftsmanship" (code quality/engineering practices) + hiring manager. Staff loops: 3 DSA (up to LC Hard) + 2 system design + managerial. LinkedIn's classic tagged set still dominates, now wrapped with AI-era production follow-ups.

### LinkedIn Data Structure Design

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Nested List Weight Sum](https://leetcode.com/problems/nested-list-weight-sum) | Medium |
| 2 | [Nested List Weight Sum II](https://leetcode.com/problems/nested-list-weight-sum-ii) | Medium |
| 3 | [Max Stack](https://leetcode.com/problems/max-stack) | Hard |
| 4 | [All O'one Data Structure](https://leetcode.com/problems/all-oone-data-structure) | Hard |
| 5 | [Shortest Word Distance II](https://leetcode.com/problems/shortest-word-distance-ii) | Medium |
| 6 | [Design Add and Search Words Data Structure](https://leetcode.com/problems/design-add-and-search-words-data-structure) | Medium |
| 7 | [Insert Delete GetRandom O(1)](https://leetcode.com/problems/insert-delete-getrandom-o1) | Medium |
| 8 | [LFU Cache](https://leetcode.com/problems/lfu-cache) (confirmed in AI-enabled round, eviction ranking with LRU tiebreaker) | Hard |
| 9 | [Insert Delete GetRandom O(1) - Duplicates allowed](https://leetcode.com/problems/insert-delete-getrandom-o1-duplicates-allowed) | Hard |
| 10 | [Design Authentication Manager](https://leetcode.com/problems/design-authentication-manager) | Medium |
| 11 | [Serialize and Deserialize BST](https://leetcode.com/problems/serialize-and-deserialize-bst) | Medium |

### LinkedIn Trees and Graphs

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Find Leaves of Binary Tree](https://leetcode.com/problems/find-leaves-of-binary-tree) | Medium |
| 2 | [Find the Celebrity](https://leetcode.com/problems/find-the-celebrity) | Medium |
| 3 | [Lowest Common Ancestor of a BST](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-search-tree) | Medium |
| 4 | [Word Ladder](https://leetcode.com/problems/word-ladder) | Hard |
| 5 | [Generate Random Point in a Circle](https://leetcode.com/problems/generate-random-point-in-a-circle) | Medium |
| 6 | [Letter Combinations of a Phone Number](https://leetcode.com/problems/letter-combinations-of-a-phone-number) | Medium |

### LinkedIn Arrays and DP

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Can Place Flowers](https://leetcode.com/problems/can-place-flowers) | Easy |
| 2 | [Maximum Subarray](https://leetcode.com/problems/maximum-subarray) | Medium |
| 3 | [Maximum Product Subarray](https://leetcode.com/problems/maximum-product-subarray) | Medium |
| 4 | [Edit Distance](https://leetcode.com/problems/edit-distance) | Medium |
| 5 | [Decode Ways](https://leetcode.com/problems/decode-ways) | Medium |
| 6 | [House Robber II](https://leetcode.com/problems/house-robber-ii) | Medium |
| 7 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium |
| 8 | [Isomorphic Strings](https://leetcode.com/problems/isomorphic-strings) | Easy |
| 9 | [Max Consecutive Ones III](https://leetcode.com/problems/max-consecutive-ones-iii) | Medium |
| 10 | [Max Consecutive Ones II](https://leetcode.com/problems/max-consecutive-ones-ii) | Medium |
| 11 | [Paint House III](https://leetcode.com/problems/paint-house-iii) | Hard |
| 12 | [Allocate Mailboxes](https://leetcode.com/problems/allocate-mailboxes) | Hard |
| 13 | [Valid Perfect Square](https://leetcode.com/problems/valid-perfect-square) | Easy |
| 14 | [Squares of a Sorted Array](https://leetcode.com/problems/squares-of-a-sorted-array) | Easy |
| 15 | [Valid Parentheses](https://leetcode.com/problems/valid-parentheses) | Easy |

### LinkedIn Custom Problems

| No. | Problem | Category | Description |
| --- | ------- | -------- | ----------- |
| 1 | Structured data processing from scratch | AI-Enabled Round | Build classes/methods to parse JSON-like objects. AI-round staple |
| 2 | Merge Intervals design variant | AI-Enabled Round | Reframed as a data-structure-choice design problem |
| 3 | LRU Cache with production follow-ups | Design / Concurrency | Thread safety, scaling; most-reported screening problem |
| 4 | Compute point-to-segment minimum distance | Geometry | Math-flavored coding |
| 5 | Count trips from vehicle logs | Parsing / Aggregation | Log processing |
| 6 | Find index with positive suffix sums | Arrays | Prefix/suffix reasoning |
| 7 | Merge two n-ary trees by key rules | Trees | Recursive merge |

### LinkedIn System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Kafka-like distributed message queue | Partitioning, replication, ordering (Staff) |
| 2 | Flexible in-memory cache with customizable capacity + pluggable eviction (LRU/priority) | Extensible design |
| 3 | LinkedIn-scale internal notification system | Microservices + Kafka async |
| 4 | Feed ranking, messaging, job-recommendation systems | Recurring domain themes |

---

## OpenAI

> **2025-2026 Trends**: Production over puzzles. Problems drawn from a fixed bank of ~8 core challenges with progressive difficulty layers, and the bank churns (Dependency Version Finder is a new entrant). Python strongly recommended. Coding bar is non-negotiable. Interviewers expect you to "fly through" problems, candidates report typing the whole 60 minutes. **New in 2026**: (1) **Agentic coding round (beta)**: you get an existing codebase and must add features scoped "too large and complex to tackle by hand," so you are *expected* to drive an AI coding agent. This is the **only live round** where AI use is permitted, every other interview strictly prohibits it. (The take-home is the one other carve-out, and only for Applied AI roles; see below.) Not all candidates get it while in beta. (2) The 48-hour take-home is now widely reported as a **paid work trial (~$1,000)** under NDA, scoped for ~3-6 hours of work and graded like a senior engineer's PR review, **"missing test coverage" is the single most-cited rejection reason**, and a design doc explaining tradeoffs is expected. AI tooling is allowed for Applied AI roles, restricted for Core Infra/Research. (3) Official candidate guide published: final loop is 4-6 hours with 4-6 people over 1-2 days; engineering criteria are explicitly "well-designed solutions, high-quality code, optimal performance, good test coverage." Loop = 2 coding + 1 system design + behavioral + hiring manager, plus a 45-min project presentation round (deep defense of a personal project). System design interviewers push 10x/100x/1000x scaling, fault tolerance, and idempotency.

### OpenAI Core Custom Problems

These are unique to OpenAI and not standard LeetCode problems.

| No. | Problem | Difficulty | Category | Context |
| --- | ------- | ---------- | -------- | ------- |
| 1 | KV Store Serialize/Deserialize | Hard | Design / Strings | Multi-part: serialization, file persistence, multithreading, versioned store |
| 2 | CD Directory Navigation | Hard | String / Path Resolution | `cd()` with relative/absolute paths, `..`, `.`, `~`, symlink cycle detection |
| 3 | Excel/Spreadsheet Engine | Hard | Graph / Design | Cell get/set with formula dependencies, circular dependency detection |
| 4 | In-Memory Database | Hard | Database Design | `select()` with WHERE, AND, ORDER BY -- no SQL parsing |
| 5 | Resumable Iterator | Hard | Iterator / State | Stateful iterator with `getState()`/`setState()`, nested structures, async |
| 6 | Async Node Counting | Hard | Distributed / Trees | Count tree nodes using only async parent-child messaging |
| 7 | Toy Language Interpreter | Hard | Parsing / Compilers | 75-min round: lexer, parser, evaluator for variables, arithmetic, control flow |
| 8 | GPU Credit Allocation / Manager | Hard | Design / State | Add credits with expiration, auto-expire, deduct with history tracking |
| 9 | Rate Limiter with Sliding Window | Hard | Design / Algorithms | Sliding window or token bucket implementation |
| 10 | SQL Engine / Parser + Executor | Hard | Parsing / Design | Build parser + executor for basic SQL operations |
| 11 | Versioned KV Store | Hard | Design / Binary Search | Auto-incrementing versions, `get(key, version)` returns latest <= version; follow-ups: global vs per-key locks, optimistic locking, custom serialization + disk persistence |
| 12 | Dependency Version Finder (new 2026) | Medium-Hard | Iterative Refinement | Given a dependency version list + feature-support test data, find the earliest version supporting the current feature; requirements evolve as new test cases are revealed |
| 13 | Token Consumption Log Parser | Easy-Medium | Parsing | Parse an API-call log string, total token consumption per user, sort by user ID |
| 14 | Chatbot interface class with command tracking | Medium | OOP Design | Class-based chatbot interface tracking commands |
| 15 | Design a chess game | Medium | OOP Design | Classic OO design, coded live |
| 16 | Refactor nested code preserving tests | Medium | Refactoring | Restructure deeply nested code; all tests must keep passing |
| 17 | One-NN + feedforward NN from scratch | Medium | ML Coding | Implement 1-nearest-neighbor, then a basic feedforward net with activation layers |
| 18 | KL divergence / probability coding | Hard | Math / Stats Coding | KL divergence for continuous distributions; expected-iterations probability; cross-entropy minimization |

**Progressive layers reported in 2026**: *Resumable Iterator* now runs up to 6 parts (lists -> multi-file with empty files -> async/coroutines -> 2D -> 3D iterators). *CD Directory Navigation* adds `~` home-dir handling and symlink resolution with cycle detection. *GPU Credit Allocation* uses half-open intervals `[start, expiration)`, consumes soonest-expiring first (heap/queue), and must answer balance queries at an arbitrary timestamp.

### OpenAI LeetCode-Equivalent Problems

| No. | Question | Difficulty | Context |
| --- | -------- | ---------- | ------- |
| 1 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium | Inference KV cache -- most frequently reported |
| 2 | [Time Based Key-Value Store](https://leetcode.com/problems/time-based-key-value-store) | Medium | Model checkpoint storage |
| 3 | [Snapshot Array](https://leetcode.com/problems/snapshot-array) | Medium | Model state checkpointing |
| 4 | [Alien Dictionary](https://leetcode.com/problems/alien-dictionary) | Hard | Tokenizer ordering |
| 5 | [Web Crawler Multithreaded](https://leetcode.com/problems/web-crawler-multithreaded) | Medium | Training data crawling |
| 6 | [LFU Cache](https://leetcode.com/problems/lfu-cache) | Hard | Advanced caching |
| 7 | [Design Memory Allocator](https://leetcode.com/problems/design-memory-allocator) | Medium | GPU memory management |
| 8 | [Game of Life](https://leetcode.com/problems/game-of-life) | Medium | Extended to infinite board |
| 9 | [Meeting Rooms II](https://leetcode.com/problems/meeting-rooms-ii) | Medium | Interval scheduling |
| 10 | [Encode and Decode Strings](https://leetcode.com/problems/encode-and-decode-strings) | Medium | Serialization family |
| 11 | [Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree) | Hard | Data persistence |
| 12 | [Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements) | Medium | ML preprocessing |
| 13 | [Course Schedule II](https://leetcode.com/problems/course-schedule-ii) | Medium | Dependency resolution |
| 14 | [Decode String](https://leetcode.com/problems/decode-string) | Medium | String processing |
| 15 | [Word Ladder](https://leetcode.com/problems/word-ladder) | Hard | NLP transformations |

### OpenAI System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Design LLM-Powered Enterprise Search | Embeddings, vector DBs, chunking, hallucination prevention |
| 2 | Design a Real-Time Chatbot API | WebSocket vs REST, streaming, safety filters, rate limiting |
| 3 | Design a Large-Scale AI Model Serving System | Load balancing, GPU servers, autoscaling, model versioning |
| 4 | Design a Distributed Training System | Data/model parallelism, all-reduce, failure handling |
| 5 | Design a Vector Database | ANN algorithms, sharding, billions of embeddings |
| 6 | Design an Enterprise RAG System | Document ingestion, chunking, embedding, retrieval |
| 7 | Design a Rate Limiter | Token bucket, sliding window, distributed rate limiting |
| 8 | Design Slack (with 100x/1000x scaling scenarios) | Fan-out, presence, scaling pressure |
| 9 | Design the OpenAI Playground (UI through backend) | Full-stack: wireframes + API contract + storage |
| 10 | Design a GPU credits allocation system | Real-time deduction, top-ups, rate limiting, fairness across GPU nodes |
| 11 | Design a distributed job scheduler | Queuing, retries, idempotency |
| 12 | Design a payment-processing system | Idempotency, consistency |
| 13 | User profile system scaled to 100M users | Users/sessions/settings tables, batch migration logic |

### OpenAI ML and AI Technical

| No. | Topic | Category |
| --- | ----- | -------- |
| 1 | Implement scaled dot-product attention from scratch (NumPy/PyTorch) | Coding / Transformers |
| 2 | Implement full multi-head attention | Coding / Transformers |
| 3 | Debug a broken Transformer model | Debugging |
| 4 | Partition a 200B-parameter model across 2000 GPUs | Distributed Systems |
| 5 | Deploy a 70B model with low latency (quantization, MoE, continuous batching) | Inference Optimization |
| 6 | Detect and mitigate hallucinations in LLMs | Safety |
| 7 | Design red-teaming / adversarial evaluations for models | Safety / Evaluation |
| 8 | Evaluate RLHF impact on model responses | RLHF / Evaluation |
| 9 | Transformer bug-fixing in 400+ lines of PyTorch | ML Debugging |
| 10 | Debug a minimal causal LM whose loss never improves / goes NaN | ML Debugging |
| 11 | Transformer text classifier with 4 failing unit tests -- make it train and evaluate | ML Debugging |
| 12 | Implement attention from scratch in numpy / raw PyTorch tensor ops (no libraries) | Coding / Transformers |
| 13 | "Practical Engineering" round: interact with an API, parse log files, debug a broken system live | Applied Engineering |
| 14 | Graduate-level statistics round (research engineer loops) | Statistics |

**Transformer bug-fixing specifics**: planted bugs include position-embedding init, mask values, missing `loss.backward()`, and wrong `nn.Linear` dims; follow-up discussion covers KV-cache optimization.

---

## Anthropic

> **2025-2026 Trends**: CodeSignal OA (90 min) then a 4-6 hour onsite with 4-6 rounds. Python expected. Live rounds moved to **CodeSignal** (replacing Replit), screen-share via Google Meet, and code must actually run. **Split AI policy**: AI tools are strictly prohibited in all live interviews (candidates have been dropped for AI use), but **explicitly permitted on the performance take-home**. Google/Stack Overflow are allowed in live coding. Anthropic reportedly uses LLMs to analyze OA submissions for test-gaming patterns.
>
> **The performance take-home has been redesigned three times because Claude kept beating it** (Anthropic engineering blog + TechCrunch, Jan 2026): V1 (2024) was a 4-hour simulated-accelerator optimization (multicore, SIMD, VLIW); V2 (mid-2025) was cut to 2 hours after Claude Opus 4 outperformed most humans; V3 (late 2025) is a fully redesigned Zachtronics-puzzle-style constrained instruction set where you minimize instruction count with **no built-in debugging tools, building your own tooling is part of the test**. In Anthropic's words, "we no longer had a way to distinguish between the output of our top candidates and our most capable model." The original is open-sourced at [anthropics/original_performance_takehome](https://github.com/anthropics/original_performance_takehome).
>
> **Transparent question bank**: recruiters tell you which prompt family you'll get days before the round; the live-coding bank is only ~6 questions. Scheduling emails describe "a pure programming problem solving interview which doesn't benefit from memorizing standard algorithms." **OA cutoff signals**: HR reportedly states 480 as the cutoff, but community reports put the realistic bar near 600. Candidates at 540-590 report not advancing, and near-perfect scores are still rejected under holistic review. **Values/Culture round (45 min)** is universal, identical across all roles and levels, and remains the #1 failure point. NOT behavioral/STAR. It evaluates holding complexity, admitting knowledge gaps, second-order reasoning, and intellectual honesty; scripted STAR stories are the top failure mode, and measured skepticism about the mission scores better than performed enthusiasm. Prep material: Core Views on AI Safety + the Responsible Scaling Policy.

### Anthropic Core Custom Coding Problems

These are Anthropic's own custom problems. Not LeetCode. Each has multiple difficulty layers added progressively.

| No. | Problem | Difficulty | Category | Details |
| --- | ------- | ---------- | -------- | ------- |
| 1 | In-Memory Database | Hard | Design | 4 levels: SET/GET/DELETE -> filtered scans -> TTL -> backup/restore |
| 2 | Web Crawler | Hard | BFS / Concurrency | BFS crawl -> multithreaded/async optimization |
| 3 | LRU Cache (Bugfix + Extend) | Hard | Design / Debugging | Fix bugs in given code, add persistence, handle `*args`/`**kwargs` |
| 4 | Stack Trace / Profiler | Hard | Parsing / Design | Convert sampling profiler data to chronological events |
| 5 | Tokenization Engine | Hard | String / NLP | Code review, tokenize/detokenize with vocabulary coverage |
| 6 | Distributed Mode/Median | Hard | Distributed Systems | Compute statistics across 10 nodes with bandwidth constraints |
| 7 | Bank System / Bank Account | Hard | Design / Refactoring | Progressive: account creation -> merging -> cashback logic requiring redesign |
| 8 | File System Implementation | Hard | Design | Layered stages of increasing complexity |
| 9 | Package Manager | Hard | Graph / Design | Toy package manager with dependency resolution |
| 10 | Duplicate File Finder | Hard | Hashing / File System | File dedup via hashing; related to LC 609 |
| 11 | Recipe Catalog | Easy-Medium | Progressive OA | Store recipes with metadata; search by ingredient and prep time |
| 12 | Task Tracker | Medium | Progressive OA | Priority-based tasks, deadline tracking, completion reporting |
| 13 | Record Store | Hard | Progressive OA | In-memory DB extended with conditional writes and historical ("at timestamp") queries; L4 adds compression/persistence |
| 14 | Worker Mode Tracker | Medium | Distributed | Collect shard data from workers; track globally frequent values (distributed mode/median variant) |
| 15 | Profiler Trace Denoising | Hard | Algorithms | Filter short-lived calls from sampling profiler data; emit events only after N consecutive appearances |
| 16 | Parallel Word Segmentation | Hard | Concurrency | Parallelize segmentation over large datasets; task distribution, result merging, shared-memory safety |

**Progressive layers reported in 2026**: *Bank Ledger* now adds delayed cashback and spending-analytics levels. *LRU Cache* goes beyond the bugfix to demand durability, survive a process restart and restore usage order from disk. *Web Crawler* runs up to 7 follow-up levels: single-threaded BFS with `htmlParser.getUrls(url)` -> threads/processes/async -> a GIL discussion -> multi-machine scaling. *Greedy Tokenizer* uses longest-match tokenization against a vocabulary with unknown-token merging, and also appears as a code-review exercise.

### Anthropic LeetCode Practice (Mapped to Focus Areas)

| No. | Question | Difficulty | Category |
| --- | -------- | ---------- | -------- |
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
| 11 | [Count of Smaller Numbers After Self](https://leetcode.com/problems/count-of-smaller-numbers-after-self) (phone screen; O(n log n) required) | Hard | Merge Sort / BIT |

### Anthropic System Design

| No. | Question | Key Concepts |
| --- | -------- | ------------ |
| 1 | Design RLHF training pipeline | Data collection, reward model, PPO loop |
| 2 | Design distributed training system | Model parallelism, gradient sync, fault tolerance |
| 3 | Design inference optimization system | KV cache, quantization, dynamic batching |
| 4 | Design red-teaming and adversarial evaluation platform | Attack generation, defense layers, metrics |
| 5 | Design Constitutional AI feedback loop | Principle-based critique, revision chains, scalable oversight |
| 6 | Design APIs for developers to access Anthropic's models securely and efficiently | CreateCompletion/StreamCompletion, key management, usage tracking, model routing, GPU-backed serving with batching |
| 7 | Design request batching + GPU utilization under variable load | Dynamic batching, queueing |
| 8 | Design the Claude chat service | End-to-end serving |
| 9 | Design a batch preprocessing service for LLM training data | Prioritization, Kubernetes elastic scaling |
| 10 | Design evaluation pipelines and a red-teaming workflow | Safety as a first-class requirement |

Anthropic's design rounds treat the safety/moderation layer as a first-class requirement and focus on AI/ML workloads rather than "design Twitter."

### Anthropic ML and AI Safety

| No. | Topic | Category |
| --- | ----- | -------- |
| 1 | Implement attention mechanism from scratch | Coding / Transformers |
| 2 | Explain and implement Constitutional AI approach | AI Safety |
| 3 | Design RLHF training pipeline | Training / Alignment |
| 4 | Red-teaming and adversarial evaluation design | Safety / Evaluation |
| 5 | Model interpretability and mechanistic understanding | Research |
| 6 | Scaling laws and compute-optimal training | Research / Scaling |
| 7 | Implement a recent paper (often an Anthropic paper) live | Research Coding |
| 8 | Mechanistic interpretability: activation patching, steering vectors, probing | Interpretability |
| 9 | Build attention-pattern visualizations | Interpretability |
| 10 | KV-cache management and GPU memory optimization | Inference |

**Research engineer loop**: recruiter -> tech screen -> 4-5 rounds including research-coding (implement a paper), an ML-systems round, a research-fluency round, a cross-functional round, and the values round.

---

## Palantir

> **2025-2026 Trends**: Unique 4-round format (you get 3 of 4: Decomposition, System Design, Re-engineering/Debugging, Coding). Each round includes 20 min behavioral. Loop: screen -> 60-min CodePair -> 3x60-min onsite -> hiring manager. **The OA is a 3-part practical HackerRank (~90 min): one coding + one SQL + one REST API/pagination task**: not pure DSA. Graph/BFS/DFS and hash map problems dominate, wrapped in narrative prompts that require extracting requirements before coding. **AI use is strictly prohibited in interviews**: a notable divergence from the industry's 2026 drift toward AI-assisted rounds. **New in 2026**: decomposition prompts have gone AI/LLM-flavored (LLM claim summarization for an insurer, a shipment-rerouting agent, retailer demand forecasting) alongside the classics. Design rounds treat correctness and fault tolerance as first-class constraints, data integrity, access control, auditability, failure modes. **Meritocracy Fellowship** (launched 2025) is an alternative pipeline for high-school grads (SAT >= 1460 / ACT >= 33, $5,400/mo, 4 months); 22 were hired from 500+ applicants, and successful fellows interview for full-time roles without a degree.

### Palantir Coding Problems

| No. | Question | Difficulty | Category |
| --- | -------- | ---------- | -------- |
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
| 15 | [Integer to English Words](https://leetcode.com/problems/integer-to-english-words) | Hard | String / Math |
| 16 | [Minimum Time Difference](https://leetcode.com/problems/minimum-time-difference) | Medium | String / Sorting |
| 17 | [Flood Fill](https://leetcode.com/problems/flood-fill) | Easy | BFS / DFS |
| 18 | [Cheapest Flights Within K Stops](https://leetcode.com/problems/cheapest-flights-within-k-stops) | Medium | Shortest Path |
| 19 | [Word Ladder](https://leetcode.com/problems/word-ladder) | Hard | BFS / State-Space Search |
| 20 | [Best Time to Buy and Sell Stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock) | Easy | Array |

### Palantir OA Problems (2026, HackerRank 3-part)

| No. | Problem | Part | Description |
| --- | ------- | ---- | ----------- |
| 1 | Shape classes | Coding (OOP) | Circle/rectangle/square area with ceiling of result |
| 2 | Client session duration | SQL | 3-table join (CITIES/CLIENTS/SESSIONS), sum durations per city |
| 3 | Finest Food Outlets | REST API | Fetch restaurant data from a paginated endpoint, aggregate JSON |

### Palantir System Design

Palantir system design ties directly to their product domain:

| No. | Question | Key Concepts |
| --- | -------- | ------------ |
| 1 | Design multi-source data integration platform | Schema normalization, CDC, ETL/ELT pipelines |
| 2 | Design fine-grained access control for sensitive datasets | ABAC vs RBAC, row/column-level security |
| 3 | Design a knowledge graph for entity tracking | Entity resolution, ontology versioning, temporal modeling |
| 4 | Design real-time anomaly detection on streaming data | Streaming ingestion, windowing, alerting |
| 5 | Design immutable audit log with data lineage | Event sourcing, replayability |

### Palantir Unique Rounds

**Decomposition Interview** (Non-coding, most distinctive round):
- Framework: Goal -> Inputs/Outputs -> Assumptions -> Subproblems -> Tests -> Integration
- *AI-flavored prompts (new in 2026)*: an insurer wants LLM-powered claim summarization; a logistics firm wants an agent to reroute shipments; unify bank fraud detection across legacy systems; an enterprise platform for 500 data sources; retailer demand forecasting; reduce 911 response times
- *Classics still rotating*: "How would you design technology to help elderly people with poor vision cook safely?"; chess game; parking garage management; social graph with friend recommendations; infection-spread tracking; taxi dispatch; hospital patient records; smart city traffic management

**Re-engineering (Debugging) Interview**:
- Debug 500-1000 lines of pre-written code with intentional bugs and red herrings
- Examples: HashMap with incorrect if-else logic, contact tracing double-counting bug

**FDSE vs SWE differences**: FDSE interviews weight decomposition higher with Easy-Medium coding; SWE interviews have Medium-Hard coding with infrastructure-scale system design

---

## Tesla

> **2025-2026 Trends**: Greedy + string manipulation heavily tested (Reorganize String is most-asked). Prefix sum / subarray problems common. For embedded/firmware roles, expect C/C++ and real-time constraints. OA is ~85-90 min, 3 problems on Codility. **New in 2026**: take-homes have been **replaced by a ~60-min practical CoderPad screen** for many teams, and Tesla is shifting back toward in-person onsites for stronger live signal. **Googling and documentation are allowed during coding rounds; LLM/Copilot use is at interviewer discretion**: evaluators explicitly watch whether you critically review code rather than paste blindly. Questions are team-tied rather than generic LeetCode: Autopilot/firmware/energy loops add domain exercises (sensor data parsing, state machines, scheduling). Autopilot loops of up to 7 rounds reported. Difficulty across ~47 tracked problems: 8 Easy / 33 Medium / 6 Hard, with arrays+sorting the highest volume.

### Tesla Algorithms

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Reorganize String](https://leetcode.com/problems/reorganize-string) | Medium |
| 2 | [Two Sum](https://leetcode.com/problems/two-sum) | Easy |
| 3 | [Group Anagrams](https://leetcode.com/problems/group-anagrams) | Medium |
| 4 | [3Sum](https://leetcode.com/problems/3sum) | Medium |
| 5 | [Maximum Subarray](https://leetcode.com/problems/maximum-subarray) | Medium |
| 6 | [Subarray Sum Equals K](https://leetcode.com/problems/subarray-sum-equals-k) | Medium |
| 7 | [Find Pivot Index](https://leetcode.com/problems/find-pivot-index) | Easy |
| 8 | [Search in Rotated Sorted Array](https://leetcode.com/problems/search-in-rotated-sorted-array) | Medium |
| 9 | [Word Ladder](https://leetcode.com/problems/word-ladder) | Hard |
| 10 | [First Missing Positive](https://leetcode.com/problems/first-missing-positive) | Hard |
| 11 | [Minimum Window Substring](https://leetcode.com/problems/minimum-window-substring) | Hard |
| 12 | [Alien Dictionary](https://leetcode.com/problems/alien-dictionary) | Hard |
| 13 | [Minimum Area Rectangle](https://leetcode.com/problems/minimum-area-rectangle) | Medium |
| 14 | [Find Peak Element](https://leetcode.com/problems/find-peak-element) | Medium |
| 15 | [Reverse Words in a String](https://leetcode.com/problems/reverse-words-in-a-string) | Medium |
| 16 | [Palindrome Permutation](https://leetcode.com/problems/palindrome-permutation) | Easy |
| 17 | [Palindrome Linked List](https://leetcode.com/problems/palindrome-linked-list) | Easy |
| 18 | [Top K Frequent Words](https://leetcode.com/problems/top-k-frequent-words) | Medium |
| 19 | [Kth Largest Element in an Array](https://leetcode.com/problems/kth-largest-element-in-an-array) | Medium |
| 20 | [Task Scheduler](https://leetcode.com/problems/task-scheduler) | Medium |
| 21 | [Sort Colors](https://leetcode.com/problems/sort-colors) | Medium |
| 22 | [Rotate Image](https://leetcode.com/problems/rotate-image) | Medium |
| 23 | [Course Schedule II](https://leetcode.com/problems/course-schedule-ii) | Medium |
| 24 | [Merge k Sorted Lists](https://leetcode.com/problems/merge-k-sorted-lists) | Hard |
| 25 | [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water) | Hard |

### Tesla System Design

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium |
| 2 | [Implement Trie (Prefix Tree)](https://leetcode.com/problems/implement-trie-prefix-tree) | Medium |
| 3 | [Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree) | Hard |
| 4 | [Design HashMap](https://leetcode.com/problems/design-hashmap) | Easy |
| 5 | [Design Underground System](https://leetcode.com/problems/design-underground-system) | Medium |
| 6 | [Design Hit Counter](https://leetcode.com/problems/design-hit-counter) | Medium |
| 7 | Design a Rate Limiter (LLD implementation round) | Medium |

Tesla-specific system design: telemetry pipeline for vehicle data, real-time monitoring for energy systems, shortest path between Tesla chargers. Architecture rounds (1-2, weighted more for staff) are tied to the team's actual work rather than a canonical public list. Interviewers start from "what are we trying to do?" and grade requirements-gathering. Domain variants: React/frontend implementation design, backend fundamentals, and embedded/hardware-aware design with HW-SW tradeoffs.

**Tesla custom problems**: sensor data parsing (parse/validate noisy sensor streams), state machine implementation (vehicle/charging states and transitions), scheduling/simulation problems from an internal question bank, and bitwise/register exercises for firmware roles.

### Tesla Embedded Systems

For firmware/embedded roles (Autopilot, battery management, motor controllers):

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Number of 1 Bits](https://leetcode.com/problems/number-of-1-bits) | Easy |
| 2 | [Reverse Bits](https://leetcode.com/problems/reverse-bits) | Easy |
| 3 | [Single Number](https://leetcode.com/problems/single-number) | Easy |
| 4 | [Counting Bits](https://leetcode.com/problems/counting-bits) | Easy |
| 5 | [Find the Duplicate Number](https://leetcode.com/problems/find-the-duplicate-number) | Medium |
| 6 | [Sum of Two Integers](https://leetcode.com/problems/sum-of-two-integers) | Medium |

Domain-specific: interrupt-safe circular buffers in C, CAN bus protocol design, RTOS task scheduling, mutex vs. semaphore, I2C/UART/SPI protocol selection.

---

## Databricks

> **2025-2026 Trends**: OA is 4 problems in 70 minutes on CodeSignal (2 easy, 2 medium), webcam-proctored, single browser, scored on a scale "resembling a credit score, up to 850" (~30% pass rate). Onsite is **fully virtual in 2026** and standardized: 2 algorithm rounds + a **dedicated 60-min concurrency/multithreading round** (unique among tech companies, "most companies wave at the topic; Databricks makes it an entire hour") + system design + behavioral; senior/staff sometimes get a second system design round. **Small question pool, deep follow-up variations**: candidates report the same core problems (SnapshotSet, Lazy Array, House Robber variants, Tic-Tac-Toe) recycled with escalating twists, including "now distribute this with Spark" follow-ups. ML and platform engineering interviews are increasingly intertwined post-acquisitions, feature-store and Spark-internals prompts now appear in generalist SWE loops. ~25% of candidates pivot teams post-onsite.

### Databricks Algorithms and Design

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Capacity To Ship Packages Within D Days](https://leetcode.com/problems/capacity-to-ship-packages-within-d-days) | Medium |
| 2 | [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water) | Hard |
| 3 | [Max Stack](https://leetcode.com/problems/max-stack) | Hard |
| 4 | [All O'one Data Structure](https://leetcode.com/problems/all-oone-data-structure) | Hard |
| 5 | [Word Break](https://leetcode.com/problems/word-break) | Medium |
| 6 | [Rotting Oranges](https://leetcode.com/problems/rotting-oranges) | Medium |
| 7 | [All Nodes Distance K in Binary Tree](https://leetcode.com/problems/all-nodes-distance-k-in-binary-tree) | Medium |
| 8 | [Decode String](https://leetcode.com/problems/decode-string) | Medium |
| 9 | [K Closest Points to Origin](https://leetcode.com/problems/k-closest-points-to-origin) | Medium |
| 10 | [Asteroid Collision](https://leetcode.com/problems/asteroid-collision) | Medium |
| 11 | [Design Hit Counter](https://leetcode.com/problems/design-hit-counter) | Medium |
| 12 | [Time Based Key-Value Store](https://leetcode.com/problems/time-based-key-value-store) | Medium |
| 13 | [Snapshot Array](https://leetcode.com/problems/snapshot-array) | Medium |
| 14 | [Find All Anagrams in a String](https://leetcode.com/problems/find-all-anagrams-in-a-string) | Medium |
| 15 | [Cheapest Flights Within K Stops](https://leetcode.com/problems/cheapest-flights-within-k-stops) | Medium |
| 16 | [IP to CIDR](https://leetcode.com/problems/ip-to-cidr) | Medium |
| 17 | [Max Area of Island](https://leetcode.com/problems/max-area-of-island) | Medium |
| 18 | [House Robber II](https://leetcode.com/problems/house-robber-ii) | Medium |
| 19 | [Design Tic-Tac-Toe](https://leetcode.com/problems/design-tic-tac-toe) (variable board size + configurable win condition) | Medium |
| 20 | [Top K Frequent Words](https://leetcode.com/problems/top-k-frequent-words) (in a stream, under memory constraints) | Medium |
| 21 | [LRU Cache](https://leetcode.com/problems/lru-cache) (with hit-count tracking + thread safety) | Medium |
| 22 | [Binary Search Tree Iterator](https://leetcode.com/problems/binary-search-tree-iterator) | Medium |

### Databricks Custom Problems

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | **SnapshotSet / versioned iterator**: set whose iterator reflects state at creation time; later put/remove must not affect it | Hard | Design (most-reported) |
| 2 | **Lazy Array**: lazy evaluation with chained `map` operations and `indexOf` | Hard | Design |
| 3 | Revenue System, track customer revenue including referral chains; top-k filtered queries | Hard | Design |
| 4 | In-place incremental (delta) encoding, store array as diffs; follow-up: distribute with Spark | Medium-Hard | Arrays / Distributed |
| 5 | Replaying shell commands, simulate history with `cp`/`ls`/`mv`/`!<index>` | Medium | Simulation (OA) |
| 6 | SMS message splitting, split text with `<x/y>` suffixes, minimize count | Hard | Strings (OA) |
| 7 | Lamps on a number line, interval coverage counting | Medium | Intervals (OA) |
| 8 | Fibonacci Tree path finding. O(log n) connecting-path solution | Hard | Trees |
| 9 | IP firewall ALLOW/DENY rules | Medium | Bit manipulation (phone screen) |

### Databricks Concurrency (Dedicated Round)

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Print in Order](https://leetcode.com/problems/print-in-order) | Easy |
| 2 | [Print FooBar Alternately](https://leetcode.com/problems/print-foobar-alternately) | Medium |
| 3 | [Building H2O](https://leetcode.com/problems/building-h2o) | Medium |
| 4 | [The Dining Philosophers](https://leetcode.com/problems/the-dining-philosophers) | Medium |
| 5 | [Fizz Buzz Multithreaded](https://leetcode.com/problems/fizz-buzz-multithreaded) | Medium |

Custom concurrency problems also reported: **multi-threaded logger** efficiently draining a message queue (classic prompt), thread-safe logger with disk flush, **rate limiter (token bucket)** with burst probing ("client sends 10x their limit in the first 100ms of the window"), producer-consumer with condition variables.

### Databricks System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Bookstore: return the cheapest copy of a book across 50-200 seller integrations within a 10-20s latency budget | Long-running Databricks staple |
| 2 | Throttle system: rate limiting + circuit breaker to prevent cascading failures | Resilience |
| 3 | Payment gateway: card routing, validation APIs, failure handling, load estimation | Distributed systems |
| 4 | Dependency-aware job scheduler for Spark workloads | Executor cores/memory as first-class constraints |
| 5 | Multi-tenant feature store at 50K QPS with sub-50ms p99 | ML platform round |
| 6 | Add delete + trash functionality to a database | New grad onsite |
| 7 | Spark internals as design: "what happens when you join two billion-row DataFrames"; Delta Lake transaction log vs Iceberg/Hudi | Domain depth |

---

## Stripe

> **2025-2026 Trends**: Stripe does NOT use traditional LeetCode-style interviews. Problems model real engineering work -- payment processing, debugging, API integration. Process spans 7-9 weeks. Unique rounds: Bug Squash (debug a GitHub repo with real issues), Integration (build with Stripe API), API Design (REST resource modeling, idempotency, versioning). Production code quality valued over algorithmic cleverness -- O(n^2) is fine if code is clean. Speed is NOT measured. **New in 2026**: the new-grad OA changed to a **single 60-minute multi-part question on HackerRank**: "measuring true coding ability with one question", with state-machine modeling and case-intensive hidden tests (some tracks still see 2 questions / 90 min). **Integration round rules clarified: web/docs search is allowed, but AI coding assistants are NOT permitted**; the round gives you a private GitHub repo + a real API, and you expose endpoints and handle paginated JSON. Bug Squash is unchanged as the signature round but now focuses sharply on financial-logic bugs: race conditions, missing idempotency checks, non-atomic check-then-act, and unvalidated refund logic, roughly 5-7 bugs in ~200 lines.

### Stripe Coding and Integration

Stripe avoids LeetCode; these are the closest **analogues** to reported Stripe problems, useful for pattern practice, not literal questions.

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Two Sum](https://leetcode.com/problems/two-sum) | Easy |
| 2 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium |
| 3 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium |
| 4 | [Design Hit Counter](https://leetcode.com/problems/design-hit-counter) | Medium |
| 5 | [Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements) | Medium |
| 6 | [Subarray Sum Equals K](https://leetcode.com/problems/subarray-sum-equals-k) | Medium |
| 7 | [Time Based Key-Value Store](https://leetcode.com/problems/time-based-key-value-store) | Medium |
| 8 | [Course Schedule](https://leetcode.com/problems/course-schedule) | Medium |
| 9 | [Coin Change](https://leetcode.com/problems/coin-change) | Medium |
| 10 | [Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree) | Hard |
| 11 | [Sliding Window Maximum](https://leetcode.com/problems/sliding-window-maximum) | Hard |
| 12 | [Evaluate Division](https://leetcode.com/problems/evaluate-division), analogue of the multi-hop currency-conversion problem | Medium |
| 13 | [Invalid Transactions](https://leetcode.com/problems/invalid-transactions), analogue of the fraud-detection OA | Medium |
| 14 | [Single-Threaded CPU](https://leetcode.com/problems/single-threaded-cpu), analogue of the subscription-notification scheduler | Medium |
| 15 | [Task Scheduler](https://leetcode.com/problems/task-scheduler), analogue of store-closing-time penalty ordering | Medium |
| 16 | [LFU Cache](https://leetcode.com/problems/lfu-cache), analogue of the duplicate-request/idempotency store | Hard |

### Stripe Bug Squash and API Design

**Custom Problems (unique to Stripe)**

| No. | Problem | Category | Description |
| --- | ------- | -------- | ----------- |
| 1 | **Accept-Language header parser** | Parsing | Parse q-values, sort by quality; the long-standing Stripe screen, still reported in 2026 |
| 2 | **Currency conversion string parsing** | Parsing / Graph | `"USD:CAD:DHL:5,USD:GBP:FEDX:10"`; part 2: multi-hop conversion; part 3: best rate over all paths |
| 3 | Invoice Reconciliation | Data Processing | Parse CSV of transactions, filter by status, output totals per user; match payments to invoices on memo lines |
| 4 | Request Deduplication | Integration | Build an idempotent request handler preventing duplicate charges |
| 5 | Webhook Handler Debug | Bug Squash | Find and fix bugs in a failing webhook handler with unit tests |
| 6 | API Response Parser | Bug Squash | Debug a parser that silently drops fields |
| 7 | Payment Retry Logic | Integration | Implement retry logic with exponential backoff |
| 8 | Shipping Cost Calculator | Multi-part | Multi-carrier business-logic simulation with extensibility follow-ups |
| 9 | Card range obfuscation | OA | Merge overlapping card-number ranges then mask digits |
| 10 | Fraud detection stream | OA | CHARGE/DISPUTE events, per-MCC fraud thresholds, real-time flagging |
| 11 | Subscription notification scheduler | OA | Start/interval/count, chronological output |
| 12 | CSV parse + validate (4 parts) | Onsite | Headers, row values, cross-column deps, circular dependency detection via graph |
| 13 | Atlas company name check | OA | Validation + blacklist |
| 14 | Integration round task | Integration | Private repo + docs: expose names/emails via a CLI endpoint, consume a paginated API, pick optimal endpoints from the API surface |

**System Design**: Stripe's webhook delivery system (reliability while minimizing duplicate delivery, idempotency, retries, exactly-once reasoning); distributed API rate limiter handling burst traffic; payment system with idempotency and exactly-once semantics; fraud-detection pipeline (Radar-like); multi-currency payment routing; design an HTTP server. Domain knowledge expected: PCI compliance, idempotency patterns, double-entry bookkeeping.

---

## NVIDIA

> **2025-2026 Trends**: Most strategically central tech company in 2026 due to AI infrastructure dominance. Emphasizes performance awareness over generalist coding. After solving baseline, expect follow-ups: "How does this behave under memory pressure? What's the cache miss profile? How would you parallelize across 10,000 threads?" C++ essential for systems/GPU roles; Python acceptable for ML/infra. Difficulty: 8 Easy, 29 Medium, 9 Hard across 46 tracked problems. **New in 2026**: loops are team-scoped with genuine-medium coding and a **"build from scratch" preference: interviewers prefer you avoid built-in library functions**. Recruiter screen -> 1-2 phone screens -> 4-6 interview virtual onsite over 6-8 weeks. Candidates report bespoke variants over tagged problems ("brushing up on NVIDIA classification problems on LeetCode wasn't particularly helpful"). Classic problems now get systems extensions. LRU Cache follow-ups ask you to make it thread-safe with a read-write lock (and why RW lock vs mutex), or relate it to GPU memory caching semantics. **AI-infra system design is the new senior bar**: batch inference APIs on GPU clusters, tensor+pipeline parallelism across H100s, and naming TensorRT-LLM/vLLM tradeoffs. New grad rounds increasingly mix one PyTorch problem + one LC medium.

### NVIDIA Algorithms

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Maximum Number of Events That Can Be Attended](https://leetcode.com/problems/maximum-number-of-events-that-can-be-attended) | Medium |
| 2 | [Min Stack](https://leetcode.com/problems/min-stack) | Medium |
| 3 | [Clone Graph](https://leetcode.com/problems/clone-graph) | Medium |
| 4 | [K Closest Points to Origin](https://leetcode.com/problems/k-closest-points-to-origin) | Medium |
| 5 | [Random Pick with Weight](https://leetcode.com/problems/random-pick-with-weight) | Medium |
| 6 | [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water) | Hard |
| 7 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium |
| 8 | [Rotate Image](https://leetcode.com/problems/rotate-image) | Medium |
| 9 | [Word Break](https://leetcode.com/problems/word-break) | Medium |
| 10 | [Shortest Path in Binary Matrix](https://leetcode.com/problems/shortest-path-in-binary-matrix) | Medium |
| 11 | [Longest Increasing Path in a Matrix](https://leetcode.com/problems/longest-increasing-path-in-a-matrix) | Hard |
| 12 | [Expression Add Operators](https://leetcode.com/problems/expression-add-operators) | Hard |
| 13 | [Word Ladder II](https://leetcode.com/problems/word-ladder-ii) | Hard |
| 14 | [Bus Routes](https://leetcode.com/problems/bus-routes) | Hard |
| 15 | [Making A Large Island](https://leetcode.com/problems/making-a-large-island) | Hard |
| 16 | [Special Binary String](https://leetcode.com/problems/special-binary-string) | Hard |
| 17 | [LRU Cache](https://leetcode.com/problems/lru-cache) (thread-safe RW-lock extension) | Medium |
| 18 | [Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters) | Medium |
| 19 | [Maximum Binary Tree](https://leetcode.com/problems/maximum-binary-tree) | Medium |
| 20 | [Merge k Sorted Lists](https://leetcode.com/problems/merge-k-sorted-lists) | Hard |
| 21 | [Group Anagrams](https://leetcode.com/problems/group-anagrams) | Medium |
| 22 | [Valid Parentheses](https://leetcode.com/problems/valid-parentheses) | Easy |
| 23 | [Best Time to Buy and Sell Stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock) | Easy |
| 24 | [Two Sum](https://leetcode.com/problems/two-sum) | Easy |
| 25 | [Course Schedule](https://leetcode.com/problems/course-schedule) | Medium |
| 26 | [Rotting Oranges](https://leetcode.com/problems/rotting-oranges) | Medium |
| 27 | [Coin Change](https://leetcode.com/problems/coin-change) | Medium |
| 28 | [Search in Rotated Sorted Array](https://leetcode.com/problems/search-in-rotated-sorted-array) | Medium |
| 29 | [Reverse Linked List](https://leetcode.com/problems/reverse-linked-list) | Easy |

### NVIDIA Custom Problems (2026)

| No. | Problem | Category | Description |
| --- | ------- | -------- | ----------- |
| 1 | Polynomial multiplication API in C | Systems / API Design | Design and implement the API from scratch |
| 2 | Temperature spike detection | Arrays / Streaming | Find spikes from (timestamp, CPU temp) pairs |
| 3 | Minimum sum after K operations | Greedy / Heap | Greedy-heap variant |
| 4 | Log processing/aggregation by HTTP status code | Hashing | Aggregate logs by status |
| 5 | Tree planting constraint satisfaction | Graph / Constraints | Constraint problem |
| 6 | Thread-safe LRU with read-write lock | Concurrency | Why RW lock vs mutex; GPU-cache semantics follow-up |
| 7 | PyTorch coding problem + LC medium in one round | ML / DSA | New grad format |

### NVIDIA GPU and Systems

**CUDA/GPU-Specific Problems**

| No. | Problem | Category | Description |
| --- | ------- | -------- | ----------- |
| 1 | CUDA Memory Optimization | GPU Programming | Optimize matrix operations for GPU memory hierarchy |
| 2 | CUDA Kernel Fusion | Performance | Fuse Transformer attention operations into efficient kernels |
| 3 | Matrix Multiplication Optimization | Parallel Computing | Implement GEMM considering cache locality and thread scheduling |
| 4 | Sorting Algorithm Parallelization | GPU Computing | Implement parallel sort analyzing stability and parallelizability |
| 5 | Memory Coalescing Analysis | CUDA | Fix uncoalesced memory access patterns in warp execution |
| 6 | Thread Synchronization | Concurrency | Implement barrier synchronization across thread blocks |
| 7 | Multi-GPU Communication | Distributed | Optimize communication patterns in distributed training |

**Key topics**: GPU memory architecture (SRAM vs HBM), CUDA thread hierarchy (threads/warps/blocks/grids), KV-cache optimization, LoRA fine-tuning, Mixture-of-Experts, beam search. **CUDA conceptual drills (2026)**: explain memory coalescing; profile a slow kernel with Nsight Compute; fix uncoalesced access / bank conflicts / thread divergence; make a kernel scale across GPU architectures; occupancy analysis.

### NVIDIA System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Design a batch inference API for a GPU cluster | Queuing, batching under constraints, GPU-memory-aware load balancing (most-reported) |
| 2 | Design distributed inference at 10,000 RPS with sub-100ms P99 across H100s | Tensor parallelism intra-node via NVLink, pipeline parallelism across nodes via InfiniBand |
| 3 | Serve multiple LLMs efficiently on one GPU cluster | Multi-model serving |
| 4 | Multi-tenant inference platform with KV-cache sharing and fair scheduling | Isolation, fairness |
| 5 | HPC data pipelines, distributed storage, real-time telemetry | Role-dependent |

---

## Uber

> **2025-2026 Trends**: Interviews reflect product domain -- routing, dispatch, surge pricing map to graph traversal, streaming aggregation, sliding-window patterns. OA: 4 problems in 70-90 minutes on CodeSignal (easy/medium arrays + harder graph/DP), followed by a 4-6 round onsite. Code readability explicitly evaluated. L5A (Senior): 5 rounds total with elimination Round 0 (LeetCode Medium). Difficulty: 7% Easy, 73% Medium, 20% Hard. **New in 2026**: **machine-coding / LLD rounds are the differentiator at senior levels**: coding is the primary gate while system-design quality decides leveling (L5a/L5b/Senior/Staff). Original non-LeetCode problems appear in "Hack2Hire" assessments. Questions cluster into four families: graphs/BFS-DFS, sliding window/two pointers, heaps/streaming, and cache/design, with domain-flavored twists (quadtrees for geo points, rate limiters, autocomplete) rather than pure textbook problems. Frequent themes: Uber Eats cart pricing, geo heatmaps, surge, restaurant recommendation. No evidence Uber allows AI tools in interviews as of mid-2026.

### Uber Algorithms

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Maximize Amount After Two Days of Conversions](https://leetcode.com/problems/maximize-amount-after-two-days-of-conversions) | Medium |
| 2 | [Bus Routes](https://leetcode.com/problems/bus-routes) | Hard |
| 3 | [Alien Dictionary](https://leetcode.com/problems/alien-dictionary) | Hard |
| 4 | [Number of Islands II](https://leetcode.com/problems/number-of-islands-ii) | Hard |
| 5 | [Design Hit Counter](https://leetcode.com/problems/design-hit-counter) | Medium |
| 6 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium |
| 7 | [Spiral Matrix](https://leetcode.com/problems/spiral-matrix) | Medium |
| 8 | [Word Search](https://leetcode.com/problems/word-search) | Medium |
| 9 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium |
| 10 | [Evaluate Division](https://leetcode.com/problems/evaluate-division) | Medium |
| 11 | [Random Pick with Weight](https://leetcode.com/problems/random-pick-with-weight) | Medium |
| 12 | [Find Median from Data Stream](https://leetcode.com/problems/find-median-from-data-stream) | Hard |
| 13 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium |
| 14 | [Meeting Rooms II](https://leetcode.com/problems/meeting-rooms-ii) | Medium |
| 15 | [Longest Subarray With Absolute Diff <= Limit](https://leetcode.com/problems/longest-continuous-subarray-with-absolute-diff-less-than-or-equal-to-limit) | Medium |
| 16 | [Course Schedule II](https://leetcode.com/problems/course-schedule-ii) | Medium |
| 17 | [Group Anagrams](https://leetcode.com/problems/group-anagrams) | Medium |
| 18 | [Kth Smallest Element in a BST](https://leetcode.com/problems/kth-smallest-element-in-a-bst) (O(1)-space Morris-traversal follow-up at L5+) | Medium |
| 19 | [Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree) | Hard |
| 20 | [Design Search Autocomplete System](https://leetcode.com/problems/design-search-autocomplete-system) (as "Implement Store Autocomplete", Uber Eats framing) | Hard |

### Uber Custom Problems (Machine Coding)

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | Thread-Safe Token-Bucket Rate Limiter | Hard | Concurrency (Senior+) |
| 2 | Expiry Counter, counter whose entries expire over time (TTL-based driver sessions) | Medium | Design |
| 3 | Geo Heatmap builder, aggregate ride pings into a city heatmap | Medium-Hard | Geo / Aggregation |
| 4 | Driver-rider matching engine | Hard | Design |
| 5 | Surge pricing calculator (real-time supply/demand) | Hard | Design |
| 6 | Referral Revenue Tracker | Medium | Design |
| 7 | Simulate a Rank-Based Tournament | Medium | Frontend machine coding |
| 8 | Deep Equality of Two Records, write `deepEquals` for nested records | Medium | Recursion |
| 9 | Sort a String of Clothing Sizes, custom comparator ("XS < S < M") | Easy-Medium | Sorting (new grad) |
| 10 | Find Earliest Full Connectivity Timestamp | Medium | Union-Find |
| 11 | Cache Eviction + Seat Assignment (two-part) | Medium-Hard | Design |
| 12 | Adaptive bitrate selector | Medium | Streaming |

### Uber System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Design a Ride-Hailing System | Distributed concurrency, real-time updates, consistency |
| 2 | Design Real-Time Surge Pricing Engine | Millions of GPS pings/sec, supply vs demand, 30-second multiplier |
| 3 | Design Location Tracking System | Millions of location updates/sec for drivers and riders |
| 4 | Design Notification System at Scale | Push notifications, SMS, emails for ride updates |
| 5 | Design ETA Prediction Service | ML-based arrival time estimation |
| 6 | Design a simplified global food-delivery marketplace | Merchant registration + restaurant management; Uber Eats cart pricing |
| 7 | Design a backend for a daily puzzle platform | Reported 2026 prompt |
| 8 | Model-drift monitoring for pricing; real-time analytics dashboard for city ops | ML / analytics |

---

## ByteDance / TikTok

> **2025-2026 Trends**: Among the most technically demanding interviews. Baseline is Medium, Hard is frequent. 2-3 problems per round (vs 1-2 at Google/Meta) -- speed matters. Interviewers write their own problems and progressively mutate them mid-round. Compile-ready, bug-free code expected (not pseudocode). Acceptance rate estimated at 1-2%. Max 2 applications allowed. **New in 2026**: the OA was overhauled, switched from HackerRank to **CodeSignal**, multiple-choice questions removed entirely, now **4 pure coding problems in 70-90 min** (down from ~120 in 2025), with strict proctoring (camera on, screen share, no leaving the window). **AI tools are explicitly banned** in coding assessments and technical interviews, violations mean immediate disqualification. Questions are increasingly scenario-wrapped (file systems, server infrastructure, data pipelines) instead of abstract puzzles, with live coding blended into system-design thinking. New OA emphasis on combinatorics. The hiring-manager round can include an LC-Hard DP under a strict clock, one candidate reported "two LeetCode hard DP questions in one hour." Fresh-grad rounds still include CS trivia (OS, networking, DB).

### ByteDance Algorithms

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Implement Queue using Stacks](https://leetcode.com/problems/implement-queue-using-stacks) | Easy |
| 2 | [Daily Temperatures](https://leetcode.com/problems/daily-temperatures) | Medium |
| 3 | [Merge k Sorted Lists](https://leetcode.com/problems/merge-k-sorted-lists) | Hard |
| 4 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium |
| 5 | [Max Consecutive Ones III](https://leetcode.com/problems/max-consecutive-ones-iii) | Medium |
| 6 | [Sliding Window Maximum](https://leetcode.com/problems/sliding-window-maximum) | Hard |
| 7 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium |
| 8 | [Binary Tree Maximum Path Sum](https://leetcode.com/problems/binary-tree-maximum-path-sum) | Hard |
| 9 | [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water) | Hard |
| 10 | [3Sum](https://leetcode.com/problems/3sum) | Medium |
| 11 | [Longest Valid Parentheses](https://leetcode.com/problems/longest-valid-parentheses) | Hard |
| 12 | [N-Queens](https://leetcode.com/problems/n-queens) | Hard |
| 13 | [Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree) | Hard |
| 14 | [Coin Change](https://leetcode.com/problems/coin-change) | Medium |
| 15 | [Regular Expression Matching](https://leetcode.com/problems/regular-expression-matching) | Hard |
| 16 | [Longest Increasing Path in a Matrix](https://leetcode.com/problems/longest-increasing-path-in-a-matrix) | Hard |
| 17 | [Minimum Difference in Sums After Removal of Elements](https://leetcode.com/problems/minimum-difference-in-sums-after-removal-of-elements) | Hard |
| 18 | [Search in Rotated Sorted Array](https://leetcode.com/problems/search-in-rotated-sorted-array) | Medium |
| 19 | [Kth Largest Element in an Array](https://leetcode.com/problems/kth-largest-element-in-an-array) | Medium |
| 20 | [Course Schedule II](https://leetcode.com/problems/course-schedule-ii) | Medium |
| 21 | [Gas Station](https://leetcode.com/problems/gas-station) | Medium |
| 22 | [The kth Factor of n](https://leetcode.com/problems/the-kth-factor-of-n) | Medium |
| 23 | [Zero Array Transformation I](https://leetcode.com/problems/zero-array-transformation-i) | Medium |
| 24 | [Maximum Area Rectangle With Point Constraints I](https://leetcode.com/problems/maximum-area-rectangle-with-point-constraints-i) | Medium |
| 25 | [Maximize Amount After Two Days of Conversions](https://leetcode.com/problems/maximize-amount-after-two-days-of-conversions) | Medium |
| 26 | [Count Unhappy Friends](https://leetcode.com/problems/count-unhappy-friends) | Medium |
| 27 | [Continuous Subarray Sum](https://leetcode.com/problems/continuous-subarray-sum) | Medium |
| 28 | [Number of Islands II](https://leetcode.com/problems/number-of-islands-ii) | Hard |
| 29 | [K Inverse Pairs Array](https://leetcode.com/problems/k-inverse-pairs-array) | Hard |
| 30 | [Sliding Window Median](https://leetcode.com/problems/sliding-window-median) | Hard |
| 31 | [Basic Calculator II](https://leetcode.com/problems/basic-calculator-ii) | Medium |
| 32 | [The Maze](https://leetcode.com/problems/the-maze) | Medium |
| 33 | [Decode Ways II](https://leetcode.com/problems/decode-ways-ii) | Hard |

### ByteDance Custom Problems

| No. | Problem | Category | Description |
| --- | ------- | -------- | ----------- |
| 1 | GPU Resource Management | Design / Scheduling | Job queue + scheduler + resource monitor with fairness and bin-packing |
| 2 | Server Investment | Optimization | New 2026 OA problem |
| 3 | Round Robin Load Balancer | Simulation | New 2026 OA problem |
| 4 | Map Async Limit | Frontend / Async | Implement async map with a concurrency limit |
| 5 | Middleware composition | Frontend | Koa/Express-style `compose()` implementation |
| 6 | Implement `bind` with `new` support | Frontend | `Function.prototype.bind` polyfill handling constructor calls |
| 7 | Video chunk scheduler | Design | Streaming domain |
| 8 | Hashtag trend detector | Streaming | Sliding window on streams |
| 9 | Comment tree flattening | Trees | Social domain |
| 10 | Content moderation priority queue | Heap | Moderation domain |
| 11 | Video deduplication via hashing | Hashing | Content dedup |
| 12 | Live viewer count at billion scale | Distributed | Counting at scale |

### ByteDance System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Design TikTok "For You" Page | Two-phase recommendation: candidate generation + ranking |
| 2 | Design Real-Time Live Streaming System | Billion-scale concurrent users |
| 3 | Design Content Moderation Pipeline | ML-based automated moderation at scale |
| 4 | Design Social Graph Service | Following/follower relationships, efficient traversal |
| 5 | Design Ad Serving Platform | Real-time bidding and targeting |

---

## Airbnb

> **2025-2026 Trends**: **No pseudocode, code must actually run and pass test cases** in the 45-60 min CoderPad screen (or HackerRank/CodeSignal OA). This remains Airbnb's most distinctive coding-round rule. **Hardest difficulty skew among peers**: ~33% of reported problems are Hard, with heavy DP and simulation emphasis. Problems arrive dressed as product features, interval merging framed as overlapping reservation windows, tree path sums with depth constraints. **Core values and cross-functional rounds are true gates**, not chats: dedicated rounds on Belonging / "Be a Host", then hiring-committee review. No evidence Airbnb permits AI tools in interviews.

### Airbnb Algorithms

| No. | Question | Difficulty | Category |
| --- | -------- | ---------- | -------- |
| 1 | [Text Justification](https://leetcode.com/problems/text-justification) | Hard | String Simulation |
| 2 | [Maximum Profit in Job Scheduling](https://leetcode.com/problems/maximum-profit-in-job-scheduling) | Hard | DP + Binary Search |
| 3 | [Palindrome Pairs](https://leetcode.com/problems/palindrome-pairs) | Hard | Trie / Hash + String |
| 4 | [Flatten 2D Vector](https://leetcode.com/problems/flatten-2d-vector) | Medium | Iterator Design |
| 5 | [Combination Sum](https://leetcode.com/problems/combination-sum) | Medium | Backtracking |
| 6 | [Smallest Common Region](https://leetcode.com/problems/smallest-common-region) | Medium | Hash / LCA |
| 7 | [Maximum Candies You Can Get from Boxes](https://leetcode.com/problems/maximum-candies-you-can-get-from-boxes) | Hard | BFS |
| 8 | [Pour Water](https://leetcode.com/problems/pour-water) | Medium | Simulation (Airbnb signature) |
| 9 | [Alien Dictionary](https://leetcode.com/problems/alien-dictionary) | Hard | Topological Sort |
| 10 | [Cheapest Flights Within K Stops](https://leetcode.com/problems/cheapest-flights-within-k-stops) | Medium | BFS / Bellman-Ford |
| 11 | [Sliding Puzzle](https://leetcode.com/problems/sliding-puzzle) | Hard | BFS State Search |
| 12 | [Design Excel Sum Formula](https://leetcode.com/problems/design-excel-sum-formula) | Hard | Design / Topological |
| 13 | [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water) | Hard | Two Pointers |
| 14 | [IP to CIDR](https://leetcode.com/problems/ip-to-cidr) | Medium | Bit Manipulation |
| 15 | [Employee Free Time](https://leetcode.com/problems/employee-free-time) | Hard | Intervals / Heap |
| 16 | [Simple Bank System](https://leetcode.com/problems/simple-bank-system) | Medium | Design / Simulation |
| 17 | [Word Search II](https://leetcode.com/problems/word-search-ii) | Hard | Trie + Backtracking |
| 18 | [Mini Parser](https://leetcode.com/problems/mini-parser) | Medium | Stack Parsing |
| 19 | [Regular Expression Matching](https://leetcode.com/problems/regular-expression-matching) | Hard | DP |

**Custom problems**: Boxes and Candies (custom optimization, paired with Alien Dictionary in a phone round); reservation-window merging (Merge Intervals reskinned as overlapping guest bookings); binary tree path sums with a depth constraint.

### Airbnb System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Design a booking/reservation system | Time-based availability modeling, strict payment correctness, consistency boundaries, caching-vs-freshness |
| 2 | Design geo-aware search + ranking for listings at scale | Search / ranking |
| 3 | Design a notification service | Fan-out, delivery |
| 4 | Design a recommendation engine | ML / ranking |
| 5 | Design a payment processing flow | Consistency, idempotency |

---

## DoorDash

> **2025-2026 Trends**: DoorDash **publicly announced it is rebuilding its engineering interviews around AI**. The new format is a **60-min AI-assisted working session on your own machine/IDE**: Cursor, Claude Code, or Codex free tiers suffice, and all agent features are allowed. You're evaluated on pragmatic tradeoffs, turning ambiguity into a plan, minimal-repro validation, and narrating your reasoning. **The AI policy is transitional**: traditional algorithm rounds still ban AI use, while the new working-session round mandates it. 2026 loop: **CodeCraft** round (build a small business module from requirements, then extend as requirements are added), a dedicated **Debugging** round (find subtle bugs in an unfamiliar codebase, uninitialized maps, null pointers), System Design (60-75 min, logistics-centric), and Behavioral. Hiring has been decentralized since ~2025, so round mix varies by team.

### DoorDash Algorithms

| No. | Question | Difficulty | Category |
| --- | -------- | ---------- | -------- |
| 1 | [Walls and Gates](https://leetcode.com/problems/walls-and-gates) | Medium | Multi-source BFS (DashMart framing) |
| 2 | [Shortest Distance from All Buildings](https://leetcode.com/problems/shortest-distance-from-all-buildings) | Hard | Multi-source BFS |
| 3 | [01 Matrix](https://leetcode.com/problems/01-matrix) | Medium | Multi-source BFS |
| 4 | [Maximum Profit in Job Scheduling](https://leetcode.com/problems/maximum-profit-in-job-scheduling) | Hard | DP + Binary Search |
| 5 | [Binary Tree Maximum Path Sum](https://leetcode.com/problems/binary-tree-maximum-path-sum) | Hard | Tree DP |
| 6 | [Basic Calculator](https://leetcode.com/problems/basic-calculator) | Hard | Stack Parsing |
| 7 | [Longest Increasing Path in a Matrix](https://leetcode.com/problems/longest-increasing-path-in-a-matrix) | Hard | DFS + Memo |
| 8 | [Koko Eating Bananas](https://leetcode.com/problems/koko-eating-bananas) | Medium | Binary Search on Answer |
| 9 | [Search Suggestions System](https://leetcode.com/problems/search-suggestions-system) | Medium | Trie / Sorting (store search) |
| 10 | [Find K Closest Elements](https://leetcode.com/problems/find-k-closest-elements) | Medium | Binary Search + Two Pointers |
| 11 | [Ways to Make a Fair Array](https://leetcode.com/problems/ways-to-make-a-fair-array) | Medium | Prefix Sums |
| 12 | [Check if One String Swap Can Make Strings Equal](https://leetcode.com/problems/check-if-one-string-swap-can-make-strings-equal) | Easy | String (phone-screen warmup) |
| 13 | [Largest Rectangle in Histogram](https://leetcode.com/problems/largest-rectangle-in-histogram) | Hard | Monotonic Stack |
| 14 | [Making A Large Island](https://leetcode.com/problems/making-a-large-island) | Hard | Union-Find / DFS |
| 15 | [Design HashMap](https://leetcode.com/problems/design-hashmap) | Easy | Design |
| 16 | [Jump Game](https://leetcode.com/problems/jump-game) | Medium | Greedy / DP |
| 17 | [Longest Common Prefix](https://leetcode.com/problems/longest-common-prefix) | Easy | String |

### DoorDash AI-Assisted and Custom Rounds

| No. | Problem | Round | Description |
| --- | ------- | ----- | ----------- |
| 1 | Nearest DashMart | Coding | City grid with open/blocked roads and DashMarts; compute distance to the closest DashMart (multi-source BFS) |
| 2 | Dasher pay module with rule stacking | CodeCraft | Implement payment logic layering base pay, boosts, and tips per changing requirements |
| 3 | Support-ticket workflow automation engine | AI Working Session | Build an engine automating the self-help menu for tickets like "my order arrived late" |
| 4 | Unfamiliar multi-file codebase with planted bugs | Debugging | Fix bugs + discuss testing and production readiness |

### DoorDash System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Design Dasher dispatch/matching | Geo-hashing, sharding |
| 2 | Design real-time Dasher location tracking; ETA estimation | Streaming, ML |
| 3 | Design DoorDash end-to-end (order -> matching -> dispatch -> ETA) | Full system |
| 4 | Design an order status notification system; item review & rating system | Fan-out, storage |
| 5 | Ingest donations and serve rolling 3-day totals | Streaming aggregation |
| 6 | Payment consistency | Idempotency keys, reconciliation/audit trails, webhook handling, async decoupling to prevent double charges |

---

## Topic-wise Questions

### Array Manipulation

| No. | Question | Difficulty | Companies |
| --- | -------- | ---------- | --------- |
| 1 | [Two Sum](https://leetcode.com/problems/two-sum) | Easy | All |
| 2 | [Container With Most Water](https://leetcode.com/problems/container-with-most-water) | Medium | Google, Amazon |
| 3 | [3Sum](https://leetcode.com/problems/3sum) | Medium | All |
| 4 | [Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self) | Medium | Meta, Apple, Amazon |
| 5 | [Subarray Sum Equals K](https://leetcode.com/problems/subarray-sum-equals-k) | Medium | Meta, Amazon |
| 6 | [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water) | Hard | Amazon, Netflix, Google |
| 7 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium | All |
| 8 | [Sliding Window Maximum](https://leetcode.com/problems/sliding-window-maximum) | Hard | Amazon, Google |
| 9 | [Next Permutation](https://leetcode.com/problems/next-permutation) | Medium | Meta, Microsoft, Cerebras |
| 10 | [First Missing Positive](https://leetcode.com/problems/first-missing-positive) | Hard | Meta, Microsoft, Tesla |
| 11 | [Minimum Area Rectangle](https://leetcode.com/problems/minimum-area-rectangle) | Medium | Google, Tesla, Waymo |
| 12 | [Continuous Subarray Sum](https://leetcode.com/problems/continuous-subarray-sum) | Medium | Meta, ByteDance, Cerebras |

### Trees and Graphs

| No. | Question | Difficulty | Companies |
| --- | -------- | ---------- | --------- |
| 1 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium | All |
| 2 | [Course Schedule II](https://leetcode.com/problems/course-schedule-ii) | Medium | Google, Amazon, Netflix, Tesla, Uber |
| 3 | [Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree) | Hard | All |
| 4 | [Lowest Common Ancestor of a Binary Tree](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-tree) | Medium | Meta, Amazon, Apple, Scale AI |
| 5 | [Accounts Merge](https://leetcode.com/problems/accounts-merge) | Medium | Meta, Google |
| 6 | [Word Ladder](https://leetcode.com/problems/word-ladder) | Hard | Google, Amazon, OpenAI, Apple, Palantir, Tesla |
| 7 | [Alien Dictionary](https://leetcode.com/problems/alien-dictionary) | Hard | Google, OpenAI, Palantir, Databricks, Netflix, Airbnb, Uber, Waymo, Tesla |
| 8 | [Number of Islands II](https://leetcode.com/problems/number-of-islands-ii) | Hard | Uber, ByteDance, Waymo |
| 9 | [Path With Minimum Effort](https://leetcode.com/problems/path-with-minimum-effort) | Medium | Google, Waymo |
| 10 | [Cheapest Flights Within K Stops](https://leetcode.com/problems/cheapest-flights-within-k-stops) | Medium | Microsoft, Databricks, Palantir, Airbnb |
| 11 | [Maximize Amount After Two Days of Conversions](https://leetcode.com/problems/maximize-amount-after-two-days-of-conversions) | Medium | Uber, ByteDance, Cerebras |
| 12 | [Find Leaves of Binary Tree](https://leetcode.com/problems/find-leaves-of-binary-tree) | Medium | LinkedIn, Google, Cerebras |

### Dynamic Programming

| No. | Question | Difficulty | Companies |
| --- | -------- | ---------- | --------- |
| 1 | [Word Break](https://leetcode.com/problems/word-break) | Medium | Meta, Amazon, Apple |
| 2 | [Coin Change](https://leetcode.com/problems/coin-change) | Medium | Google, Amazon |
| 3 | [Best Time to Buy and Sell Stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock) | Easy | Meta, Amazon, Apple |
| 4 | [Edit Distance](https://leetcode.com/problems/edit-distance) | Medium | Google, Netflix, LinkedIn |
| 5 | [Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring) | Medium | All |
| 6 | [Longest Increasing Subsequence](https://leetcode.com/problems/longest-increasing-subsequence) | Medium | Google, Tesla, Palantir, Apple |
| 7 | [Maximum Profit in Job Scheduling](https://leetcode.com/problems/maximum-profit-in-job-scheduling) | Hard | Apple, Airbnb, DoorDash |
| 8 | [Longest Increasing Path in a Matrix](https://leetcode.com/problems/longest-increasing-path-in-a-matrix) | Hard | Google, NVIDIA, ByteDance, DoorDash, Waymo |

### Design

| No. | Question | Difficulty | Companies |
| --- | -------- | ---------- | --------- |
| 1 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium | All |
| 2 | [Implement Trie (Prefix Tree)](https://leetcode.com/problems/implement-trie-prefix-tree) | Medium | Google, OpenAI, Anthropic, Databricks, DeepMind, Perplexity |
| 3 | [Design Hit Counter](https://leetcode.com/problems/design-hit-counter) | Medium | Netflix, Anthropic, Databricks, Amazon, Apple, Uber, Tesla |
| 4 | [LFU Cache](https://leetcode.com/problems/lfu-cache) | Hard | Amazon, OpenAI, LinkedIn, Waymo |
| 5 | [Time Based Key-Value Store](https://leetcode.com/problems/time-based-key-value-store) | Medium | OpenAI, Databricks, Apple, Netflix, Perplexity |
| 6 | [Snapshot Array](https://leetcode.com/problems/snapshot-array) | Medium | OpenAI, Google, Databricks, DeepMind |
| 7 | [Logger Rate Limiter](https://leetcode.com/problems/logger-rate-limiter) | Easy | Google, Netflix, Waymo, Perplexity |
| 8 | [Design Tic-Tac-Toe](https://leetcode.com/problems/design-tic-tac-toe) | Medium | Meta, Databricks, Waymo |
| 9 | [Find Median from Data Stream](https://leetcode.com/problems/find-median-from-data-stream) | Hard | Netflix, Uber, Google, Meta, DeepMind, Perplexity |

### Concurrency and Systems (Rising Category)

Concurrency follow-ups are now standard at LinkedIn, Anthropic, Databricks, xAI, Cohere, and NVIDIA, often as the *second half* of an otherwise ordinary problem.

| No. | Question | Difficulty | Companies |
| --- | -------- | ---------- | --------- |
| 1 | [Web Crawler Multithreaded](https://leetcode.com/problems/web-crawler-multithreaded) | Medium | OpenAI, Anthropic |
| 2 | [Print in Order](https://leetcode.com/problems/print-in-order) | Easy | Databricks |
| 3 | [Building H2O](https://leetcode.com/problems/building-h2o) | Medium | Databricks |
| 4 | [The Dining Philosophers](https://leetcode.com/problems/the-dining-philosophers) | Medium | Databricks |
| 5 | Thread-safe LRU with read-write lock | Hard | NVIDIA, LinkedIn, Databricks |
| 6 | Token-bucket rate limiter (thread-safe) | Hard | Uber, Cohere, Databricks, xAI |

### Machine Learning

| No. | Question | Difficulty | Companies |
| --- | -------- | ---------- | --------- |
| 1 | [K-Closest Points to Origin](https://leetcode.com/problems/k-closest-points-to-origin) | Medium | OpenAI, Google |
| 2 | [Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements) | Medium | OpenAI, Google, Amazon, Anthropic |
| 3 | [Word Ladder](https://leetcode.com/problems/word-ladder) | Hard | OpenAI, Google, Amazon |
| 4 | [Time Based Key-Value Store](https://leetcode.com/problems/time-based-key-value-store) | Medium | OpenAI, Databricks |
| 5 | [Design Search Autocomplete System](https://leetcode.com/problems/design-search-autocomplete-system) | Hard | Amazon, Netflix, OpenAI, Uber |
| 6 | [Implement Trie (Prefix Tree)](https://leetcode.com/problems/implement-trie-prefix-tree) | Medium | OpenAI, Google, Meta, Anthropic |

### ML Coding From Scratch (Asked at AI Labs)

These recur across OpenAI, Anthropic, Mistral, DeepMind, xAI, Perplexity, and NVIDIA loops. See the [AI Labs guide](./AI-Companies-Interview-Questions.md) for company-by-company detail.

| No. | Task | Companies |
| --- | ---- | --------- |
| 1 | Implement scaled dot-product / multi-head attention from scratch (numpy or raw PyTorch, no libraries) | OpenAI, Anthropic, Mistral, DeepMind |
| 2 | Debug a broken Transformer (position-embedding init, mask values, missing `loss.backward()`, wrong `nn.Linear` dims) | OpenAI, Amazon AGI, Mistral, Apple |
| 3 | Implement top-k / top-p (nucleus) sampling | Mistral |
| 4 | Write a BPE-style / greedy tokenizer | Mistral, Anthropic, Perplexity |
| 5 | Implement KV-cache management for batched inference | Mistral, NVIDIA, Together AI |
| 6 | Implement beam search | xAI, Perplexity |
| 7 | Implement a request batching / inference engine | xAI, Cohere, Together AI |
| 8 | Implement KL divergence / cross-entropy from first principles | OpenAI |

---

<div align="center">

### 🔔 You Found the Shortcut. Don't Lose It.

New questions, papers, and strategies drop here **every single week**: before they surface anywhere else.

The engineers who land FAANG offers aren't the ones who *find* a resource. They're the ones who **never lose it**.

⚡ **One click. Every update. Zero effort.**

<a href="https://github.com/ombharatiya/FAANG-Coding-Interview-Questions/subscription">
  <img src="https://img.shields.io/badge/🔔 Watch This Repo-Get Every Update-blue?style=for-the-badge" alt="Watch Repo" />
</a>&nbsp;
<a href="https://github.com/ombharatiya/FAANG-Coding-Interview-Questions">
  <img src="https://img.shields.io/badge/⭐ Star-Show Support-yellow?style=for-the-badge" alt="Star Repo" />
</a>

**Follow [@ombharatiya](https://github.com/ombharatiya)** for exclusive tips, paper breakdowns, and career moves that never make it into the repo:

[![GitHub](https://img.shields.io/badge/GitHub-@ombharatiya-181717?style=flat-square&logo=github)](https://github.com/ombharatiya)
[![Twitter](https://img.shields.io/badge/Twitter-@ombharatiya-1DA1F2?style=flat-square&logo=twitter)](https://twitter.com/ombharatiya)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-ombharatiya-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/ombharatiya)

</div>
