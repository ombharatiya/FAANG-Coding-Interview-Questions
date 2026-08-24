# Python Programming Language and Resources to Learn

> Click :star: if you like the project. Pull requests are highly appreciated. Follow [@OmBharatiya](https://github.com/ombharatiya) for more updates.

> **More from this repo**: [All guides](./README.md) | [Latest company questions](./FAANG-Recent-Questions.md) | [AI labs](./AI-Companies-Interview-Questions.md) | [System design](./SYSTEM_DESIGN_INTERVIEW.md) | [ML interviews](./ML_INTERVIEW_PREP.md) | [Blind 75](./Blind-75.md) | [NeetCode 150](./NeetCode-150.md)

---

1. ### Best YouTube Channels to Learn
| No. | Channel |
| --- | --------- |
|1  | [Complete Python Tutorial for Beginners by Telusko](https://youtube.com/playlist?list=PLsyeobzWxl7poL9JTVyndKe62ieoN-MZ3) |
|2  | [Python Programming Beginners by Corey Schafer](https://youtube.com/playlist?list=PL-osiE80TeTskrapNbzXhwoFUiLCjGgY7) |
|3  | [Python for Beginners by Mosh](https://youtu.be/_uQrJ0TkZlc) |
|4  | [Python for Beginners in Hindi by CodeWithHarry](https://www.youtube.com/watch?v=aqvDTCpNRek&list=PLu0W_9lII9agICnT8t4iYVSZ3eykIAOME) |


2. ### Best GitHub Learning Resources
| No. | Repository |
| --- | --------- |
|1  | [30 days of Python](https://github.com/Asabeneh/30-Days-Of-Python) : A Step-by-step guide to learn Python programming language in 30 days.|
|2  | [Learn Python](https://github.com/trekhleb/learn-python) : Playground and cheatsheets for learning Python, split by topics and contain code examples with explanations. |
|3  | [Python Mini Projects](https://github.com/Python-World/python-mini-projects): A collection of simple python projects. Archived and read-only since 2022, still useful as practice material |
|4  | [WTF Python](https://github.com/satwikkansal/wtfpython): Explains some counter-intuitive snippets and lesser-known features in Python |
|5  | [Python Basics](https://github.com/learning-zone/python-basics): Python fundamentals and interview questions. The old python-interview-questions repository was renamed to this |
|6  | [Python reference](https://github.com/rasbt/python_reference): Useful functions, tutorials, and other Python-related things. Last updated 2022 |



3. ### Best Udemy Courses
| No. | Course |
| --- | --------- |
|1  | [Complete Python Bootcamp](https://www.udemy.com/course/complete-python-bootcamp/)|
|2  | [Python and Django Full Stack Web Developer Bootcamp](https://www.udemy.com/course/python-and-django-full-stack-web-developer-bootcamp/) |
|3  | [REST APIs with Flask and Python](https://www.udemy.com/course/rest-api-flask-and-python/) |
|4  | [Python A-Z™: Python For Data Science With Real Exercises!](https://www.udemy.com/course/python-coding/) |
|5  | [Python for Finance: Investment Fundamentals & Data Analytics](https://www.udemy.com/course/python-for-finance-investment-fundamentals-data-analytics/) |
|6  | [Machine Learning A-Z™: Hands-On Python & R In Data Science](https://www.udemy.com/course/machinelearning/) |

4. ### Python for Coding Interviews

Python is the most common choice in coding interviews because it keeps solutions short. These are the parts that come up most often.

| Need | Reach for | Note |
| ---- | --------- | ---- |
| Counting | `collections.Counter` | `most_common(k)` solves top-K questions directly |
| Queue or deque | `collections.deque` | O(1) `popleft()`. A plain list is O(n) |
| Heap | `heapq` | Min-heap only. Push `-x` for a max-heap |
| Sorted insert | `bisect` | `bisect_left` and `insort` for ordered arrays |
| Default values | `collections.defaultdict` | Avoids `KeyError` in graph adjacency lists |
| Grouping | `itertools.groupby` | Input must already be sorted by the key |
| Cache | `functools.lru_cache` | One decorator turns recursion into memoised DP |
| Big integers | built-in `int` | No overflow, unlike C++ or Java |

**Idioms interviewers expect to see**

| Instead of | Write |
| ---------- | ----- |
| Manual index loop | `for i, x in enumerate(xs)` |
| Building a list then filtering | A comprehension, or a generator when the input is large |
| Swapping with a temp variable | `a, b = b, a` |
| Nested `if` for bounds | `if 0 <= r < rows and 0 <= c < cols` |
| String concatenation in a loop | `"".join(parts)`, since strings are immutable |

**Things that cost people offers**

- Mutable default arguments: `def f(acc=[])` keeps the same list across calls. Use `None` and create inside.
- Shallow copies: `grid = [[0] * n] * m` makes m references to one row. Use a comprehension.
- Recursion depth: the default limit is 1000, so deep DFS needs an iterative version.
- Sorting cost: `sorted()` is O(n log n), which can quietly break a required O(n) bound.

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

