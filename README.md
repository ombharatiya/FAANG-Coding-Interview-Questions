# FAANG / MAANG+ Coding Interview Questions

<div align="center">

  <p><strong>A curated collection of coding, system design, and ML interview questions from top tech companies.</strong><br/>Continuously updated with 2025-2026 interview questions across 44 companies: FAANG, frontier AI labs, and AI-first startups.</p>

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
- [AI Labs & AI Companies Interview Questions](./AI-Companies-Interview-Questions.md): DeepMind, xAI, Mistral, Perplexity, Scale AI, Cohere, Cursor, Waymo and 12 more
- [System Design Interview Guide](./SYSTEM_DESIGN_INTERVIEW.md)

**AI & Machine Learning**
- [LLM Papers Cheatsheet - Essential Research Papers](./LLM_PAPERS_CHEATSHEET.md)
- [Complete ML Interview Preparation Guide](./ML_INTERVIEW_PREP.md)
- [Guide to Building AI Agents](./AGENT_BUILDING_GUIDE.md)

**Programming Resources**
- [Python Resources](./PythonResources.md)

## What Changed in 2026

The interview format shifted more this past year than in the previous five. The headline: **AI-assisted rounds went mainstream**, and where AI is allowed the rubric moved to *verification*: test before you trust the output, and be able to explain it.

- **Meta** rolled out an AI-enabled coding round (3-panel CoderPad), now reaching SWE and EM roles up through E7/M2. **Google** is piloting an AI-assisted code-comprehension round with Gemini, while simultaneously bringing back an in-person round to curb cheating. **LinkedIn** made its AI-enabled round standard. **DoorDash** publicly rebuilt its interviews around AI.
- **OpenAI** added an agentic coding round in beta, the only *live* round where AI is allowed (the take-home also permits it for Applied AI roles). **Anthropic** runs a split policy (AI permitted on the take-home, banned in live rounds) and has redesigned that take-home three times because Claude kept beating it. **Sierra** dropped algorithm interviews entirely.
- **ByteDance** and **Palantir** explicitly ban AI use. **Amazon** and **Apple** report no AI round at all.
- **Work trials are the AI-startup norm**: Cursor runs paid 8-9 hour onsite projects; OpenAI's take-home is a paid (~$1,000) work trial.
- **Netflix** introduced formal engineering levels (E1-E7). The same answer is now scored against your target level.

Full breakdown in [FAANG-Recent-Questions.md](./FAANG-Recent-Questions.md#the-single-biggest-change-in-2026-ai-assisted-rounds) and the [AI Labs guide](./AI-Companies-Interview-Questions.md#2026-ai-interview-trends).

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
| 13. | [Stripe](#stripe) |
| 14. | [NVIDIA](#nvidia) |
| 15. | [Uber](#uber) |
| 16. | [ByteDance / TikTok](#bytedance--tiktok) |
| 17. | [Airbnb](#airbnb) |
| 18. | [DoorDash](#doordash) |
| 19. | [Tesla](#tesla) |
| 20. | [Flipkart](#flipkart) |
| 21. | [Anduril](./FAANG-Recent-Questions.md#anduril) |
| 22. | [Figma](./FAANG-Recent-Questions.md#figma) |
| 23. | [Ramp](./FAANG-Recent-Questions.md#ramp) |

**AI Labs & AI Companies**: [full guide](./AI-Companies-Interview-Questions.md)

| SNo. | Company | Signature Round |
| ---- | ------- | --------------- |
| 1. | [Google DeepMind](./AI-Companies-Interview-Questions.md#google-deepmind) | 2-hour rapid-fire technical quiz (CS + math + stats + ML) |
| 2. | [xAI](./AI-Companies-Interview-Questions.md#xai) | Proctored CodeSignal; concurrency-at-scale extensions |
| 3. | [Mistral AI](./AI-Companies-Interview-Questions.md#mistral-ai) | LLM knowledge quiz; ML coding from scratch |
| 4. | [Meta Superintelligence Labs](./AI-Companies-Interview-Questions.md#meta-superintelligence-labs) | AI-enabled coding round |
| 5. | [Amazon AGI](./AI-Companies-Interview-Questions.md#amazon-agi) | Transformer debugging + Leadership Principles |
| 6. | [Perplexity AI](./AI-Companies-Interview-Questions.md#perplexity-ai) | Founder final round; RAG/search depth |
| 7. | [Scale AI](./AI-Companies-Interview-Questions.md#scale-ai) | Card-game OOP simulation; debugging round |
| 8. | [Cohere](./AI-Companies-Interview-Questions.md#cohere) | Production infra code (Python/Go), no LeetCode tricks |
| 9. | [Hugging Face](./AI-Companies-Interview-Questions.md#hugging-face) | Open-source take-home (Spaces demo) |
| 10. | [Cursor (Anysphere)](./AI-Companies-Interview-Questions.md#cursor-anysphere) | Paid 8-9 hour onsite project on the real codebase |
| 11. | [Together AI](./AI-Companies-Interview-Questions.md#together-ai) | CUDA kernel take-home |
| 12. | [Groq](./AI-Companies-Interview-Questions.md#groq) | Compiler/LPU depth (NDA before first interview) |
| 13. | [Cerebras](./AI-Companies-Interview-Questions.md#cerebras) | Two LC Mediums in 45 minutes |
| 14. | [ElevenLabs](./AI-Companies-Interview-Questions.md#elevenlabs) | Product decomposition round |
| 15. | [Waymo](./AI-Companies-Interview-Questions.md#waymo) | Modern C++; correctness over speed |
| 16. | [Character.AI](./AI-Companies-Interview-Questions.md#characterai) | ML coding + real-time chat design |
| 17. | [Sierra AI](./AI-Companies-Interview-Questions.md#sierra-ai) | Plan -> Build (2h with AI) -> Review; no algorithms |
| 18. | [Glean](./AI-Companies-Interview-Questions.md#glean) | 2-hour on-the-spot build assignment |
| 19. | [Runway](./AI-Companies-Interview-Questions.md#runway) | Craft deep-dive; GPU pipeline design |
| 20. | [Snowflake](./AI-Companies-Interview-Questions.md#snowflake-aidata) | Data-processing twists; Cortex/AI platform design |

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

**AI Lab Track** (OpenAI, Anthropic, DeepMind, Mistral, xAI)
- Read the [AI Labs & AI Companies guide](./AI-Companies-Interview-Questions.md). These loops look nothing like FAANG
- Practice implementing attention, tokenizers, and sampling **from scratch**: no libraries
- Prepare for debugging rounds (broken Transformers, planted bugs) and progressive multi-level problems
- Expect concurrency follow-ups on ordinary problems, and values/mission rounds that are real gates

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
| 14 | [Maximum Subarray](https://leetcode.com/problems/maximum-subarray) | Medium | O(n) | O(1) |
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
<summary>View 45 Problems (2025-2026 Most Frequent)</summary>

**2026 changes**: an AI-assisted "code comprehension" round is piloting, in which you debug and optimize an existing codebase with **Gemini available**; interviewers score AI fluency (prompting, output validation, debugging AI output). An **in-person round has been reinstated** to curb AI-assisted cheating. The Googleyness round is now part-technical. Roughly 19% of reported problems are Hard. Segment tree / BIT problems are a Google-distinctive category.

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
| 22 | [Edit Distance](https://leetcode.com/problems/edit-distance) | Medium | Dynamic Programming |
| 23 | [Minimum Window Substring](https://leetcode.com/problems/minimum-window-substring) | Hard | Sliding Window |
| 24 | [Implement Trie (Prefix Tree)](https://leetcode.com/problems/implement-trie-prefix-tree) | Medium | Trie |
| 25 | [Accounts Merge](https://leetcode.com/problems/accounts-merge) | Medium | Union-Find |
| 26 | [Sliding Window Maximum](https://leetcode.com/problems/sliding-window-maximum) | Hard | Monotonic Deque |
| 27 | [The Skyline Problem](https://leetcode.com/problems/the-skyline-problem) | Hard | Heap / Divide and Conquer |
| 28 | [Largest Rectangle in Histogram](https://leetcode.com/problems/largest-rectangle-in-histogram) | Hard | Monotonic Stack |
| 29 | [Word Search II](https://leetcode.com/problems/word-search-ii) | Hard | Trie / Backtracking |
| 30 | [Rotting Oranges](https://leetcode.com/problems/rotting-oranges) | Medium | Graph / BFS |
| 31 | [Critical Connections in a Network](https://leetcode.com/problems/critical-connections-in-a-network) | Hard | Graph / Tarjan's |
| 32 | [Pacific Atlantic Water Flow](https://leetcode.com/problems/pacific-atlantic-water-flow) | Medium | Graph / Multi-source BFS |
| 33 | [Network Delay Time](https://leetcode.com/problems/network-delay-time) | Medium | Graph / Dijkstra |
| 34 | [Daily Temperatures](https://leetcode.com/problems/daily-temperatures) | Medium | Monotonic Stack |
| 35 | [Find the Safest Path in a Grid](https://leetcode.com/problems/find-the-safest-path-in-a-grid) | Medium | BFS / Binary Search |
| 36 | [The Earliest Moment When Everyone Become Friends](https://leetcode.com/problems/the-earliest-moment-when-everyone-become-friends) | Medium | Union-Find |
| 37 | [Checking Existence of Edge Length Limited Paths](https://leetcode.com/problems/checking-existence-of-edge-length-limited-paths) | Hard | Union-Find / Offline Queries |
| 38 | [Longest String Chain](https://leetcode.com/problems/longest-string-chain) | Medium | DP / Hash |
| 39 | [Maximum Points You Can Obtain from Cards](https://leetcode.com/problems/maximum-points-you-can-obtain-from-cards) | Medium | Sliding Window |
| 40 | [Step-By-Step Directions From a Binary Tree Node to Another](https://leetcode.com/problems/step-by-step-directions-from-a-binary-tree-node-to-another) | Medium | Tree / LCA |
| 41 | [Swim in Rising Water](https://leetcode.com/problems/swim-in-rising-water) | Hard | Binary Search + BFS |
| 42 | [Detect Squares](https://leetcode.com/problems/detect-squares) | Medium | Design / Geometry |
| 43 | [Amount of New Area Painted Each Day](https://leetcode.com/problems/amount-of-new-area-painted-each-day) | Hard | Sweep Line / Segment Tree |
| 44 | [Range Sum Query - Mutable](https://leetcode.com/problems/range-sum-query-mutable) | Medium | Segment Tree / BIT |
| 45 | [Best Meeting Point](https://leetcode.com/problems/best-meeting-point) | Hard | Math / Median |

**Custom problems**: restaurant waitlist data structure; number of lakes on an island; root an undirected acyclic graph as a binary tree; top-K most talkative users from chat logs; network of teleporters; car rental booking overlap.

</details>

## Meta (Facebook)

<details>
<summary>View 45 Problems (2025-2026 Most Frequent)</summary>

**2026 changes**: The **AI-enabled coding round** is rolling out to all SWE roles, 60 min in a 3-panel CoderPad (file explorer, editor, AI chat; GPT-5, Claude Sonnet, Gemini, Llama 4 available; AI reads files but cannot edit). Three phases: fix a bug -> build a 120+ line feature -> optimize for larger datasets. Scored on problem solving, code quality, **verification**, and communication. For E4-E5 it randomly replaces one of the two coding rounds; at E6 it also replaces one of two, so a traditional CoderPad round normally remains. Behavioral weight increased, it can single-handedly downlevel E5 to E4. Candidates increasingly get *variants* of tagged problems.

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Minimum Remove to Make Valid Parentheses](https://leetcode.com/problems/minimum-remove-to-make-valid-parentheses) | Medium | Stack / String |
| 2 | [Binary Tree Vertical Order Traversal](https://leetcode.com/problems/binary-tree-vertical-order-traversal) | Medium | Tree / BFS |
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
| 26 | [Valid Word Abbreviation](https://leetcode.com/problems/valid-word-abbreviation) | Easy | String / Parsing |
| 27 | [Lowest Common Ancestor of a Binary Tree III](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-tree-iii) | Medium | Tree / Hash Table |
| 28 | [Convert BST to Sorted Doubly Linked List](https://leetcode.com/problems/convert-binary-search-tree-to-sorted-doubly-linked-list) | Medium | Tree / Linked List |
| 29 | [K Closest Points to Origin](https://leetcode.com/problems/k-closest-points-to-origin) | Medium | Heap / Math |
| 30 | [Interval List Intersections](https://leetcode.com/problems/interval-list-intersections) | Medium | Two Pointers / Intervals |
| 31 | [Simplify Path](https://leetcode.com/problems/simplify-path) | Medium | Stack / String |
| 32 | [Insert Delete GetRandom O(1)](https://leetcode.com/problems/insert-delete-getrandom-o1) | Medium | Design / Hash Table |
| 33 | [Sliding Window Maximum](https://leetcode.com/problems/sliding-window-maximum) | Hard | Monotonic Deque |
| 34 | [Regular Expression Matching](https://leetcode.com/problems/regular-expression-matching) | Hard | DP / Recursion |
| 35 | [All Nodes Distance K in Binary Tree](https://leetcode.com/problems/all-nodes-distance-k-in-binary-tree) | Medium | Tree / BFS |
| 36 | [Validate IP Address](https://leetcode.com/problems/validate-ip-address) | Medium | String Parsing |
| 37 | [Remove All Adjacent Duplicates in String II](https://leetcode.com/problems/remove-all-adjacent-duplicates-in-string-ii) | Medium | Stack |
| 38 | [Greatest Common Divisor of Strings](https://leetcode.com/problems/greatest-common-divisor-of-strings) | Easy | String / Math |
| 39 | [Find the Length of the Longest Common Prefix](https://leetcode.com/problems/find-the-length-of-the-longest-common-prefix) | Medium | Trie / Hash |
| 40 | [Toeplitz Matrix](https://leetcode.com/problems/toeplitz-matrix) | Easy | Matrix |
| 41 | [Range Sum Query 2D - Immutable](https://leetcode.com/problems/range-sum-query-2d-immutable) | Medium | Prefix Sums |
| 42 | [Diagonal Traverse II](https://leetcode.com/problems/diagonal-traverse-ii) | Medium | Array / BFS |
| 43 | [Wildcard Matching](https://leetcode.com/problems/wildcard-matching) | Hard | DP |
| 44 | [Integer to English Words](https://leetcode.com/problems/integer-to-english-words) | Hard | String / Recursion |
| 45 | [First Missing Positive](https://leetcode.com/problems/first-missing-positive) | Hard | Array / Index Cycle |

**AI-round problems** (~9 in rotation): Maze Solver with Path Printing; Maximize Unique Characters from Word List; Card Game (Three Cards Summing to 15); Friend Recommendation System.

</details>

## Amazon

<details>
<summary>View 45 Problems (2025-2026 Most Frequent)</summary>

**2026 changes**: HackerRank OA = 2 coding problems (~70 min) + Work Simulation (~20 min) + Work Style Assessment; the SDE II OA adds a 20-min System Design scenario. ~75-80% of OA problems are Medium, wrapped in Amazon-themed framing (servers, warehouses, parcels). Onsite is ~50/50 coding vs Leadership Principles in every round, plus Bar Raiser. Rising: Dijkstra/weighted-shortest-path problems. **No AI-assisted round**: Amazon rotates custom OA sets aggressively instead, so pattern prep beats memorization.

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
| 26 | [Car Pooling](https://leetcode.com/problems/car-pooling) | Medium | Array / Prefix Sum |
| 27 | [Meeting Rooms III](https://leetcode.com/problems/meeting-rooms-iii) | Hard | Heap / Sorting |
| 28 | [K Closest Points to Origin](https://leetcode.com/problems/k-closest-points-to-origin) | Medium | Heap / Math |
| 29 | [Valid Parentheses](https://leetcode.com/problems/valid-parentheses) | Easy | Stack / String |
| 30 | [Word Search](https://leetcode.com/problems/word-search) | Medium | Backtracking / Matrix |
| 31 | [Course Schedule II](https://leetcode.com/problems/course-schedule-ii) | Medium | Graph / Topological Sort |
| 32 | [Design Hit Counter](https://leetcode.com/problems/design-hit-counter) | Medium | Design / Queue |
| 33 | [Min Stack](https://leetcode.com/problems/min-stack) | Medium | Stack / Design |
| 34 | [Maximum Frequency After Subarray Operation](https://leetcode.com/problems/maximum-frequency-after-subarray-operation) | Medium | Array / Greedy-DP |
| 35 | [Maximize Y-Sum by Picking a Triplet of Distinct X-Values](https://leetcode.com/problems/maximize-ysum-by-picking-a-triplet-of-distinct-xvalues) | Medium | Heap / Greedy |
| 36 | [Max Difference You Can Get From Changing an Integer](https://leetcode.com/problems/max-difference-you-can-get-from-changing-an-integer) | Medium | Greedy / Digits |
| 37 | [Analyze User Website Visit Pattern](https://leetcode.com/problems/analyze-user-website-visit-pattern) | Medium | Hash / Sorting |
| 38 | [Minimum Cost to Connect Sticks](https://leetcode.com/problems/minimum-cost-to-connect-sticks) | Medium | Heap / Greedy |
| 39 | [Word Search II](https://leetcode.com/problems/word-search-ii) | Hard | Trie + Backtracking |
| 40 | [Alien Dictionary](https://leetcode.com/problems/alien-dictionary) | Hard | Topological Sort |
| 41 | [The Skyline Problem](https://leetcode.com/problems/the-skyline-problem) | Hard | Sweep Line / Heap |
| 42 | [Burst Balloons](https://leetcode.com/problems/burst-balloons) | Hard | Interval DP |
| 43 | [Count of Smaller Numbers After Self](https://leetcode.com/problems/count-of-smaller-numbers-after-self) | Hard | Merge Sort / BIT |
| 44 | [Max Points on a Line](https://leetcode.com/problems/max-points-on-a-line) | Hard | Geometry / Hash |
| 45 | [Reorder List](https://leetcode.com/problems/reorder-list) | Medium | Linked List |

**Custom OA problems (2026)**: Server Allocation Cost; Warehouse Distribution; Minimum Array Operations; Bug Sorting by Frequency & Code; Distribute Parcels; Suitable Warehouse Locations; Min Cost To Add New Roads (Hard); Dropped Requests (Hard).

</details>

## Apple

<details>
<summary>View 30 Problems (2025-2026 Most Frequent)</summary>

**Still radically team-dependent. No unified loop**: some teams ask standard LC mediums, embedded/hardware teams ask C/C++ memory questions, services teams ask API design or debug-broken-code. **2026**: design-style coding questions are disproportionately common; loops for experienced hires run 8-9 rounds over several weeks. **No AI-assisted rounds reported**: human-only interviews graded on correctness, memory behavior, and boundary handling.

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
| 21 | [Sum Root to Leaf Numbers](https://leetcode.com/problems/sum-root-to-leaf-numbers) | Medium | Trees |
| 22 | [Check Completeness of a Binary Tree](https://leetcode.com/problems/check-completeness-of-a-binary-tree) | Medium | Trees / BFS |
| 23 | [Time Based Key-Value Store](https://leetcode.com/problems/time-based-key-value-store) | Medium | Design / Binary Search |
| 24 | [Design Hit Counter](https://leetcode.com/problems/design-hit-counter) | Medium | Design |
| 25 | [Design Add and Search Words Data Structure](https://leetcode.com/problems/design-add-and-search-words-data-structure) | Medium | Trie / Design |
| 26 | [Vertical Order Traversal of a Binary Tree](https://leetcode.com/problems/vertical-order-traversal-of-a-binary-tree) | Hard | Trees |
| 27 | [Binary Search Tree Iterator](https://leetcode.com/problems/binary-search-tree-iterator) | Medium | Design / Trees |
| 28 | [Subarray Sum Equals K](https://leetcode.com/problems/subarray-sum-equals-k) | Medium | Prefix Sum |
| 29 | [Minimum Unique Word Abbreviation](https://leetcode.com/problems/minimum-unique-word-abbreviation) | Hard | Backtracking / Bitmask |
| 30 | [H-Index](https://leetcode.com/problems/h-index) | Medium | Sorting |

**Custom problems**: memory-efficient ProRAW image decoder (<=1GB RAM); lock-free queue for watchOS sensor data; debug a PyTorch U-Net shape mismatch; Bag-of-Words similarity search; Library Management System OOP design.

</details>

## Netflix

<details>
<summary>View 22 Problems (2025-2026 Most Frequent)</summary>

**Biggest 2026 change: formal engineering levels.** Netflix moved from a single "Senior Engineer" rung to an explicit multi-band ladder (~E1/L4-E7). The same coding answer is now scored against your target level, so an answer that passes at E4 can fail at E6 for being "too tactical." Loops are decentralized and team-owned; the hiring manager is involved from the first screen. Coding favors practical mediums re-skinned with Netflix domain (shows, playlists, watch history). The culture/Keeper Test round is mandatory in every loop.

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
| 16 | [Rotating the Box](https://leetcode.com/problems/rotating-the-box) | Medium | Matrix / Simulation |
| 17 | [Time Based Key-Value Store](https://leetcode.com/problems/time-based-key-value-store) | Medium | Design / Binary Search |
| 18 | [Logger Rate Limiter](https://leetcode.com/problems/logger-rate-limiter) | Easy | Design |
| 19 | [Word Search II](https://leetcode.com/problems/word-search-ii) | Hard | Trie / Backtracking |
| 20 | [Reconstruct Itinerary](https://leetcode.com/problems/reconstruct-itinerary) | Hard | Graph / Euler Path |
| 21 | [Alien Dictionary](https://leetcode.com/problems/alien-dictionary) | Hard | Topological Sort |
| 22 | [Parallel Courses](https://leetcode.com/problems/parallel-courses) | Medium | Topological Sort |

**Custom problems**: TTL Cache with LRU eviction; Weighted Eviction Cache; Versioned Key-Value Store; Streaming Word Counter; group users by overlapping last-K watched movies; playlist add/remove/shuffle; rate limiter with graceful degradation when the limiter itself fails.

</details>

## Microsoft

<details>
<summary>View 30 Problems (2025-2026 Most Frequent)</summary>

**2026 changes**: Process compressed. OA (2 mediums) then 4 virtual onsite rounds usually on a single day; SDE2 loops = 2-3 DSA + LLD + HLD + hiring manager. The **"As Appropriate" (AA) round** is formalized and run by Principal EMs; ~85% who reach it get offers, but it retains veto power. Behavioral "growth mindset" scoring is level-banded. **AI-assisted rounds are org-specific, not universal**: mostly CoreAI/Copilot teams; ask your recruiter.

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
| 21 | [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water) | Hard | Two Pointers |
| 22 | [Container With Most Water](https://leetcode.com/problems/container-with-most-water) | Medium | Two Pointers |
| 23 | [Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring) | Medium | DP / Strings |
| 24 | [Next Permutation](https://leetcode.com/problems/next-permutation) | Medium | Arrays |
| 25 | [Search in Rotated Sorted Array](https://leetcode.com/problems/search-in-rotated-sorted-array) | Medium | Binary Search |
| 26 | [Spiral Matrix](https://leetcode.com/problems/spiral-matrix) | Medium | Matrix |
| 27 | [Word Search](https://leetcode.com/problems/word-search) | Medium | Backtracking |
| 28 | [First Missing Positive](https://leetcode.com/problems/first-missing-positive) | Hard | Arrays |
| 29 | [Jump Game II](https://leetcode.com/problems/jump-game-ii) | Medium | Greedy |
| 30 | [Generate Parentheses](https://leetcode.com/problems/generate-parentheses) | Medium | Backtracking |

**Custom problems (2026)**: reconstruct DNA payload strings from tagged fragments; build a CSV query engine; in-memory URL shortener; memory allocation simulation; debug broken queue code; combined rate-limiter + LFU round; traverse an org chart by level; minimum moves on a grid with k-cell jumps.

**LLD**: Vending Machine, Parking Lot, Snake & Ladder, Elevator Control System (SOLID + State/Strategy probed).

</details>

## LinkedIn

<details>
<summary>View 30 Problems (2025-2026 Most Frequent)</summary>

**2026 changes**: The **AI-enabled coding round is now standard**: one of two coding rounds, on CoderPad with an AI chat panel (Claude/Opus tiers). The AI **cannot edit code**: you paste and verify. Graded on a **4-point scale where 3 passes**, relative to other candidates. **The follow-ups are the real bar**: after working code, questioning pivots to concurrency/thread safety, scaling, malformed input, and production readiness.

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
| 21 | [LFU Cache](https://leetcode.com/problems/lfu-cache) | Hard | Design (confirmed in AI-enabled round) |
| 22 | [Insert Delete GetRandom O(1) - Duplicates allowed](https://leetcode.com/problems/insert-delete-getrandom-o1-duplicates-allowed) | Hard | Design |
| 23 | [Max Consecutive Ones III](https://leetcode.com/problems/max-consecutive-ones-iii) | Medium | Sliding Window |
| 24 | [Max Consecutive Ones II](https://leetcode.com/problems/max-consecutive-ones-ii) | Medium | Sliding Window |
| 25 | [Design Authentication Manager](https://leetcode.com/problems/design-authentication-manager) | Medium | Design / TTL |
| 26 | [Serialize and Deserialize BST](https://leetcode.com/problems/serialize-and-deserialize-bst) | Medium | Trees / Design |
| 27 | [Paint House III](https://leetcode.com/problems/paint-house-iii) | Hard | DP |
| 28 | [Allocate Mailboxes](https://leetcode.com/problems/allocate-mailboxes) | Hard | DP |
| 29 | [Generate Random Point in a Circle](https://leetcode.com/problems/generate-random-point-in-a-circle) | Medium | Math / Randomized |
| 30 | [Valid Perfect Square](https://leetcode.com/problems/valid-perfect-square) | Easy | Binary Search |

**Custom problems**: structured data processing from scratch (parse JSON-like objects, AI-round staple); Merge Intervals reframed as a data-structure-choice design problem; LRU Cache with thread-safety and scaling follow-ups; merge two n-ary trees by key rules; count trips from vehicle logs.

</details>

## OpenAI

<details>
<summary>View Problems (2025-2026 -- Production-Oriented)</summary>

OpenAI interviews focus on practical engineering over LeetCode puzzles. Problems are drawn from a bank of ~8 core challenges with progressive difficulty layers, and the bank churns. Python is strongly recommended.

**New in 2026**: (1) **Agentic coding round (beta)**: you get an existing codebase and must add features scoped "too large and complex to tackle by hand," so you're *expected* to drive an AI coding agent. This is the only *live* round where AI is permitted. Every other interview strictly prohibits it (the take-home is the one other carve-out, and only for Applied AI roles). (2) The 48-hour take-home is now a **paid work trial (~$1,000)** under NDA, graded like a senior engineer's PR review, **"missing test coverage" is the single most-cited rejection reason**. (3) Loop = 2 coding + 1 system design + behavioral + hiring manager, plus a 45-min project presentation round.

**Core Custom Problems (Most Frequently Reported)**

| No. | Problem | Difficulty | Category | Context |
| --- | ------- | ---------- | -------- | ------- |
| 1 | KV Store Serialize/Deserialize | Hard | Design / Strings | Multi-part: basic serialization, file persistence, multithreading, versioned store |
| 2 | CD Directory Navigation | Hard | String / Path Resolution | Implement `cd()` with relative/absolute paths, `..`, `.`, `~`, symlink cycle detection |
| 3 | Excel/Spreadsheet Engine | Hard | Graph / Design | `getCell()` O(1), `setCell()` with formula dependencies, circular dependency detection |
| 4 | In-Memory Database | Hard | Database Design | `select()` with WHERE, AND, ORDER BY, comparison operators -- no SQL parsing |
| 5 | Resumable Iterator | Hard | Iterator / State | Stateful iterator with `getState()`/`setState()`; now up to 6 parts: lists -> multi-file -> async -> 2D -> 3D |
| 6 | Async Node Counting | Hard | Distributed / Trees | Count tree nodes using only async parent-child messaging |
| 7 | Dependency Version Finder (new 2026) | Medium-Hard | Iterative Refinement | Find earliest version supporting a feature; requirements evolve as test cases are revealed |
| 8 | GPU Credit Allocation | Hard | Design / State | Half-open intervals `[start, expiration)`, consume soonest-expiring first, balance at any timestamp |
| 9 | Versioned KV Store | Hard | Design | Auto-versioning; follow-ups: global vs per-key locks, optimistic locking, disk persistence |
| 10 | Token Consumption Log Parser | Easy-Medium | Parsing | Parse API-call logs, total tokens per user, sort by user ID |

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

Anthropic uses a CodeSignal OA followed by a 4-6 hour onsite with 4-6 rounds. Python expected. Problems are drawn from a bank of ~6 core custom challenges with progressive difficulty layers, and **recruiters tell you which prompt family you'll get days beforehand**.

**Split AI policy**: AI tools are strictly prohibited in all live interviews (candidates have been dropped for using them), but **explicitly permitted on the performance take-home**. Google/Stack Overflow are allowed in live coding.

**The performance take-home has been redesigned three times because Claude kept beating it** (Anthropic engineering blog + TechCrunch, Jan 2026): V1 (2024) was a 4-hour simulated-accelerator optimization; V2 (mid-2025) was cut to 2 hours after Claude Opus 4 outperformed most humans; V3 (late 2025) is a Zachtronics-puzzle-style constrained instruction set where you minimize instruction count with **no built-in debugging tools, building your own tooling is part of the test**. The original is open-sourced at [anthropics/original_performance_takehome](https://github.com/anthropics/original_performance_takehome).

**The Values/Culture round (45 min) is the #1 failure point**: identical across all roles and levels. It's NOT behavioral/STAR: it evaluates holding complexity, admitting knowledge gaps, second-order reasoning, and intellectual honesty. Scripted STAR stories are the top failure mode, and measured skepticism about the mission scores better than performed enthusiasm.

**Core Custom Coding Problems (Most Frequently Reported)**

| No. | Problem | Difficulty | Category | Context |
| --- | ------- | ---------- | -------- | ------- |
| 1 | In-Memory Database | Hard | Design | 4 levels: SET/GET/DELETE -> filtered scans -> TTL -> backup/restore |
| 2 | Web Crawler | Hard | BFS / Concurrency | BFS crawl -> multithreaded/async optimization |
| 3 | LRU Cache (Bugfix + Extend) | Hard | Design / Debugging | Fix bugs, add persistence, handle `*args`/`**kwargs` |
| 4 | Stack Trace / Profiler | Hard | Parsing / Design | Convert sampling data to chronological events |
| 5 | Tokenization Engine | Hard | String / NLP | Greedy longest-match tokenization with unknown-token merging; also a code-review exercise |
| 6 | Distributed Mode/Median | Hard | Distributed Systems | Compute across 10 nodes with bandwidth constraints |
| 7 | Record Store | Hard | Progressive OA | In-memory DB + conditional writes + historical ("at timestamp") queries; L4 = compression/persistence |
| 8 | Bank Ledger | Medium-Hard | Progressive OA | Account creation -> merging -> delayed cashback -> spending analytics |
| 9 | Recipe Catalog / Task Tracker | Easy-Medium | Progressive OA | Metadata storage, search by ingredient/prep time; priority + deadline tracking |
| 10 | Profiler Trace Denoising | Hard | Algorithms | Filter short-lived calls; emit events only after N consecutive appearances |

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
| 11 | [Count of Smaller Numbers After Self](https://leetcode.com/problems/count-of-smaller-numbers-after-self) | Hard | Merge Sort / BIT (phone screen; O(n log n) required) |

**Key Focus Areas**: AI safety/alignment (Constitutional AI, RLHF, red-teaming), systems engineering (distributed training, inference optimization), concurrency/parallel programming, Transformer architecture depth. Prep material for the values round: Core Views on AI Safety + the Responsible Scaling Policy.

</details>

## Palantir

<details>
<summary>View 25 Problems + Unique Interview Format (2025-2026)</summary>

Palantir's onsite gives you 3 of 4 round types: **Decomposition**, **System Design**, **Re-engineering (Debugging)**, and **Coding**. Each round includes 20 min of behavioral questions. **AI use is strictly prohibited in interviews**: a notable divergence from the industry's 2026 drift toward AI-assisted rounds.

**The OA is a 3-part practical HackerRank (~90 min)**: one coding (shape classes OOP) + one SQL (sessions-per-city 3-table join) + one REST API task (paginated restaurant endpoint). Not pure DSA.

**Meritocracy Fellowship** (launched 2025): an alternative pipeline for high-school grads (SAT >= 1460 / ACT >= 33, $5,400/mo, 4 months). 22 hired from 500+ applicants; successful fellows interview for full-time roles without a degree.

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
| 21 | [Minimum Time Difference](https://leetcode.com/problems/minimum-time-difference) | Medium | String / Sorting |
| 22 | [Flood Fill](https://leetcode.com/problems/flood-fill) | Easy | BFS / DFS |
| 23 | [Cheapest Flights Within K Stops](https://leetcode.com/problems/cheapest-flights-within-k-stops) | Medium | Shortest Path |
| 24 | [Word Ladder](https://leetcode.com/problems/word-ladder) | Hard | BFS / State-Space Search |
| 25 | [Best Time to Buy and Sell Stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock) | Easy | Array |

**Unique Interview Rounds**
- **Decomposition**: Break down open-ended real-world problems. Non-coding. *AI-flavored prompts (new in 2026)*: an insurer wants LLM-powered claim summarization; a logistics firm wants an agent to reroute shipments; unify bank fraud detection across legacy systems; retailer demand forecasting; a platform for 500 data sources. *Classics*: "Design tech to help elderly cook safely"; chess; parking garage; social graph; infection spread; taxi dispatch.
- **Re-engineering (Debugging)**: Debug 500-1000 lines of buggy code with red herrings; sometimes proprietary-library docs are supplied
- **System Design**: Focus on data integration, ontology design, access control (ABAC); correctness and fault tolerance are first-class constraints
- **FDSE vs SWE**: Forward-deployed roles emphasize client-facing scenarios; backend roles emphasize scale

</details>

## Databricks

<details>
<summary>View 30 Problems (2025-2026 Most Frequent -- includes dedicated concurrency round)</summary>

Databricks has a unique **dedicated concurrency/multithreading round** (1 hour), "most companies wave at the topic; Databricks makes it an entire hour." OA is 4 problems in 70 minutes on CodeSignal (2 easy, 2 medium), webcam-proctored, scored on a scale up to 850. The onsite is fully virtual in 2026: 2 algorithm rounds + concurrency + system design + behavioral.

**Small question pool, deep follow-up variations**: the same core problems (SnapshotSet, Lazy Array, House Robber variants, Tic-Tac-Toe) recycle with escalating twists, including "now distribute this with Spark" follow-ups.

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
| 26 | [IP to CIDR](https://leetcode.com/problems/ip-to-cidr) | Medium | Bit Manipulation |
| 27 | [Max Area of Island](https://leetcode.com/problems/max-area-of-island) | Medium | DFS |
| 28 | [House Robber II](https://leetcode.com/problems/house-robber-ii) | Medium | DP |
| 29 | [Design Tic-Tac-Toe](https://leetcode.com/problems/design-tic-tac-toe) | Medium | Design (variable board + win condition) |
| 30 | [Top K Frequent Words](https://leetcode.com/problems/top-k-frequent-words) | Medium | Heap (in a stream, memory-bounded) |

**Custom problems**: **SnapshotSet / versioned iterator** (iterator reflects state at creation time, most-reported); **Lazy Array** (chained `map` + `indexOf`); Revenue System with referral chains; in-place delta encoding (+ "distribute with Spark"); replaying shell commands (`cp`/`ls`/`mv`/`!<index>`); SMS message splitting; lamps on a number line; multi-threaded logger; token-bucket rate limiter with burst probing.

</details>

## Stripe

<details>
<summary>View 19 Problems + Unique Interview Format (2025-2026)</summary>

Stripe does NOT use traditional LeetCode-style interviews. Problems model real engineering work -- payment processing, debugging, API integration. Code quality valued over algorithmic cleverness. Unique rounds: **Bug Squash** (debug a GitHub repo), **Integration** (build with Stripe API), **API Design** (REST resource modeling).

**2026 changes**: The new-grad OA is now a **single 60-minute multi-part question on HackerRank**: "measuring true coding ability with one question." **Integration round rules clarified: web/docs search is allowed, but AI coding assistants are NOT permitted.** Bug Squash now focuses sharply on financial-logic bugs: race conditions, missing idempotency checks, non-atomic check-then-act, unvalidated refund logic (~5-7 bugs in ~200 lines).

**LeetCode-Mapped Practice Problems**

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Two Sum](https://leetcode.com/problems/two-sum) | Easy | Hash Map (transaction matching) |
| 2 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium | Design (caching patterns) |
| 3 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium | Intervals (batch scheduling) |
| 4 | [Design Hit Counter](https://leetcode.com/problems/design-hit-counter) | Medium | Design (rate limiting) |
| 5 | [Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements) | Medium | Heap (merchant ranking) |
| 6 | [Subarray Sum Equals K](https://leetcode.com/problems/subarray-sum-equals-k) | Medium | Prefix Sum (revenue calc) |
| 7 | [Time Based Key-Value Store](https://leetcode.com/problems/time-based-key-value-store) | Medium | Design / Binary Search |
| 8 | [Course Schedule](https://leetcode.com/problems/course-schedule) | Medium | Graph / Cycle Detection |
| 9 | [Sliding Window Maximum](https://leetcode.com/problems/sliding-window-maximum) | Hard | Deque (event log analysis) |
| 10 | [Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree) | Hard | Design (JSON parsing) |
| 11 | [Coin Change](https://leetcode.com/problems/coin-change) | Medium | DP (fee calculation) |
| 12 | [Group Anagrams](https://leetcode.com/problems/group-anagrams) | Medium | Hashing / Strings |
| 13 | [Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self) | Medium | Arrays / Prefix |
| 14 | [Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters) | Medium | Sliding Window |
| 15 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium | Graph / DFS |
| 16 | [Evaluate Division](https://leetcode.com/problems/evaluate-division) | Medium | Graph (currency conversion analogue) |
| 17 | [Invalid Transactions](https://leetcode.com/problems/invalid-transactions) | Medium | Simulation (fraud-detection analogue) |
| 18 | [Single-Threaded CPU](https://leetcode.com/problems/single-threaded-cpu) | Medium | Heap (notification scheduler analogue) |
| 19 | [LFU Cache](https://leetcode.com/problems/lfu-cache) | Hard | Design (idempotency store analogue) |

**Custom Problems**: **Accept-Language header parser** (parse q-values, sort by quality, the long-standing screen); **currency conversion string parsing** (`"USD:CAD:DHL:5,..."` -> multi-hop -> best rate over all paths); card range obfuscation; fraud detection stream (CHARGE/DISPUTE, per-MCC thresholds); subscription notification scheduler; CSV parse + validate with circular dependency detection; invoice reconciliation; request deduplication (idempotency); webhook handler debugging; payment retry with exponential backoff; shipping cost calculator.

</details>

## NVIDIA

<details>
<summary>View 25 Problems (2025-2026 -- GPU/Performance Focus)</summary>

NVIDIA interviews emphasize performance awareness (cache hierarchies, memory bandwidth, parallelization). After solving the baseline, expect: "How does this behave under memory pressure? How would you parallelize across 10,000 threads?" C++ essential for systems/GPU roles.

**2026 changes**: Loops are team-scoped with a **"build from scratch" preference: interviewers prefer you avoid built-in library functions**. Candidates report bespoke variants over tagged problems. Classic problems now get systems extensions: LRU Cache follow-ups ask you to make it thread-safe with a read-write lock (and justify RW lock vs mutex), or relate it to GPU memory caching. **AI-infra system design is the new senior bar**: batch inference APIs on GPU clusters, tensor+pipeline parallelism across H100s, TensorRT-LLM/vLLM tradeoffs.

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Maximum Number of Events That Can Be Attended](https://leetcode.com/problems/maximum-number-of-events-that-can-be-attended) | Medium | Greedy / Heap |
| 2 | [Min Stack](https://leetcode.com/problems/min-stack) | Medium | Stack / Design |
| 3 | [Clone Graph](https://leetcode.com/problems/clone-graph) | Medium | Graph / DFS |
| 4 | [K Closest Points to Origin](https://leetcode.com/problems/k-closest-points-to-origin) | Medium | Heap / Math |
| 5 | [Random Pick with Weight](https://leetcode.com/problems/random-pick-with-weight) | Medium | Binary Search / Prefix Sum |
| 6 | [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water) | Hard | Two Pointers / Stack |
| 7 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium | Graph / DFS / BFS |
| 8 | [Rotate Image](https://leetcode.com/problems/rotate-image) | Medium | Array / Matrix |
| 9 | [Word Break](https://leetcode.com/problems/word-break) | Medium | Dynamic Programming |
| 10 | [Shortest Path in Binary Matrix](https://leetcode.com/problems/shortest-path-in-binary-matrix) | Medium | BFS / Graph |
| 11 | [Design HashMap](https://leetcode.com/problems/design-hashmap) | Easy | Design / Hash Table |
| 12 | [Longest Increasing Path in a Matrix](https://leetcode.com/problems/longest-increasing-path-in-a-matrix) | Hard | DFS / DP / Topological Sort |
| 13 | [Permutation in String](https://leetcode.com/problems/permutation-in-string) | Medium | Sliding Window |
| 14 | [Expression Add Operators](https://leetcode.com/problems/expression-add-operators) | Hard | Backtracking / Math |
| 15 | [Binary Search Tree Iterator](https://leetcode.com/problems/binary-search-tree-iterator) | Medium | Tree / Stack |
| 16 | [Word Ladder II](https://leetcode.com/problems/word-ladder-ii) | Hard | BFS / DFS / Backtracking |
| 17 | [Bus Routes](https://leetcode.com/problems/bus-routes) | Hard | BFS / Graph |
| 18 | [Making A Large Island](https://leetcode.com/problems/making-a-large-island) | Hard | DFS / Union Find |
| 19 | [Line Reflection](https://leetcode.com/problems/line-reflection) | Medium | Hash Table / Math |
| 20 | [Missing Ranges](https://leetcode.com/problems/missing-ranges) | Easy | Array / String |
| 21 | [Special Binary String](https://leetcode.com/problems/special-binary-string) | Hard | String / Recursion |
| 22 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium | Design (thread-safe RW-lock extension) |
| 23 | [Maximum Binary Tree](https://leetcode.com/problems/maximum-binary-tree) | Medium | Recursion / Tree |
| 24 | [Merge k Sorted Lists](https://leetcode.com/problems/merge-k-sorted-lists) | Hard | Heap / Linked List |
| 25 | [Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters) | Medium | Sliding Window |

**CUDA/GPU-Specific**: Matrix multiplication optimization (GEMM), CUDA kernel fusion, memory coalescing analysis, thread synchronization across blocks, multi-GPU communication patterns. **2026 conceptual drills**: profile a slow kernel with Nsight Compute; fix uncoalesced access / bank conflicts / thread divergence; make a kernel scale across GPU architectures; occupancy analysis.

**Custom problems**: polynomial multiplication API in C; temperature spike detection from (timestamp, temp) pairs; minimum sum after K operations; log aggregation by HTTP status code; tree planting constraint satisfaction.

</details>

## Uber

<details>
<summary>View 24 Problems (2025-2026 -- Domain-Driven)</summary>

Uber interviews reflect the product domain -- routing, dispatch, surge pricing map to graph traversal, streaming aggregation, and sliding-window patterns. Code readability is explicitly evaluated.

**2026 changes**: **Machine-coding / LLD rounds are the differentiator at senior levels**: coding is the primary gate while system-design quality decides leveling (L5a/L5b/Senior/Staff). Original non-LeetCode problems appear in "Hack2Hire" assessments. Questions cluster into four families: graphs/BFS-DFS, sliding window/two pointers, heaps/streaming, and cache/design, with domain-flavored twists (quadtrees for geo points, rate limiters, autocomplete).

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Maximize Amount After Two Days of Conversions](https://leetcode.com/problems/maximize-amount-after-two-days-of-conversions) | Medium | Graph / BFS |
| 2 | [Bus Routes](https://leetcode.com/problems/bus-routes) | Hard | Graph / BFS |
| 3 | [Alien Dictionary](https://leetcode.com/problems/alien-dictionary) | Hard | Topological Sort |
| 4 | [Number of Islands II](https://leetcode.com/problems/number-of-islands-ii) | Hard | Union Find |
| 5 | [Design Hit Counter](https://leetcode.com/problems/design-hit-counter) | Medium | Design / Sliding Window |
| 6 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium | Graph / DFS |
| 7 | [Spiral Matrix](https://leetcode.com/problems/spiral-matrix) | Medium | Matrix / Array |
| 8 | [Word Search](https://leetcode.com/problems/word-search) | Medium | Backtracking / DFS |
| 9 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium | Design / HashMap + Linked List |
| 10 | [Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements) | Medium | Heap / Bucket Sort |
| 11 | [Evaluate Division](https://leetcode.com/problems/evaluate-division) | Medium | Graph / Weighted |
| 12 | [Construct Quad Tree](https://leetcode.com/problems/construct-quad-tree) | Medium | Divide and Conquer |
| 13 | [Random Pick with Weight](https://leetcode.com/problems/random-pick-with-weight) | Medium | Prefix Sum / Binary Search |
| 14 | [Find Median from Data Stream](https://leetcode.com/problems/find-median-from-data-stream) | Hard | Two Heaps / Design |
| 15 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium | Sorting / Greedy |
| 16 | [Meeting Rooms II](https://leetcode.com/problems/meeting-rooms-ii) | Medium | Heap / Intervals |
| 17 | [Course Schedule](https://leetcode.com/problems/course-schedule) | Medium | Graph / Cycle Detection |
| 18 | [Course Schedule II](https://leetcode.com/problems/course-schedule-ii) | Medium | Graph / Topological Sort |
| 19 | [Longest Subarray With Absolute Diff <= Limit](https://leetcode.com/problems/longest-continuous-subarray-with-absolute-diff-less-than-or-equal-to-limit) | Medium | Sliding Window / Monotonic Deque |
| 20 | [Squares of a Sorted Array](https://leetcode.com/problems/squares-of-a-sorted-array) | Easy | Two Pointers |
| 21 | [Kth Smallest Element in a BST](https://leetcode.com/problems/kth-smallest-element-in-a-bst) | Medium | BST (O(1)-space Morris follow-up at L5+) |
| 22 | [Group Anagrams](https://leetcode.com/problems/group-anagrams) | Medium | Hash Table |
| 23 | [Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree) | Hard | Tree Encoding |
| 24 | [Design Search Autocomplete System](https://leetcode.com/problems/design-search-autocomplete-system) | Hard | Trie / Design (Uber Eats framing) |

**Custom Problems**: thread-safe token-bucket rate limiter (machine coding); expiry counter (TTL-based driver sessions); geo heatmap builder (aggregate ride pings); driver-rider matching engine; surge pricing calculator; referral revenue tracker; deep equality of nested records; sort a string of clothing sizes ("XS < S < M"); earliest full connectivity timestamp; adaptive bitrate selector.

</details>

## ByteDance / TikTok

<details>
<summary>View 30 Problems (2025-2026 -- High Difficulty)</summary>

ByteDance interviews are among the most technically demanding in the industry. Baseline is Medium, Hard is frequent. Candidates solve 2-3 problems per round (vs 1-2 at Google/Meta). Interviewers write their own problems and progressively mutate them mid-round. Compile-ready, bug-free code expected.

**2026 changes**: The OA was overhauled, switched from HackerRank to **CodeSignal**, multiple-choice removed entirely, now **4 pure coding problems in 70-90 min** (down from ~120 in 2025), with strict proctoring (camera on, screen share, no leaving the window). **AI tools are explicitly banned**: violations mean immediate disqualification. Questions are increasingly scenario-wrapped (file systems, server infrastructure, data pipelines). The hiring-manager round can include an LC-Hard DP under a strict clock.

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Implement Queue using Stacks](https://leetcode.com/problems/implement-queue-using-stacks) | Easy | Stack / Queue / Design |
| 2 | [Daily Temperatures](https://leetcode.com/problems/daily-temperatures) | Medium | Monotonic Stack |
| 3 | [Merge k Sorted Lists](https://leetcode.com/problems/merge-k-sorted-lists) | Hard | Linked List / Heap |
| 4 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium | Design / Hash + Linked List |
| 5 | [Max Consecutive Ones III](https://leetcode.com/problems/max-consecutive-ones-iii) | Medium | Sliding Window |
| 6 | [Sliding Window Maximum](https://leetcode.com/problems/sliding-window-maximum) | Hard | Deque / Sliding Window |
| 7 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium | Graph / DFS / BFS |
| 8 | [Search in Rotated Sorted Array](https://leetcode.com/problems/search-in-rotated-sorted-array) | Medium | Binary Search |
| 9 | [Binary Tree Maximum Path Sum](https://leetcode.com/problems/binary-tree-maximum-path-sum) | Hard | Tree / DFS |
| 10 | [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water) | Hard | Two Pointers / DP |
| 11 | [Course Schedule II](https://leetcode.com/problems/course-schedule-ii) | Medium | Graph / Topological Sort |
| 12 | [3Sum](https://leetcode.com/problems/3sum) | Medium | Two Pointers / Array |
| 13 | [Longest Valid Parentheses](https://leetcode.com/problems/longest-valid-parentheses) | Hard | Stack / DP |
| 14 | [N-Queens](https://leetcode.com/problems/n-queens) | Hard | Backtracking |
| 15 | [Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree) | Hard | Tree / Design |
| 16 | [Kth Largest Element in an Array](https://leetcode.com/problems/kth-largest-element-in-an-array) | Medium | Heap / Quickselect |
| 17 | [Coin Change](https://leetcode.com/problems/coin-change) | Medium | Dynamic Programming |
| 18 | [Regular Expression Matching](https://leetcode.com/problems/regular-expression-matching) | Hard | DP / String |
| 19 | [Longest Increasing Path in a Matrix](https://leetcode.com/problems/longest-increasing-path-in-a-matrix) | Hard | DFS / DP / Topological Sort |
| 20 | [Minimum Difference in Sums After Removal of Elements](https://leetcode.com/problems/minimum-difference-in-sums-after-removal-of-elements) | Hard | Heap / Greedy |
| 21 | [Gas Station](https://leetcode.com/problems/gas-station) | Medium | Greedy |
| 22 | [The kth Factor of n](https://leetcode.com/problems/the-kth-factor-of-n) | Medium | Math |
| 23 | [Zero Array Transformation I](https://leetcode.com/problems/zero-array-transformation-i) | Medium | Prefix Sum / Diff Array |
| 24 | [Maximum Area Rectangle With Point Constraints I](https://leetcode.com/problems/maximum-area-rectangle-with-point-constraints-i) | Medium | Geometry / Hash |
| 25 | [Maximize Amount After Two Days of Conversions](https://leetcode.com/problems/maximize-amount-after-two-days-of-conversions) | Medium | Graph / DFS |
| 26 | [Count Unhappy Friends](https://leetcode.com/problems/count-unhappy-friends) | Medium | Simulation |
| 27 | [Number of Islands II](https://leetcode.com/problems/number-of-islands-ii) | Hard | Union-Find |
| 28 | [K Inverse Pairs Array](https://leetcode.com/problems/k-inverse-pairs-array) | Hard | DP |
| 29 | [Sliding Window Median](https://leetcode.com/problems/sliding-window-median) | Hard | Two Heaps |
| 30 | [Decode Ways II](https://leetcode.com/problems/decode-ways-ii) | Hard | DP |

**Custom Problems**: GPU resource management (job queue + scheduler + monitor with fairness and bin-packing); Server Investment and Round Robin Load Balancer (new 2026 OA); Map Async Limit, middleware `compose()`, and `bind` polyfill (frontend rounds); video chunk scheduler; hashtag trend detector; comment tree flattening; content moderation priority queue; video deduplication via hashing; live viewer count at billion scale.

</details>

## Airbnb

<details>
<summary>View 19 Problems (2025-2026 -- Hardest Difficulty Skew)</summary>

Airbnb's most distinctive rule is **no pseudocode: your code must actually run and pass test cases** in the 45-60 min CoderPad screen. ~33% of reported problems are Hard, with heavy DP and simulation emphasis. Problems arrive dressed as product features (interval merging as overlapping reservation windows). Core values and cross-functional rounds are true gates, not chats.

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Text Justification](https://leetcode.com/problems/text-justification) | Hard | String Simulation |
| 2 | [Maximum Profit in Job Scheduling](https://leetcode.com/problems/maximum-profit-in-job-scheduling) | Hard | DP + Binary Search |
| 3 | [Palindrome Pairs](https://leetcode.com/problems/palindrome-pairs) | Hard | Trie / Hash |
| 4 | [Flatten 2D Vector](https://leetcode.com/problems/flatten-2d-vector) | Medium | Iterator Design |
| 5 | [Combination Sum](https://leetcode.com/problems/combination-sum) | Medium | Backtracking |
| 6 | [Smallest Common Region](https://leetcode.com/problems/smallest-common-region) | Medium | Hash / LCA |
| 7 | [Maximum Candies You Can Get from Boxes](https://leetcode.com/problems/maximum-candies-you-can-get-from-boxes) | Hard | BFS |
| 8 | [Pour Water](https://leetcode.com/problems/pour-water) | Medium | Simulation |
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

**System Design**: Booking/reservation system with time-based availability and strict payment correctness; geo-aware listing search and ranking; notification service; recommendation engine.

</details>

## DoorDash

<details>
<summary>View 17 Problems + AI-Assisted Interview Format (2025-2026)</summary>

DoorDash **publicly rebuilt its engineering interviews around AI**. The new format is a 60-min AI-assisted working session in your own IDE, where free tiers of the common agent tools suffice and all agent features are allowed. You're graded on pragmatic tradeoffs, turning ambiguity into a plan, minimal-repro validation, and narrating reasoning. The policy is transitional: traditional algorithm rounds still ban AI, while the working session mandates it. Loop: **CodeCraft** (build a business module, extend as requirements arrive), **Debugging** (subtle bugs in an unfamiliar codebase), System Design, Behavioral.

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Walls and Gates](https://leetcode.com/problems/walls-and-gates) | Medium | Multi-source BFS |
| 2 | [Shortest Distance from All Buildings](https://leetcode.com/problems/shortest-distance-from-all-buildings) | Hard | Multi-source BFS |
| 3 | [01 Matrix](https://leetcode.com/problems/01-matrix) | Medium | Multi-source BFS |
| 4 | [Maximum Profit in Job Scheduling](https://leetcode.com/problems/maximum-profit-in-job-scheduling) | Hard | DP + Binary Search |
| 5 | [Binary Tree Maximum Path Sum](https://leetcode.com/problems/binary-tree-maximum-path-sum) | Hard | Tree DP |
| 6 | [Basic Calculator](https://leetcode.com/problems/basic-calculator) | Hard | Stack Parsing |
| 7 | [Longest Increasing Path in a Matrix](https://leetcode.com/problems/longest-increasing-path-in-a-matrix) | Hard | DFS + Memo |
| 8 | [Koko Eating Bananas](https://leetcode.com/problems/koko-eating-bananas) | Medium | Binary Search |
| 9 | [Search Suggestions System](https://leetcode.com/problems/search-suggestions-system) | Medium | Trie / Sorting |
| 10 | [Find K Closest Elements](https://leetcode.com/problems/find-k-closest-elements) | Medium | Binary Search |
| 11 | [Ways to Make a Fair Array](https://leetcode.com/problems/ways-to-make-a-fair-array) | Medium | Prefix Sums |
| 12 | [Check if One String Swap Can Make Strings Equal](https://leetcode.com/problems/check-if-one-string-swap-can-make-strings-equal) | Easy | String |
| 13 | [Largest Rectangle in Histogram](https://leetcode.com/problems/largest-rectangle-in-histogram) | Hard | Monotonic Stack |
| 14 | [Making A Large Island](https://leetcode.com/problems/making-a-large-island) | Hard | Union-Find / DFS |
| 15 | [Design HashMap](https://leetcode.com/problems/design-hashmap) | Easy | Design |
| 16 | [Jump Game](https://leetcode.com/problems/jump-game) | Medium | Greedy / DP |
| 17 | [Longest Common Prefix](https://leetcode.com/problems/longest-common-prefix) | Easy | String |

**Custom problems**: Nearest DashMart (multi-source BFS on a city grid); Dasher pay module with rule stacking (CodeCraft); support-ticket workflow automation engine (AI working session); debugging an unfamiliar codebase with planted bugs.

</details>

## Tesla

<details>
<summary>View 25 Problems (2025-2026 -- Greedy + Embedded Focus)</summary>

Greedy and string manipulation are heavily tested (Reorganize String is most-asked). OA is ~85-90 min, 3 problems on Codility. **New in 2026**: take-homes replaced by a ~60-min practical CoderPad screen for many teams, and a shift back toward in-person onsites. **Googling and documentation are allowed; LLM use is at interviewer discretion**: evaluators watch whether you critically review code rather than paste blindly. Questions are team-tied: Autopilot/firmware/energy loops add sensor parsing, state machines, and scheduling. Difficulty across ~47 tracked problems: 8 Easy / 33 Medium / 6 Hard.

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Reorganize String](https://leetcode.com/problems/reorganize-string) | Medium | Greedy / Heap |
| 2 | [Minimum Area Rectangle](https://leetcode.com/problems/minimum-area-rectangle) | Medium | Geometry / Hash |
| 3 | [Find Peak Element](https://leetcode.com/problems/find-peak-element) | Medium | Binary Search |
| 4 | [Maximum Subarray](https://leetcode.com/problems/maximum-subarray) | Medium | Kadane / DP |
| 5 | [Subarray Sum Equals K](https://leetcode.com/problems/subarray-sum-equals-k) | Medium | Prefix Sum |
| 6 | [Reverse Words in a String](https://leetcode.com/problems/reverse-words-in-a-string) | Medium | Strings |
| 7 | [Palindrome Permutation](https://leetcode.com/problems/palindrome-permutation) | Easy | Char Frequency |
| 8 | [Palindrome Linked List](https://leetcode.com/problems/palindrome-linked-list) | Easy | Two Pointers |
| 9 | [Top K Frequent Words](https://leetcode.com/problems/top-k-frequent-words) | Medium | Heap / Hash |
| 10 | [Group Anagrams](https://leetcode.com/problems/group-anagrams) | Medium | Hash / Sorting |
| 11 | [Kth Largest Element in an Array](https://leetcode.com/problems/kth-largest-element-in-an-array) | Medium | Heap / Quickselect |
| 12 | [Task Scheduler](https://leetcode.com/problems/task-scheduler) | Medium | Greedy / Heap |
| 13 | [Sort Colors](https://leetcode.com/problems/sort-colors) | Medium | Dutch National Flag |
| 14 | [Rotate Image](https://leetcode.com/problems/rotate-image) | Medium | Matrix |
| 15 | [Find Pivot Index](https://leetcode.com/problems/find-pivot-index) | Easy | Prefix Sum |
| 16 | [Search in Rotated Sorted Array](https://leetcode.com/problems/search-in-rotated-sorted-array) | Medium | Binary Search |
| 17 | [Design Hit Counter](https://leetcode.com/problems/design-hit-counter) | Medium | Design |
| 18 | [Course Schedule II](https://leetcode.com/problems/course-schedule-ii) | Medium | Topological Sort |
| 19 | [Word Ladder](https://leetcode.com/problems/word-ladder) | Hard | BFS |
| 20 | [Merge k Sorted Lists](https://leetcode.com/problems/merge-k-sorted-lists) | Hard | Heap |
| 21 | [Alien Dictionary](https://leetcode.com/problems/alien-dictionary) | Hard | Topological Sort |
| 22 | [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water) | Hard | Two Pointers |
| 23 | [First Missing Positive](https://leetcode.com/problems/first-missing-positive) | Hard | Arrays |
| 24 | [Minimum Window Substring](https://leetcode.com/problems/minimum-window-substring) | Hard | Sliding Window |
| 25 | [Number of 1 Bits](https://leetcode.com/problems/number-of-1-bits) | Easy | Bit Manipulation (embedded) |

**Embedded/firmware**: interrupt-safe circular buffers in C, CAN bus protocol design, RTOS task scheduling, mutex vs. semaphore, I2C/UART/SPI selection, bitwise register exercises.

**Custom problems**: sensor data parsing (noisy streams), state machine implementation (vehicle/charging states), scheduling simulations from an internal question bank.

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

This repository covers **1,470+ problem listings across 44 companies** (365 unique LeetCode problems, plus 100+ company-specific custom problems that never appear on LeetCode), organized by company and topic, spanning FAANG/MAANG+, frontier AI labs (OpenAI, Anthropic, DeepMind, xAI, Mistral), and AI-first companies (Perplexity, Scale AI, Cursor, Cohere, Waymo, Sierra, Glean). Includes NeetCode 150, Blind 75, system design guides, and ML/AI interview resources.

Every LeetCode link is validated against LeetCode's live problem list.

**[Latest FAANG/MAANG+ Questions](FAANG-Recent-Questions.md)** - Company-by-company breakdown with 2026 process changes and custom (non-LeetCode) problem banks.

**[AI Labs & AI Companies Guide](AI-Companies-Interview-Questions.md)** - 20 AI labs and AI-first companies: interview processes, custom problems, ML coding, and system design.

**[Complete System Design Interview Guide](SYSTEM_DESIGN_INTERVIEW.md)** - 25 system design problems with complexity ratings and company tags.

## Contributing

Contributions are welcome. Please feel free to submit a pull request with new questions, corrections, or additional company coverage.

---

<div align="center">

### 🔔 You Found the Shortcut. Don't Lose It.

New questions, papers, and strategies drop here **every single week**, before they surface anywhere else.

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

## License

GPL-3.0 -- see [LICENSE](LICENSE) for details.
