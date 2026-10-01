# AI Labs & AI Companies. Interview Questions (2025-2026)

> Interview processes, coding questions, ML questions, and system design prompts at the top AI labs and AI-first companies, compiled from 1,500+ candidate reports, engineering blogs, and interview guides (Reddit, Blind, Glassdoor, 1point3acres, LeetCode Discuss, interviewing.io, Exponent, and company sources). For OpenAI and Anthropic deep-dives, see [FAANG-Recent-Questions.md](./FAANG-Recent-Questions.md#openai). Last updated October 2026.

> **More from this repo**: [All guides](./README.md) | [Latest company questions](./FAANG-Recent-Questions.md) | [System design](./SYSTEM_DESIGN_INTERVIEW.md) | [ML interviews](./ML_INTERVIEW_PREP.md) | [Blind 75](./Blind-75.md) | [NeetCode 150](./NeetCode-150.md)

> **Last verified**: October 2026. Several companies below changed owners, CEOs or org structure during 2026 (xAI, Amazon AGI, Groq, Scale AI, Character.AI, Thinking Machines Lab, Cohere). Each affected section carries a dated corporate note, because the loop you get depends on which org the role now reports to.

## Table of Contents

**Frontier Labs**
- [Google DeepMind](#google-deepmind)
- [xAI](#xai)
- [Mistral AI](#mistral-ai)
- [Meta Superintelligence Labs](#meta-superintelligence-labs)
- [Amazon AGI](#amazon-agi)
- [Safe Superintelligence & Thinking Machines Lab](#safe-superintelligence--thinking-machines-lab)

**AI Product & Infrastructure Companies**
- [Perplexity AI](#perplexity-ai)
- [Scale AI](#scale-ai)
- [Cohere](#cohere)
- [Hugging Face](#hugging-face)
- [Cursor (Anysphere)](#cursor-anysphere)
- [Cognition (Devin)](#cognition-devin)
- [Together AI](#together-ai)
- [Groq](#groq)
- [Cerebras](#cerebras)
- [ElevenLabs](#elevenlabs)
- [Waymo](#waymo)
- [Character.AI](#characterai)
- [Sierra AI](#sierra-ai)
- [Glean](#glean)
- [Runway](#runway)
- [Snowflake (AI/Data)](#snowflake-aidata)

**Cross-Industry**
- [2026 AI Interview Trends](#2026-ai-interview-trends)

---

## Google DeepMind

> **Process**: Recruiter screen -> hiring manager screen -> **technical quiz round** (~2 hours: four ~30-min sections on CS fundamentals, mathematics, statistics, and ML, rapid-fire and definition-heavy; veterans fail on forgotten formal definitions like eigenvalues, rank, SVD) -> 2 coding rounds on CoderPad (code is expected to *run*, unlike core Google) -> ML/system design -> paper discussion round (present and defend a paper, sometimes given 2-3 days prior) -> behavioral -> hiring committee. 6-10 weeks total. AI tools prohibited in technical rounds (2026 policy; limited exceptions for some applied roles with recruiter approval). Research Scientist loops reported in mid-2026 run 5-7 rounds of about 60 min each: paper discussion, research problem framing, ML coding, math and theory, distributed-training systems design, evaluation infrastructure, plus a 45-min behavioral.

### Google DeepMind Coding Problems

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Implement Trie (Prefix Tree)](https://leetcode.com/problems/implement-trie-prefix-tree) | Medium | Trie / Design |
| 2 | [Snapshot Array](https://leetcode.com/problems/snapshot-array) (with predefined interface) | Medium | Design |
| 3 | [Find Median from Data Stream](https://leetcode.com/problems/find-median-from-data-stream) | Hard | Heap / Design |
| 4 | [Linked List Cycle](https://leetcode.com/problems/linked-list-cycle) | Easy | Linked List |
| 5 | Paint fence with minimum number of strokes | Medium | Greedy (custom) |
| 6 | Bit-packet encoding/decoding, derive equations for encoding schemes | Hard | Bit Manipulation (custom) |
| 7 | Shortest path in a DAG of model-training task dependencies | Medium | Graph / Topological Sort (custom) |
| 8 | Real-time anomaly detection over a stream of user interactions | Hard | Streaming / Design (custom) |

### Quiz Round Topics (The DeepMind Differentiator)

| No. | Topic | Section |
| --- | ----- | ------- |
| 1 | Define eigenvalues/eigenvectors, matrix rank, singularity, SVD | Mathematics |
| 2 | Differentiate and integrate by hand (chain rule, integration by parts, numerical methods) | Mathematics |
| 3 | Threading, deadlocks, data structures, sorting complexity, networking | Computer Science |
| 4 | Probability puzzles; distributions; expectation | Statistics |
| 5 | Architecture definitions from the Goodfellow *Deep Learning* book; automatic differentiation mechanics | Machine Learning |
| 6 | Regression, SVM/kernel methods, Bayesian networks | Machine Learning |
| 7 | Implement custom losses, attention mechanisms, training loops from scratch without aids | ML Coding |

### Google DeepMind System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Design a training system for a model that does not fit on a single accelerator | Pipeline/tensor parallelism, ZeRO/DeepSpeed |
| 2 | Design evaluation infrastructure | Benchmark contamination, reproducibility |
| 3 | Solve the straggler problem in synchronous training across thousands of GPUs | Distributed training |
| 4 | Design distributed telemetry ingestion from millions of training jobs | Streaming / scale |

---

## xAI

> **Process**: Engineer screen (often no recruiter; "explain your most technical project in 30 seconds") -> **proctored CodeSignal OA** (~60-70 min, camera + mic + screen recording; one problem with five escalating complexity levels) -> 2-3 live coding rounds (practical/production-flavored: class design, iterators, KV stores, caches; one 45-min format = 20 min working solution + 15 min extending to concurrency at "millions of queries") -> system design -> brief behavioral. Fast (2-3 weeks) but scheduling reported as chaotic. Candidates report failing on coding bar, not ML. Python and TypeScript most common. AI-tool policy (single source, techinterview.org, June 2026): coding rounds are generally AI-permissive, but interviewers verify you can explain and extend the code unaided. **Take-home track (Exceptional Engineer and new-grad SWE, Nov 2025 onward)**: recruiter screen (15 min) -> 4-hour take-home -> 60-min onsite coding. The take-home runs in a CodeSignal build environment or your own setup: pick one of six domain prompts spanning xAI products (example: enhance X search through Grok with the Grok API, ideally semantic rather than keyword search; another reported prompt was a "Twitter insight platform"), Grok and X API keys with credits are provided, AI assistants such as Cursor, Claude and Windsurf are encouraged, and you submit a GitHub repo plus a 5-6 minute demo video within 24 hours. The onsite then has you read and extend a 70-100 line class without AI (token queueing, rate limiters, TTL key-value stores, inference batching, LRU caches). The proctored OA is also reported (Aug 2026) as three or four independent problems in 60 minutes with about 150 test cases each and partial credit, alongside the single multi-level variant; some roles add a separate proctored writing assessment.
>
> **Corporate note (2026)**: SpaceX acquired xAI (announced Feb 3, 2026) and renamed the unit SpaceXAI on July 6, 2026, after SpaceX's June 2026 IPO. Grok and X now sit under the SpaceXAI name, so postings and offer letters may carry the SpaceX brand. On May 21, 2026 Musk posted a direct route for the AI unit: email ai_eng@spacex.com with about three bullet points demonstrating exceptional ability, no AI experience required; he says he reads every email that passes a sanity check. Treat it as a side door, not a replacement for the loop above.

### xAI Coding Problems

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | Twitter/X Spaces Active Time, unsorted create/join/leave event logs, compute total active time per Space; follow-ups: users who never leave | Medium | Intervals / Hash Map (custom, signature problem) |
| 2 | [LRU Cache](https://leetcode.com/problems/lru-cache) (edge cases: capacity=1, repeated keys) | Medium | Design |
| 3 | [Word Search II](https://leetcode.com/problems/word-search-ii) (grid vs dictionary, Trie + DFS) | Hard | Trie / Backtracking |
| 4 | In-memory database with nested transactions: SET/GET/BEGIN/ROLLBACK/COMMIT -> persistence -> concurrency | Medium-Hard | Design (custom, multi-level) |
| 5 | Implement a simplified LLM inference engine: request batching, per-batch inference, token-level result collection | Hard | ML Systems (custom) |
| 6 | Production code with concurrency added on the spot | Hard | Concurrency (custom) |
| 7 | [Course Schedule](https://leetcode.com/problems/course-schedule) (cycle detection) | Medium | Graph |
| 8 | Efficient beam search implementation | Hard | ML Algorithms (custom) |
| 9 | Tetris-block placement: drop an ordered list of block shapes into a grid of given width, return how many blocks land before the grid jams (proctored OA, Aug 2026) | Medium | Grid Simulation (custom) |
| 10 | Count subsequences that sum exactly to a target, answer modulo 10^9+7 (proctored OA, Aug 2026) | Medium | DP / Knapsack |
| 11 | Busiest 60-second window over a list of event timestamps (proctored OA, Aug 2026) | Easy-Medium | Sliding Window |
| 12 | Per-key fixed-window cost limiter: ALLOW key cost timestamp (accept only if window usage + cost <= limit; rejections record nothing) and RESET key; timestamps to 10^15, 200K commands (Sep 2026) | Medium | Design / Hash Map (custom) |
| 13 | Hand-write a parallel sort using multiple worker threads or processes; multithreading is mandatory (Sep 2026; also Jan 2026) | Medium-Hard | Concurrency |
| 14 | Token queueing: extend a provided 70-100 line class that handles LLM input so it splits the input into token-sized chunks and returns the output queue (onsite, no AI tools) | Medium | Code Extension (custom) |
| 15 | React typeahead with async suggestions, arrow/Enter/Escape navigation, stale-result and race handling, no third-party libraries (Sep 2026); also seen as an offline autocomplete box over thousands of rows in one local file (Jun 2026) | Medium | Frontend |

### xAI ML Questions

| No. | Topic | Category |
| --- | ----- | -------- |
| 1 | Why Transformers beat RNNs for LLMs; core Transformer components | Architecture |
| 2 | Data parallelism vs model parallelism for 100B+ models; tensor vs pipeline parallelism, pipeline-bubble management | Distributed Training |
| 3 | Memory-efficient training of billion-parameter models; CUDA kernel acceleration | Systems |
| 4 | Efficient attention for 100K-token contexts | Architecture |

### xAI System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Design a distributed rate limiter for an API gateway at 100k req/s across multiple instances | Per-user/per-IP limits, cross-node consistency |
| 2 | Real-time inference serving at 100,000 req/s | GPU serving, batching |
| 3 | Data pipeline for massive text-dataset ingestion/training | Data infrastructure |
| 4 | Real-time logging system for model inference | Observability |
| 5 | Design and implement a URL shortening service: short-code generation, redirect path, scaling | New-grad design round, Jul and Sep 2026 |

---

## Mistral AI

> **Process**: Recruiter screen -> technical screen (60 min, one medium-hard problem in Python/Rust; C++/CUDA for some roles) -> take-home for select/research roles (4-8h; design a small LLM/agent experiment, write-up judged with academic-paper expectations) -> **LLM knowledge quiz** (45-75 min structured deep-dive) -> system design (AI-infrastructure flavored) -> behavioral/values. Research roles add a research presentation with 20+ min of hard questioning. Ground "why Mistral" in the open-weight mission; read the Mistral 7B/Mixtral/Codestral papers plus the newer release notes: Mistral Large 3 (Dec 2025, sparse MoE, 675B total / 41B active, 256K context), Ministral 3 and Devstral 2 (Dec 2025), Mistral Small 4 (Mar 2026, merges the Magistral reasoning, Pixtral vision and Devstral coding lines) and Mistral Medium 3.5 (Apr 2026). MLE technical screens reported in Jul 2026 pair a small build (an agent or RAG tool on the Mistral API) with a defense of retrieval quality, orchestration, latency, evaluation and production boundaries, and SWE onsites add probability and logic puzzles under time pressure.

### Mistral AI Coding Problems

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | Implement top-k and top-p (nucleus) sampling from scratch, no libraries | Medium | ML Coding |
| 2 | Write a BPE-style tokenizer (~50 lines) from vocab + corpus | Medium | ML Coding / Strings |
| 3 | Implement multi-head attention from scratch (correct PyTorch math) | Hard | ML Coding |
| 4 | Implement KV-cache management for batched inference | Hard | Inference Systems |
| 5 | Implement a sliding-window attention mask | Medium | ML Coding |
| 6 | Debug a 300-line Python file with a subtle bug in 30 min (bug in attention masking, sampling, or batching) | Hard | Debugging |
| 7 | Parallelize an embedding lookup across 4 workers | Medium | Distributed |
| 8 | Batch API calls efficiently, minimize latency, handle edge cases | Medium | Applied Coding |
| 9 | Stream-process large datasets with bounded memory | Medium | Streaming |
| 10 | Classic graph/DP/priority-queue problems with ML-applied twists | Medium-Hard | Algorithms |
| 11 | Nearest-center assignment (the k-means assignment step) for N points and K centers without materializing the N x K x D distance tensor; broadcasting vs memory trade-offs (MLE onsite, Jul 2026) | Medium | ML Coding / Numerics |
| 12 | Multi-threaded load balancer with pluggable balancing strategies | Medium-Hard | Concurrency / Design |
| 13 | Intersection of two very large sorted lists of user IDs | Medium | Two Pointers / Streaming |

### Mistral AI ML Questions

| No. | Topic | Category |
| --- | ----- | -------- |
| 1 | MoE: routing, load-balancing loss, top-k expert selection, "why does Mixtral use 2 of 8 experts per token?" | Architecture |
| 2 | FlashAttention vs sliding-window attention vs grouped-query attention, when each helps | Architecture |
| 3 | "How would you debug a loss spike at step 40k?" | Training |
| 4 | DPO vs PPO vs RLHF: when would you use each? | Alignment |
| 5 | Quantization (int8/int4, GPTQ, AWQ) and its quality costs | Inference |
| 6 | Paged attention / KV-cache layout; speculative decoding (draft models, acceptance rates) | Inference |
| 7 | Continuous vs static batching; non-linear throughput-latency trade-offs | Inference |
| 8 | Data mixing, curriculum, LR schedules; scaling laws | Training |
| 9 | "How would you build an eval suite for a Codestral-class model?" | Evaluation |
| 10 | Implement RMSNorm in PyTorch and explain why current LLMs prefer it over LayerNorm; MHA vs GQA vs MQA memory and compute trade-offs | Architecture |
| 11 | Probability and logic puzzles under time pressure: structured reasoning, stated assumptions, clean communication (SWE onsite, Jul 2026) | Statistics / Math |

### Mistral AI System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Design the inference-serving system for a 70B MoE model at 10K req/sec with p95 < 1 sec | GPU serving |
| 2 | Design the training pipeline for a 70B dense model across 2K H100 GPUs | Distributed training |
| 3 | Design La Plateforme's multi-tenant API with fair rate-limiting, per-customer quotas, cost tracking | API platform |
| 4 | Design an enterprise on-premise deployment with model updates, A/B testing, data-sovereignty guarantees | Enterprise |
| 5 | Deploy across 3 EU regions with data residency; handle a 10x traffic spike | Operations |

---

## Meta Superintelligence Labs

> **Process**: MSL research hiring is a distinct track, initial ~50-person team recruited by mining most-cited paper authors, with Zuckerberg personally interviewing; candidates tested on ability to identify and quantify gaps in current AI models. Engineering roles follow the standard Meta loop **plus the AI-enabled coding round** (piloted Oct 2025, rolled out across back-end and ops-focused roles through 2026; E6 and below get one traditional coding round plus one AI-enabled round, E7 and above get a single coding round that is AI-enabled): 60 min in a 3-panel CoderPad (file explorer, editor, AI chat with GPT-4o mini, GPT-5, Claude Sonnet 4/4.5, Claude Haiku 4.5, Gemini 2.5 Pro and Llama 4 Maverick, switchable mid-session; AI reads files but cannot edit). Three phases: (1) find/fix a non-algorithmic bug, (2) build a 120+ line feature with AI expected, (3) optimize for larger datasets. Rubric: Problem Solving, Code Quality, **Verification** (test before trusting AI output), Communication. Candidates report the in-interview AI is "nerfed" vs practice environments.

### AI-Enabled Round Problems (~9 in rotation)

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | Maze Solver with Path Printing (multi-phase, directional gates) | Medium-Hard | AI-Assisted Coding |
| 2 | Maximize Unique Characters from Word List | Medium | AI-Assisted Coding |
| 3 | Card Game: Find Three Cards Summing to 15 | Medium | AI-Assisted Coding |
| 4 | Friend Recommendation System (build + optimize) | Medium-Hard | Graphs / AI-Assisted |
| 5 | Multi-file project: debug + extend (shell scripts, Dockerfiles, API endpoints) | Medium-Hard | Practical |

See [Meta in FAANG-Recent-Questions.md](./FAANG-Recent-Questions.md#meta-formerly-facebook) for the standard coding-round question bank.

---

## Amazon AGI

> **Process**: Reported loop (2025 reports): phone screen covering coding + system design + backend tasks + Leadership Principles. Onsite for ML roles: coding, ML application/design, behavioral with heavy LP emphasis, bar raiser in the loop. The Nova team follows the standard Amazon AGI / Applied Scientist process. ML coding style compared by candidates to OpenAI's.
>
> **Corporate note (2026)**: Rohit Prasad left at the end of 2025 and the AGI org was folded into a new organization under Peter DeSantis that combines frontier models, custom silicon (Trainium, Graviton, Nitro) and quantum; Pieter Abbeel leads frontier-model research. David Luan (ex-Adept) left the AGI Lab in Feb 2026, and in July 2026 Amazon confirmed it is closing the San Francisco AGI Lab site while cutting roles across the AGI org (AGI Data Services, AGI Information). Nova 2 Lite, Nova 2 Sonic, Nova Forge and Nova Act stay active. Expect roles to be posted under AGI, AWS or the DeSantis org rather than "AGI SF Lab".

### Amazon AGI Reported Problems

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | Debug a broken Transformer implementation | Hard | ML Coding |
| 2 | Build/train a small classifier live | Medium | ML Coding |
| 3 | Reinforcement learning fundamentals + coding | Medium-Hard | ML |
| 4 | Standard LC coding + backend task in phone screen | Medium | DSA / Practical |

See [Amazon in FAANG-Recent-Questions.md](./FAANG-Recent-Questions.md#amazon) for the standard question bank.

---

## Safe Superintelligence & Thinking Machines Lab

> **Safe Superintelligence (SSI)**: No public interview-question data exists, consistent with extreme secrecy. Credibly reported: in-person candidates must place phones in a Faraday cage before entering SSI offices; about 50 employees (July 2025) split between Palo Alto and Tel Aviv; hiring is network-driven; staff discouraged from listing SSI on LinkedIn. No OA platform, loop structure, or question bank has leaked. Corporate facts: co-founder Daniel Gross left for Meta Superintelligence Labs in July 2025 and Ilya Sutskever became CEO; on July 27, 2026 Nvidia announced a $5B investment with priority access to its Vera Rubin platform, taking SSI to about $7B raised at a $32B post-money valuation.
>
> **Thinking Machines Lab**: Founded Feb 2025; $2B seed at a $12B valuation (July 2025). Hires heavily through networks around the **Tinker** fine-tuning API (launched Oct 1, 2025, general availability Dec 2025) and the Inkling model (July 2026); postings list Research Engineer/SWE at $350K-$500K. Reported loop (thin, single-source): recruiter screen -> hiring manager -> research/coding interview -> cross-functional panel. No verified question bank yet. Leadership churn to factor in: four of six co-founders have left (Andrew Tulloch to Meta, late 2025; CTO Barret Zoph dismissed Jan 2026 and Luke Metz, both to OpenAI; Lilian Weng left July 29, 2026 and rejoined OpenAI). Soumith Chintala is CTO, John Schulman remains Chief Scientist. As of Sept 2026 the lab was in talks for a $5-6B round at a $40B+ pre-money valuation (Accel, Nvidia). Note: Glassdoor's "Thinking Machines" entry is a Manila data-science consultancy, different company.

---

## Perplexity AI

> **Process**: Recruiter screen (45 min) -> technical phone screen (~45 min coding) -> virtual onsite 4-5 rounds (coding, system design, infrastructure, hiring-manager deep dive) -> final round with a **founder/senior leader**. Very fast: ~11-23 days end-to-end; resume-to-first-interview within three business days. OA on HackerRank/CodeSignal (75-90 min, 2-3 questions). Python strongly preferred (codebase is Python-first). Evaluated on production-ready code, edge cases, velocity, RAG/search-domain reasoning. Guides updated July 2026 describe the loop as 4-6 rounds including a search and ML systems deep-dive and a **product and craft round** ("What makes a Perplexity answer great vs mediocre?", "How would you evaluate an answer's citation quality?"); Blind threads from September 2026 confirm full loops are running but share no new problems.

### Perplexity AI Coding Problems

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Design In-Memory File System](https://leetcode.com/problems/design-in-memory-file-system) | Hard | OOP / Design |
| 2 | [Time Based Key-Value Store](https://leetcode.com/problems/time-based-key-value-store) | Medium | Design / Binary Search |
| 3 | Credit Tracker with expiring credits (CreditTracker class) | Medium | Design / State (custom) |
| 4 | Byte Tokenizer (implement a tokenizer) | Medium | Strings / ML (custom) |
| 5 | Probability of each number appearing in a stream | Medium | Math / Streaming (custom) |
| 6 | LLM provider pool with automatic failover/fallback logic | Medium-Hard | Design / Concurrency (custom) |
| 7 | Remove duplicate/near-duplicate documents from a stream | Medium-Hard | Hashing / Streaming (custom) |
| 8 | Sequence batching for embedding requests | Medium | ML Infra (custom) |
| 9 | Implement beam search | Medium-Hard | ML Algorithms (custom) |
| 10 | Substring extraction before stop words under streaming memory constraints | Medium | Strings / Streaming (custom) |
| 11 | Ranking function balancing relevance, freshness, source quality | Medium | Ranking / Heaps (custom) |
| 12 | [Search Suggestions System](https://leetcode.com/problems/search-suggestions-system) | Medium | Trie / Strings |
| 13 | [Implement Trie (Prefix Tree)](https://leetcode.com/problems/implement-trie-prefix-tree) | Medium | Trie |
| 14 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium | Design |
| 15 | [Logger Rate Limiter](https://leetcode.com/problems/logger-rate-limiter) | Easy | Design / Hash |
| 16 | [Find Median from Data Stream](https://leetcode.com/problems/find-median-from-data-stream) | Hard | Heap / Streaming |
| 17 | [Minimum Window Substring](https://leetcode.com/problems/minimum-window-substring) | Hard | Sliding Window |
| 18 | Time-versioned key-value store with restore: deletes are recorded as events and can be undone; timestamp queries return the nearest stored value (also set as a take-home for infra roles) | Medium | Design / Binary Search (custom, 2026) |
| 19 | Dependency-aware to-do list: tasks with state transitions and dependencies, detect or reject cycles; the problem grows a part at a time as you finish each | Medium | Design / Graphs (custom, 2026) |
| 20 | Task dependencies with failure propagation: compute run order and mark downstream tasks failed or skipped when a dependency fails | Hard | Graphs / Topological Sort (custom, 2026) |
| 21 | In-memory file system, strict variant: mkdir, touch, ls, rm, rmdir with error handling plus a command runner that executes a script of commands | Hard | OOP / Design (custom, Sept 2026) |

### Perplexity AI ML/AI Questions

| No. | Topic | Category |
| --- | ----- | -------- |
| 1 | RAG end-to-end: retrieval -> context assembly -> generation with citations; chunking, dense vs sparse (BM25) vs hybrid retrieval, re-ranking | RAG |
| 2 | Hallucination mitigation and context-window management | LLM |
| 3 | SFT vs RLHF vs DPO, when would you choose one over another | Alignment |
| 4 | "How do you know Model A beats Model B for search?", calibration, factuality, A/B design | Evaluation |
| 5 | Cost/latency optimization of LLM serving (token budgets, caching, concurrency) | Inference |

### Perplexity AI System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | "Design a system that knows about something that happened 30 minutes ago" | Real-time crawling, event detection, cache invalidation |
| 2 | Design a recommender system for Perplexity's Discover page | Recommendations |
| 3 | Design a personal finance platform syncing spend data from multiple credit-card accounts | Integrations |
| 4 | Kubernetes infrastructure debugging: system overloaded, debug via metrics | Infrastructure |
| 5 | Design a long-running query service: submit, poll, stream partial results, cancel, retry | Async jobs, job state storage, timeouts (Sept 2026) |

---

## Scale AI

> **Process**: Recruiter screen -> HackerRank OA / technical screen (~60 min, 2 mediums) -> hiring-manager screen -> virtual onsite 4-5 rounds: coding, **backend practical**, **debugging round** (unfamiliar multi-file codebase, find/fix 2-3 logical bugs in 60 min), system design or ML, and "Credo" behavioral. Explicitly "not standard LeetCode", implementation-heavy, production realism, speed and working code over algorithmic cleverness. New-grad reports from early 2026 (Aced) describe the phone screen as two interval-style problems in one hour with input delivered through API-style methods, graded on speed and clean syntax; one interviewer described the culture as "pretty like 996". PracHub entries dated July and August 2026 show the backend-practical and four-player card-game rounds still in rotation.
>
> **Corporate note (2026)**: Meta bought a 49% stake in June 2025 and Alexandr Wang left to run Meta Superintelligence Labs; Scale cut about 14% of staff in July 2025. Jason Droege ran the company as interim CEO until Francis deSouza (ex-Google Cloud COO, ex-Illumina CEO) took over on Aug 10, 2026. Growth is now in applied and forward-deployed work plus public-sector contracts, so 2026 system-design and hiring-manager rounds orbit "help an enterprise or agency stand up its own AI": eval harnesses for fine-tuned models, throughput and backpressure, idempotency, and measuring label quality without ground truth.

### Scale AI Coding Problems

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | **Card game simulation**: model a card game (N players, rules, state transitions) in 60 min; follow-ups add jokers/wildcards or variants | Medium-Hard | OOP / Design (signature question) |
| 2 | Dependency-aware task scheduler (AddTasks/ConsumeTask in deadline order) | Hard | Design / Heaps / Graphs (custom) |
| 3 | Lightweight load balancer (worker state machine, task dispatch, heartbeat, failover) | Medium-Hard | Backend Practical (custom) |
| 4 | Debug a project-assignment codebase (multi-file, CSV fixtures) | Medium | Debugging (custom) |
| 5 | CSV upload endpoint calling a GPT-like classification API | Medium | Backend / ML Integration (custom) |
| 6 | Update a Neuron Grid (firing/non-firing neurons) | Medium | Matrix / Simulation (custom) |
| 7 | [Lowest Common Ancestor of a Binary Tree](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-tree) (given only children lists) | Medium | Trees |
| 8 | [Subarray Sum Equals K](https://leetcode.com/problems/subarray-sum-equals-k) | Medium | Prefix Sum / Hash |
| 9 | [Gas Station](https://leetcode.com/problems/gas-station) | Medium | Greedy |
| 10 | [Moving Average from Data Stream](https://leetcode.com/problems/moving-average-from-data-stream) | Easy | Queue / Streaming |
| 11 | [Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self) | Medium | Arrays |
| 12 | [Squares of a Sorted Array](https://leetcode.com/problems/squares-of-a-sorted-array) | Easy | Two Pointers |
| 13 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) (most frequently surfaced topic) | Medium | Intervals |
| 14 | Given a stream of labeling events, return the k most frequent labels in the last hour | Medium | Heap / Sliding Window (custom, 2026) |
| 15 | Merge overlapping annotation spans and report total coverage | Medium | Intervals / Sweep (custom, 2026) |
| 16 | Parse a nested config and validate it against a schema (null and type handling) | Medium | Recursion / Parsing (custom, 2026) |
| 17 | Party-hours intervals: given per-neighborhood party intervals through API-style getters, compute covered time blocks per neighborhood and the gaps across the town or city (two parts; also seen as the HackerRank OA) | Medium | Intervals / API-style input (custom) |
| 18 | Free-window finder for query ingestion: given query time intervals, return idle windows and order them to minimize LLM processing time; follow-up is meeting-room style availability from API input | Medium | Intervals / Sorting (custom, 2026) |
| 19 | CSV-to-JSON classification service: read a CSV, call a classification and embedding API, write JSON results (2026 backend-practical form of the CSV upload question) | Easy-Medium | Backend Practical (custom, July 2026) |
| 20 | Debug a 150-200 line modular pipeline whose model output is wrong; the bug is in hashing logic that inflates token costs | Medium | Debugging (custom, 2026) |

### Scale AI ML/AI Questions

| No. | Topic | Category |
| --- | ----- | -------- |
| 1 | Transformers, attention, decoding strategies, RLHF, evaluation, optimization | LLM Fundamentals |
| 2 | LLM post-training methods and trade-offs (SFT/RLHF/DPO pipeline for a base model) | Post-Training |
| 3 | Adversarial attacks; evaluation and deployment failure modes; pipeline debugging | Robustness |
| 4 | Human-in-the-loop labeling quality: automated + human evaluation frameworks | Data Quality |

### Scale AI System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Design a streaming job scheduler (continuous task ingestion + dispatch) | Scheduling |
| 2 | Design an LLM API pipeline (hosted LLM APIs resolving user tasks) | LLM Integration |
| 3 | Design a data-annotation/labeling pipeline; LLM evaluation system | Core Domain |
| 4 | Design a large-scale ticketing system (high concurrency) | Distributed Systems |
| 5 | Design a durable task scheduling service (persisted tasks, retries, exactly-once execution, worker failure) | Durability / Idempotency (July 2026) |
| 6 | Design the backend for an insurance-claims agent: ingest claims from emails and PDFs, extract fields with RAG, decide or route, keep LLM token cost under control | Applied LLM / Cost (2026) |
| 7 | Design an embedding and classification API shared by many internal callers | ML Serving (July 2026) |

---

## Cohere

> **Process**: Recruiter screen -> technical screen (60 min live coding, **Python or Go**) -> ML round or system design (team-dependent) -> behavioral -> team match. ~4-6 weeks. Style: production-quality infrastructure code over LeetCode tricks, "no segment trees, advanced DP, or competitive programming." Tests-first, edge cases, explicit concurrency/locking. MLE track adds a ~3-hour assessment spanning language modelling, math for ML, and coding, plus numpy ML coding and a research presentation. **2026 loop change (Blind, Sept 2026, SWE and FDE loops including a Europe-based agentic team)**: no LeetCode rounds. Recruiter screen -> two HackerRank OAs that are not LeetCode style -> hiring manager -> system design -> **problem-solving round** (root-cause a failing system by forming hypotheses and eliminating causes, then propose remediation) -> **AI-enabled coding round** (CodeSignal, 45 min for FDE, an existing Python codebase with an AI assistant available; the SWE version was "implement an agent loop with tool-call parsing"). One candidate reported the interviewer reacted poorly to leaning on the AI, so validate generated code out loud.
>
> **Corporate note (2026)**: Cohere agreed to merge with Germany's Aleph Alpha on April 24, 2026, with Schwarz Group leading a roughly $600M Series E; the combined company is valued at about $20B and the close is expected later in 2026 pending approvals. Cohere reported $240M ARR for 2025. Sovereign-cloud and on-premise deployment (the combined entity is expected to run on Schwarz Digits' STACKIT) is now core to the pitch, so prepare it alongside the RAG and Command material.

### Cohere Coding Problems

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | Token rate limiter: N tokens/sec per customer, sliding-window semantics, thread-safe | Medium | Concurrency / Design (custom) |
| 2 | Request batch aggregator: batch inference requests up to size 32 or 50 ms wait | Medium | Concurrency / Systems (custom) |
| 3 | [LRU Cache](https://leetcode.com/problems/lru-cache) with TTL expiry | Medium | Design |
| 4 | Streaming response parser handling partial chunks | Medium | Strings / Systems (custom) |
| 5 | Retry-with-backoff; token bucket implementations | Easy-Medium | Systems Utilities (custom) |
| 6 | Create a dataset for sentence completion using BERT | Medium | ML Coding (custom) |
| 7 | ML coding with numpy (implement model components) | Medium-Hard | ML Coding (custom) |
| 8 | AI-enabled coding round: implement an agent loop that parses tool calls, executes tools and loops until done, with an AI assistant available; graded on how you validate the generated code | Medium | Agents / AI-Assisted (custom, Sept 2026) |
| 9 | Problem-solving round: given a failing production system, walk through it step by step, form hypotheses and eliminate causes until you find the failure, then propose remediation | Medium | Debugging / Systems (custom, Sept 2026) |
| 10 | FDE: 45-minute CodeSignal session on an existing Python codebase with an AI tool available (fix or extend) | Medium | AI-Assisted Coding (custom, Sept 2026) |
| 11 | [Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters) with a streaming-input follow-up | Medium | Sliding Window |

### Cohere ML/AI Questions

| No. | Topic | Category |
| --- | ----- | -------- |
| 1 | RAG pipeline failure modes; chunking strategies; when BM25 beats dense embeddings | RAG |
| 2 | Embedding evaluation: NDCG, MRR, recall@k; multilingual retrieval; when to fine-tune embeddings | Evaluation |
| 3 | LoRA vs full fine-tune; mitigating catastrophic forgetting | Fine-Tuning |
| 4 | "Build an eval suite for our Rerank model on a new vertical" | Evaluation |
| 5 | "Fine-tune Command for a regulated industry where hallucinations cost the customer money" | Applied |
| 6 | Attention mathematics, write the equation; encoder-only vs decoder-only vs encoder-decoder | Architecture |

### Cohere System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Multi-tenant inference platform on a shared GPU fleet: Customer A needs 50ms p95, Customer B runs overnight batch embeddings, Customer C does RAG with strict data isolation | GPU economics, latency budgets, isolation, cost-per-query |
| 2 | Inference servers, fine-tuning pipelines, eval harnesses, customer-facing APIs | Platform |

---

## Hugging Face

> **Process**: Application review (cover letter explicitly weighted, passion for open source) -> recruiter screen -> 1-2 conversational technical interviews (~60 min) -> **take-home project** for junior/intern roles (build a HF Spaces demo, dataset card project, or fix a bug in their OSS tooling) with follow-up presentation; senior roles get architecture discussions or a "job talk." Open-source track record (PRs to HF repos) counts heavily. De-emphasizes rote algorithm memorization. Note: interview data volume is low. Treat specifics as low-sample.

### Hugging Face Coding Problems

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Merge Two Sorted Lists](https://leetcode.com/problems/merge-two-sorted-lists) | Easy | Linked List |
| 2 | [Missing Number](https://leetcode.com/problems/missing-number) | Easy | Math / Bit |
| 3 | SQL: select 2nd highest salary in the engineering department | Easy-Medium | SQL |
| 4 | Take-home: build a Hugging Face Spaces demo / dataset card project | Medium | Applied ML Project (custom) |
| 5 | Fine-tune a BERT model end-to-end; build an inference pipeline | Medium | Applied ML (custom) |

### Hugging Face ML/AI Questions

| No. | Topic | Category |
| --- | ----- | -------- |
| 1 | "What innovative approaches do you envision for enhancing transformer efficiency and performance?" | Architecture |
| 2 | Fine-tuning workflows with the HF Trainer API; dataset preprocessing, training loops, evaluation metrics | Applied ML |
| 3 | Your open-source contributions and how you'd contribute to specific HF projects | Open Source |

---

## Cursor (Anysphere)

> **Process**: Recruiter/manager screen (covers "why Cursor" and tolerance for heavy workload) -> 1-3 technical phone screens (60 min, one medium-hard problem, sometimes against part of Cursor's actual codebase) -> **paid onsite project: 8-9 hours** (CEO Michael Truell told Business Insider in Nov 2025 that every engineering and design hire does a two-day onsite trial with a desk, a laptop and a frozen copy of the codebase; real codebase access, a Slack channel, build a feature autonomously, meals with the team, ending with a presentation, this round decides the offer) -> culture-fit discussion (often over meals). Some senior/staff roles get a 4-8h take-home. AI tools: reports conflict. Some say unrestricted AI in all rounds, others say prohibited in the first coding round; all agree pasting raw model output without judgment is a fast rejection. Languages: TypeScript (editor), Rust (perf-critical), Python (ML). **Updates through October 2026**: the Aced candidate guide describes AI access as staged (autocomplete only in the earliest screen, targeted syntax help in coding rounds, open at the onsite) and says some candidates get a roughly 8-hour remote version of the two-day in-person project; a candidate interviewing in late September 2026 said Cursor had "recently changed their onsite loop" but gave no details. July 2026 job postings describe the loop only as "two to three short technical interviews, then an onsite in the office where you build a small project, discuss ideas, and meet the team", with no mention of pay or a take-home. April 2026 frontend-loop reports: one medium-hard practical problem per round plus one or two follow-ups, each tied to a part of Cursor, and backchannel reference checks after the onsite.

### Cursor Coding Problems

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Find Duplicate File in System](https://leetcode.com/problems/find-duplicate-file-in-system) | Medium | Hash / Strings |
| 2 | Print the top view of a binary tree | Medium | Tree / BFS |
| 3 | Build a hash tree (Merkle tree) to organize repository data | Medium-Hard | Trees / Hashing (custom) |
| 4 | Implement a syntax-aware edit operation | Medium-Hard | Editor Primitives (custom) |
| 5 | Handle streaming LLM output / apply streaming edits as tokens arrive | Medium-Hard | Streaming / Async (custom) |
| 6 | Model a file-tree diff / multi-file diff tracking | Medium-Hard | Data Modeling (custom) |
| 7 | Build a context-retrieval system for LLM prompts | Medium-Hard | Applied AI (custom) |
| 8 | Text-buffer primitives with efficient edit operations (rope-style structures) | Hard | Data Structures (custom) |

### Cursor System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Design Cursor's tab-prediction system with sub-100ms latency end-to-end for millions of users | Latency / ML serving |
| 2 | Design Cursor's agent mode executing multi-file edits with verification and rollback | Agents |
| 3 | Design the privacy-preserving inference architecture keeping enterprise code confidential | Privacy |
| 4 | Design the custom-model training pipeline producing coding-specialized variants | Training |

---

## Cognition (Devin)

> **Process**: Cognition (Devin, Windsurf) closed a $2B Series E at a $48B valuation on Sep 8, 2026, with run-rate revenue near $900M and new offices in Washington DC, Tokyo, Singapore, London, Sao Paulo and Madrid, so H2 2026 is a heavy hiring period. The company publishes no loop; 2026 reports agree on: recruiter or hiring-manager call (30 min) -> live coding screen (60 min, practical coding and adapting to unfamiliar tools, not LeetCode) -> final round of three to five sessions in one block (deeper coding, systems, behavioral) -> for many engineering roles an extended practical challenge of 6 to 8 hours that CEO Scott Wu describes as having candidates "build their own Devin in eight hours". Forward-deployed engineer roles replace coding and system design with a take-home done inside Devin itself (minimal code, drive the product like a customer), a 45-min project presentation to a non-technical panel, leadership 1:1s, a simulated executive pitch and a timed case-study customer call. San Francisco, in-person preferred, usually 3+ years of experience; decisions often land within days of the final round. AI policy is set per stage: confirm with recruiting whether the exercise is algorithmic, repository-based or project-based and which tools are permitted. The recurring signal in every round is judgment under ambiguity, explained in about 30 seconds.

### Cognition Reported Problems and Topics

| No. | Problem or Topic | Difficulty | Category |
| --- | ---------------- | ---------- | -------- |
| 1 | Parse a stream of tool-call outputs, reconcile state after a step fails, write the retry logic | Medium-Hard | Agents / State Machines (custom) |
| 2 | Build a small in-memory file system an agent can read and write against | Medium-Hard | Design (custom) |
| 3 | Implement a token-budget tracker that evicts the least useful context | Medium | Cache / Eviction (custom) |
| 4 | Diff two versions of a directory tree | Medium | Trees / Hashing (custom) |
| 5 | 60-minute repository change: inspect before editing, state the invariant, make the smallest patch, run narrow tests, review the diff | Medium | Repository Coding |
| 6 | Build your own coding agent from scratch in 6 to 8 hours | Hard | Extended Practical Challenge |
| 7 | "An agent loops between two failed approaches. What do you do?" | Discussion | Agent Debugging |
| 8 | "How do you know an agent solved a coding issue?", then design a benchmark for repository-level agents | Discussion | Evaluation |
| 9 | When should Devin ask for confirmation rather than continue autonomously | Discussion | Product Judgment |

### Cognition LeetCode Practice (Mapped to Reported Topics)

| No. | Question | Difficulty | Category |
| --- | -------- | ---------- | -------- |
| 1 | [Design In-Memory File System](https://leetcode.com/problems/design-in-memory-file-system) | Hard | Design (premium) |
| 2 | [LFU Cache](https://leetcode.com/problems/lfu-cache) | Hard | Eviction policy |
| 3 | [Find Duplicate File in System](https://leetcode.com/problems/find-duplicate-file-in-system) | Medium | Directory trees / hashing |
| 4 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium | Design |
| 5 | [Course Schedule II](https://leetcode.com/problems/course-schedule-ii) | Medium | Dependency ordering |

### Cognition System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Design the execution environment Devin runs inside (the signature question, about 45 min) | Sandboxing, secrets and permissions, long-running task state, rollback |
| 2 | Design a secure execution environment for an agent modifying a repository | Isolation, least privilege, audit |
| 3 | Design a benchmark and evaluation pipeline for repository-level coding agents | Contamination, flaky tests, scoring at scale |
| 4 | Keep model-call cost and latency bounded for long-running agent sessions | Caching, context budgets, early stopping |
| 5 | Project onsite prompts: brainstorm a product idea with AI, then design an agentic system that adapts to new tasks; how would you handle hallucinations in a model deployed to users | Agents / Product (2026) |

---

## Together AI

> **Process**: Recruiter screen -> technical phone screen (60 min, one medium-hard problem in Python/C++/CUDA) -> take-home for senior/research roles (4-8h; CUDA kernel implementation for inference roles) -> onsite 4-5 rounds: two coding (algorithms + applied ML-systems), system design, one or two ML/research rounds, behavioral -> VP round. ~3 weeks. Real CUDA fluency expected for inference-engine roles (difficulty compared to NVIDIA core GPU teams). **Infra/SRE track (2026)** is separate from the CUDA path: a 60-minute technical round in your own IDE, Linux and container diagnostics (logging saturation, network throughput, CPU, storage I/O) and GPU pod scheduling, per Blind reports (Jan and Aug 2026) and PracHub entries dated July to September 2026. Corporate note: Together AI announced an $800M Series C in July 2026 (company blog; Reuters reported an $8.3B valuation).

### Together AI Coding Problems

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | Detect cycles and break them in pod dependencies | Medium | Graphs / Topological Sort (custom) |
| 2 | Implement an attention primitive with batching, causal masking, numerical stability | Hard | ML Systems (custom) |
| 3 | CUDA kernels: element-wise op, reduction, softmax (memory coalescing, warp divergence) | Hard | GPU Programming (custom) |
| 4 | Batching scheduler matching requests to GPU capacity with preemption | Medium-Hard | Scheduling / Heaps (custom) |
| 5 | Streaming token generation with client-disconnect propagation | Medium | Async Systems (custom) |
| 6 | Two LeetCode Mediums in the final round (graph / DP / priority-queue with ML twists) | Medium | DSA |
| 7 | Infra/SRE diagnostics set: investigate a server saturated by logging; diagnose slow network throughput across containers; diagnose CPU problems on a Linux server; diagnose storage I/O and identify the responsible workload | Easy-Medium | Linux Diagnostics (custom, Sept 2026) |
| 8 | Schedule GPU pods onto nodes and decide whether a node can be drained (capacity check plus pod reassignment) | Medium | Scheduling / Backtracking (custom, July 2026) |
| 9 | Split a chunked text stream arriving through an iterator into n line-balanced parts without breaking lines | Easy | Strings / Streaming (custom, Sept 2026) |
| 10 | SRE screen: read a file and print its contents in your own IDE (you are told to have an IDE ready; the round is about tooling fluency and talking through choices) | Easy | Practical (custom, Aug 2026) |

### Together AI ML/Research Topics

| No. | Topic | Category |
| --- | ----- | -------- |
| 1 | Speculative decoding trade-offs: draft overhead vs acceptance rate | Inference |
| 2 | INT8 vs FP8 quantization: outlier activations, per-channel vs per-tensor scaling | Inference |
| 3 | PagedAttention, continuous batching, KV-cache + FlashAttention | Inference |
| 4 | GPU memory hierarchy (HBM/shared), occupancy, Tensor Cores; tensor parallelism | GPU |
| 5 | Mixtral MoE routing; Llama RMSNorm; RoPE | Architecture |

### Together AI System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Design the inference-serving system supporting 100+ open-source models with shared GPU capacity | Multi-model serving |
| 2 | Design a GPU-aware pod scheduler | Orchestration |
| 3 | Design the fine-tuning service with multi-tenant LoRA adapter management and per-customer isolation | Fine-tuning platform |
| 4 | Design the speculative-decoding pipeline working across diverse model architectures | Inference |

---

## Groq

> **Process**: Recruiter call -> 1-hour phone with live coding (compiler roles) -> technical round(s) with staff engineers -> 1-hour "personality"/leadership interview with a VP. ~32 days average. **NDA before the first interview**: which is why specific questions rarely leak (treat all data as low-confidence). Compiler new-grad candidates report problems "harder than FAANG." Stack: Haskell prototypes, C++/Python tooling; domain centers on the Tensor Streaming Processor (LPU): spatial compiler passes, deterministic scheduling, mapping NN graphs to hardware. LLVM/MLIR experience preferred.
>
> **Corporate note (2026)**: In Dec 2025 Nvidia paid about $20B for a non-exclusive license to Groq's inference technology and hired founder Jonathan Ross, president Sunny Madra and senior hardware staff. Groq continues as an independent company: CFO Simon Edwards briefly served as CEO, Adam Winter was interim CEO as of May 2026, and that month the company raised $650M from existing investors (Disruptive and Infinitum backstopping) to rebuild as an inference neocloud around GroqCloud and a next-generation LPU. The compiler-heavy interview reports above predate the deal, and most of the hardware leadership has moved to Nvidia; check which Groq you are interviewing with.

### Groq Reported Topics

| No. | Topic | Difficulty | Category |
| --- | ----- | ---------- | -------- |
| 1 | Compiler fundamentals: BNF grammars, visitor pattern, ASTs, LLVM concepts | Hard | Compilers |
| 2 | FAANG-style DSA live coding, reportedly harder than FAANG | Hard | DSA |
| 3 | Kernel-optimization and infrastructure-optimization discussions | Hard | Systems / Performance |

---

## Cerebras

> **Process**: OA, **two LeetCode Mediums in 45 minutes** on HackerRank (very time-pressured, short behavioral at the end) -> phone screen -> final round with two more LC Mediums. Alternate reported shape: 4 rounds (2 coding + 2 behavioral), ~1 month. Uses Microsoft Teams + HackerRank. Performance-engineer candidates get parallel programming and matrix multiplication questions on top of coding. Emphasis: Arrays + Strings. 2026 reports keep the same shape: 15-30 min recruiter screen -> 45-60 min exploratory technical with live coding -> four 45-min deep dives (coding, systems knowledge, hiring manager) on Teams + HackerRank. Corporate note: Cerebras listed on Nasdaq as CBRS on May 14, 2026, raising $5.55B at $185 a share, the largest US tech IPO since Snowflake.

### Cerebras Coding Problems

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Flood Fill](https://leetcode.com/problems/flood-fill) | Easy | DFS / BFS |
| 2 | [Word Search](https://leetcode.com/problems/word-search) | Medium | Backtracking |
| 3 | [Continuous Subarray Sum](https://leetcode.com/problems/continuous-subarray-sum) | Medium | Prefix Sum / Hash |
| 4 | [Subsets II](https://leetcode.com/problems/subsets-ii) | Medium | Backtracking |
| 5 | [High Five](https://leetcode.com/problems/high-five) | Easy | Heap / Hash |
| 6 | [Reverse Words in a String](https://leetcode.com/problems/reverse-words-in-a-string) | Medium | Two Pointers |
| 7 | [Analyze User Website Visit Pattern](https://leetcode.com/problems/analyze-user-website-visit-pattern) | Medium | Hash / Sorting |
| 8 | [Maximize Amount After Two Days of Conversions](https://leetcode.com/problems/maximize-amount-after-two-days-of-conversions) | Medium | Graph / DFS |
| 9 | [Remove All Adjacent Duplicates in String II](https://leetcode.com/problems/remove-all-adjacent-duplicates-in-string-ii) | Medium | Stack |
| 10 | [Split Array Largest Sum](https://leetcode.com/problems/split-array-largest-sum) | Hard | Binary Search |
| 11 | [Remove All Occurrences of a Substring](https://leetcode.com/problems/remove-all-occurrences-of-a-substring) | Medium | Stack / String |
| 12 | [All Nodes Distance K in Binary Tree](https://leetcode.com/problems/all-nodes-distance-k-in-binary-tree) | Medium | Tree / BFS |
| 13 | [Zigzag Conversion](https://leetcode.com/problems/zigzag-conversion) | Medium | String |
| 14 | [Adding Spaces to a String](https://leetcode.com/problems/adding-spaces-to-a-string) | Medium | Two Pointers |
| 15 | [Find Score of an Array After Marking All Elements](https://leetcode.com/problems/find-score-of-an-array-after-marking-all-elements) | Medium | Heap / Sorting |
| 16 | [Next Permutation](https://leetcode.com/problems/next-permutation) | Medium | Array |
| 17 | [Find Leaves of Binary Tree](https://leetcode.com/problems/find-leaves-of-binary-tree) | Medium | Tree / DFS |
| 18 | [Make String a Subsequence Using Cyclic Increments](https://leetcode.com/problems/make-string-a-subsequence-using-cyclic-increments) | Medium | Two Pointers |
| 19 | Parallel programming + matrix multiplication (performance roles) | Medium-Hard | HPC (custom) |

---

## ElevenLabs

> **Process**: Recruiter screen -> **async take-home coding screen: CoderPad, 90 minutes, 2-3 problems (2 Medium + 1 Medium-Hard), auto-graded, no interviewer, Python strongly preferred** -> behavioral round testing "founder mindset" (they favor ex-founders) -> practical coding round (60 min, realistic product scenarios with function stubs + sample data) -> **product decomposition round** (45-60 min, signature round: design an end-to-end solution including UI, backend architecture, and database schema). Forward Deployed Engineer roles use a 1-hour CodeSignal assessment instead. 3-5 weeks. **AI policy**: ElevenLabs runs two conversational recruiter agents (AI Becky and AI Oscar) that answer process and benefits questions before a human recruiter call, and its hiring blog tells candidates to prepare with AI, including spinning up an agent on its Conversational AI product to run mock interviews; expect to be asked how you use AI in your own work. FDE loop detail (2026): after the CodeSignal screen, live coding in a shared Google Doc and an Excalidraw case study on a customer scenario. Deployment Strategist loop (Blind, Aug 2026): a customer-scenario working session, then an Excalidraw whiteboarding round to design a hypothetical new product.

### ElevenLabs Coding Problems

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | String manipulation / parsing problems (take-home) | Medium | Strings |
| 2 | Array processing with hash-map + two-pointer patterns (take-home) | Medium | Arrays / Hashing |
| 3 | Tree/graph traversal; data-stream processing (take-home) | Medium-Hard | Trees / Streams |
| 4 | Audio file management / video processing / dubbing pipeline task (practical round) | Medium-Hard | Applied Backend (custom) |
| 5 | Rate-limited API client; streaming audio processing; caching layer (practical round) | Medium-Hard | Systems Coding (custom) |
| 6 | Dubbing workflow tracker: replace a spreadsheet with functions that apply edits to script lines and propagate which lines or files editors and voice actors must re-review after a re-recording (practical round) | Medium-Hard | Applied Backend (custom) |
| 7 | Front-end screen: find and fix a bug in a small React audio-transcription app where the transcript falls out of sync with playback | Medium | Debugging / React (custom, 2026) |
| 8 | FDE live coding: file-system permissions with hierarchy and timestamped permission changes (resolve the effective permission at a given time) | Medium | Trees / Design (custom, 2026) |

### ElevenLabs Product Decomposition Round

Decompose a customer-facing product problem into components; define UI + backend + DB architecture; discuss trade-offs. No code written. Behavioral samples: "Tell me about a project where you were the sole decision-maker", "What's the fastest idea-to-production timeline you've achieved?"

Prompts reported through 2026: redesign an Excel-based dubbing workflow into a product for editors and voice actors (the interviewer steered toward a video-player-centric UI rather than a document with comments); design a tool that lets customers review and correct AI-dubbed video; design storage and versioning for generated audio files; walk through the UI and data model for self-service voice cloning; design an internal tool so support agents can find and re-run dubbing jobs that failed overnight.

---

## Waymo

> **Process**: Recruiter screen -> technical phone screen (45-60 min, one medium-hard or two smaller problems; edge cases + concurrency probing) -> virtual onsite 4-5 rounds: two coding, system design (experienced hires), behavioral; some loops add a domain/"data fluency" round -> hiring committee. ~4-6 weeks. Modern C++ (C++17/20) for onboard/robotics roles. Interviewers test move semantics, memory management, threading primitives; Python for data/ML-eval roles. **Correctness weighted over speed** (safety-critical culture). Behavioral centers on safety mindset. Reports logged June to September 2026 add a senior frontend track (streaming chat UI, debounced autocomplete, tree filter and render), data-heavy SWE prompts (parse corrupted CSV rows, dedupe a 256 GB file in 128 MB of memory) and operational design prompts (vehicle-to-cloud command delivery, mapping-data fleet); SQL rounds appear for data science and BI roles.

### Waymo Coding Problems

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Max Points on a Line](https://leetcode.com/problems/max-points-on-a-line) | Hard | Geometry / Hash |
| 2 | [Random Pick with Weight](https://leetcode.com/problems/random-pick-with-weight) | Medium | Binary Search |
| 3 | [Logger Rate Limiter](https://leetcode.com/problems/logger-rate-limiter) | Easy | Hash / Design |
| 4 | [Number of Visible People in a Queue](https://leetcode.com/problems/number-of-visible-people-in-a-queue) | Hard | Monotonic Stack |
| 5 | [Meeting Rooms II](https://leetcode.com/problems/meeting-rooms-ii) | Medium | Heap / Intervals |
| 6 | [Minimum Number of Refueling Stops](https://leetcode.com/problems/minimum-number-of-refueling-stops) | Hard | Heap / DP |
| 7 | [Minimum Knight Moves](https://leetcode.com/problems/minimum-knight-moves) | Medium | BFS |
| 8 | [Minimum Area Rectangle](https://leetcode.com/problems/minimum-area-rectangle) | Medium | Geometry / Hash |
| 9 | [Design Tic-Tac-Toe](https://leetcode.com/problems/design-tic-tac-toe) | Medium | Design |
| 10 | [Design Excel Sum Formula](https://leetcode.com/problems/design-excel-sum-formula) | Hard | Design / Graph |
| 11 | [Shortest Distance from All Buildings](https://leetcode.com/problems/shortest-distance-from-all-buildings) | Hard | BFS |
| 12 | [Text Justification](https://leetcode.com/problems/text-justification) | Hard | String Simulation |
| 13 | [Path With Minimum Effort](https://leetcode.com/problems/path-with-minimum-effort) | Medium | Binary Search / BFS |
| 14 | [Maximum Earnings From Taxi](https://leetcode.com/problems/maximum-earnings-from-taxi) | Medium | DP |
| 15 | [Robot Room Cleaner](https://leetcode.com/problems/robot-room-cleaner) | Hard | Backtracking |
| 16 | [Number of Islands II](https://leetcode.com/problems/number-of-islands-ii) | Hard | Union-Find |
| 17 | [Car Fleet](https://leetcode.com/problems/car-fleet) | Medium | Sorting / Stack |
| 18 | [Minimum Limit of Balls in a Bag](https://leetcode.com/problems/minimum-limit-of-balls-in-a-bag) | Medium | Binary Search |
| 19 | [Longest Increasing Path in a Matrix](https://leetcode.com/problems/longest-increasing-path-in-a-matrix) | Hard | DFS + Memo |
| 20 | [Basic Calculator](https://leetcode.com/problems/basic-calculator) | Hard | Stack / Parsing |
| 21 | Determine if a shape (e.g., stop sign) is visible within a field of view from sensor data | Hard | Geometry (custom AV) |
| 22 | Will two moving bounding boxes collide within t seconds | Medium-Hard | Geometry / Simulation (custom AV) |
| 23 | [Find Median from Data Stream](https://leetcode.com/problems/find-median-from-data-stream) (framed as sensor smoothing) | Hard | Heaps |
| 24 | Implement a custom memory allocator (C++ roles) | Hard | Low-Level C++ (custom) |
| 25 | [Custom Sort String](https://leetcode.com/problems/custom-sort-string) (sort a string's characters by a given character order) | Medium | Strings / Counting |
| 26 | Parse a raw CSV string into a structure for downstream teams, handling corrupted rows | Medium | Parsing (custom, 2026) |
| 27 | Decide whether a vehicle is ready to go from a log of open and end maintenance events | Medium | Intervals / State (custom, 2026) |
| 28 | Deduplicate a 256 GB file on a machine with 128 MB of memory | Medium | External Sort / Hashing (custom, 2026) |
| 29 | Does a seven-segment LED number read the same when rotated 180 degrees | Medium | Strings / Simulation (custom, 2026) |
| 30 | ObjectTracker that merges observations from two perception systems into one set of tracks | Medium | Design / Matching (custom AV, 2026) |
| 31 | Character at position k in a run-length encoded string without decoding | Medium | Prefix Sums / Binary Search (custom, 2026) |
| 32 | Find the n-th positive integer whose digits are all 3, 5 or 6 | Medium | Math / Base Conversion (custom, 2026) |
| 33 | Frontend track (senior+): filter an N-ary tree by substring and render it with indentation; autocomplete search bar with a hand-written debounce | Medium | Frontend (custom, 2026) |
| 34 | MLE: softmax cross-entropy forward and backward passes plus a training loop | Medium | ML Coding (custom, 2026) |

### Waymo System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Design the IPC architecture to stream 4K camera data to the perception NN with zero-copy memory | On-board real-time (~10ms decision loops) |
| 2 | Design a "Black Box" recording system for anomaly-detected uploads | Off-board / storage |
| 3 | Design a tele-assistance service for stuck vehicles | Real-time operations |
| 4 | Architect validation of motion-planning software against 1M historical miles | Simulation / evaluation |
| 5 | Petabyte-scale vehicle-log ETL pipelines; LiDAR data ingestion/indexing | Data infrastructure |
| 6 | LLD: traffic-signal state machine, in-vehicle pub-sub message broker, sensor scene graph | Low-level design |
| 7 | Design a fleet that collects mapping data (route coverage, upload, map freshness) | Mapping / fleet operations (June 2026) |
| 8 | Design reliable command delivery between autonomous vehicles and the cloud (ordering, acks, retries, intermittent connectivity) | Messaging / reliability (Aug 2026) |
| 9 | Design a simulation system to evaluate a self-driving model on limited compute (scenario selection, prioritization, result caching) | Simulation / evaluation (Sept 2026) |
| 10 | Design a matchmaking service with join, cancel, matching, notification and expiry | Low-level design / state (Sept 2026) |
| 11 | Frontend (senior+): design the frontend of an AI chat application with streaming replies | Frontend architecture (Sept 2026) |

---

## Character.AI

> **Process**: Four rounds. LeetCode-style coding, system design, ML coding, culture fit. 3-4 weeks (~2 with referral). Tone reported as relaxed and collaborative, interviewers give hints. Mix of algorithmic challenges (strings, recursion, data structures), system design for real-time consumer platforms, AI/ML integration, some front-end problems, plus product-sense questions on engaging user experiences.
>
> **Corporate note (2026)**: Character.AI stopped training its own foundation models after the 2024 Google licensing deal and builds on open-weight models (Llama, Qwen, DeepSeek). CEO Karandeep Anand (in the role since June 2025) leaves to become Disney's first CTO effective Oct 2, 2026, and Disney said "a number of Character.AI's technical team" will join him. Factor the leadership transition into any Q4 2026 loop.

### Character.AI Reported Problems & Topics

| No. | Problem / Topic | Difficulty | Category |
| --- | --------------- | ---------- | -------- |
| 1 | String manipulation / recursion / data structure problems | Medium | DSA |
| 2 | Design a transformer that solves the traveling salesman problem | Hard | ML Theory (custom) |
| 3 | Fine-tuning vs RAG for conversational AI, when and why | Medium | LLM Concepts |
| 4 | Design a high-traffic real-time chat system (modularity, data flow, bottlenecks, failure handling) | Hard | System Design |
| 5 | Design a recommendation engine (user/content features, model selection, feedback loops) | Hard | ML System Design |

---

## Sierra AI

> **Process**: Sierra **publicly removed coding/algorithms interviews** ("The AI-native interview," sierra.ai engineering blog). Phone screen is a system-design screen focused on production-readiness. The AI-native onsite has three phases: **Plan** (drive ideation of a product with interviewers) -> **Build** (2 hours solo, any AI tools/frameworks allowed; scope pivots allowed) -> **Review** (demo + defend product decisions, data models, abstractions, and how AI was used). Blog post dated April 22, 2026: https://sierra.ai/blog/the-ai-native-interview. Also piloting a debugging round in which you review a colleague's PR in an existing codebase, pull the code down, inspect the output and improve it with coding agents. Agent SWE loop: CoderPad practical screen -> debugging round (multi-file agent codebase, find ~3 bugs by running tests) -> agent-building take-home (build an agent with a provided API key) + 60-min presentation -> hiring-manager behavioral. Agent Engineer loops reported through September 2026 still open with a 60-minute data-structures screen before the take-home, and the onsite is debugging + agent-project presentation + hiring manager; a September 2026 guide notes conflicting AI rules at the screen (one account: CoderPad with no AI; another: no LLMs but syntax lookup allowed), so confirm the policy in your invitation. Take-home follow-ups: which two features you would prioritize for the client and why, and what metrics and observability you would track in production.

### Sierra AI Reported Problems

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | Flaky-API caller + product-ID resolution, multi-part extensible OOP | Medium | Practical Coding (custom) |
| 2 | Keyboard object with undo/redo, expanding requirements | Medium | OOP Design (custom) |
| 3 | Find and fix ~3 bugs in a multi-file agent codebase | Medium | Debugging (custom) |
| 4 | Build a working AI agent (take-home with provided LLM API key), then extend live | Medium-Hard | Agent Building (custom) |
| 5 | Design an AI customer-service agent for a hypothetical company; extend for new use cases live | Medium-Hard | Agents / Product |
| 6 | Detect circular references in a spreadsheet where cells reference other cells (technical screen) | Medium | Graphs / Cycle Detection (custom, 2026) |
| 7 | Design an agentic service for a given flow, such as subscription cancellation (technical screen) | Medium | Agents / Design (custom, 2026) |
| 8 | Debugging round: find and fix the bugs in a React/TypeScript app and explain how each bug affects the customer | Medium | Debugging / React (custom, 2026) |
| 9 | Split a Markdown document into ordered, header-aware chunks under a size limit | Hard | Parsing / Chunking (custom, Apr 2026) |

---

## Glean

> **Process**: Recruiter screen + LeetCode-style coding round (medium/hard, escalating difficulty) -> onsite: 1 coding round + **signature 2-hour on-the-spot build assignment** (build a functional mini-application that runs) + system design + behavioral. Some candidates report up to 6 rounds. Emphasis on practical engineering speed, "build working software quickly." 2-4 weeks. Entries logged in September 2026 show the loop branching by track: frontend candidates get React build tasks (social feed, Connect Four on a 6x7 board), MLE candidates get an **AI-paired coding exercise** (the rate-limited Wikipedia crawler, with an assistant allowed), and SWE candidates still get LeetCode-style mediums plus the two-hour build.

### Glean Coding Problems

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | Graph DFS connectivity (similar to [Number of Provinces](https://leetcode.com/problems/number-of-provinces)) | Medium | Graphs |
| 2 | Connect 4 with winner detection | Medium | OOP / Simulation (custom) |
| 3 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium | Design |
| 4 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium | Arrays |
| 5 | [Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements) | Medium | Heap / Hash |
| 6 | [Course Schedule](https://leetcode.com/problems/course-schedule) (cycle detection) | Medium | Graphs |
| 7 | [Valid Parentheses](https://leetcode.com/problems/valid-parentheses) with O(1) space follow-up | Easy-Hard | Stack |
| 8 | Event stream processing | Medium | Practical (custom) |
| 9 | [Word Search II](https://leetcode.com/problems/word-search-ii) (search words in a character grid) | Hard | Trie / Backtracking |
| 10 | Top-k prefix suggestions filtered by department within a tight memory budget (follow-up to "return top department suggestions") | Medium | Trie / Heaps (custom, 2026) |
| 11 | Implement a byte-pair encoding tokenizer: threshold-based training, encode and decode | Medium | Strings / ML (custom, 2026) |
| 12 | 2048 board tilts in four directions with merging and game-over detection | Medium | Matrix / Simulation (custom, 2026) |
| 13 | Sort in linear time an array where at most one element was moved out of place | Medium | Arrays (custom, 2026) |
| 14 | Shortest Manhattan distance between any X and any Y in a string or grid | Medium | BFS / Two Pointers (custom, 2026) |
| 15 | [Shortest Distance from All Buildings](https://leetcode.com/problems/shortest-distance-from-all-buildings) (cell with the smallest total walking distance to all targets around walls) | Hard | BFS |
| 16 | [Divide Chocolate](https://leetcode.com/problems/divide-chocolate) (k cuts in a row of positive values, maximize the smallest piece sum) | Hard | Binary Search |
| 17 | Rank every cell of a distinct-value matrix consistently within its row and column (simplified [Rank Transform of a Matrix](https://leetcode.com/problems/rank-transform-of-a-matrix)) | Medium-Hard | Graphs / Topological Sort |
| 18 | Group words into transitive synonym sets by shared two-words-before-and-after context | Medium | Union-Find / Hashing (custom, 2026) |
| 19 | Kth largest element across two sorted arrays | Medium | Binary Search (custom, 2026) |
| 20 | MLE: rate-limited Wikipedia crawler; the Sept 2026 version is paired with an AI assistant and prioritizes unseen title initials | Medium | Async / Rate Limiting (custom, AI-paired, 2026) |
| 21 | Frontend: React social feed with upvote/downvote re-sorting and pinned posts | Medium | Frontend (custom, 2026) |

### Glean System Design

Enterprise search systems: indexing pipelines, ranking algorithms, document retrieval at scale, **permissions-aware search**; improving search relevance while balancing performance and accuracy. Prompts reported in 2026 guides: design search over a company's documents; permission-aware retrieval, comparing replicating ACLs into the index against live permission checks at query time; rolling out a new embedding model over an index holding billions of vectors (backfill cost, fallback); per-tenant versus shared vector indices with metadata filtering; and an API plus database schema for a commenting system.

---

## Runway

> **Process**: Recruiter screen -> 60-min coding screen (Python or TypeScript) -> virtual onsite: 2 coding rounds, ML system design or product system design, craft deep-dive, behavioral. Research candidates add a paper-discussion round. ~4-5 weeks (company aims for screen-to-offer in ~10 days). The coding rounds are medium-hard DSA (arrays, strings, graphs, DP). Craft deep-dive emphasizes ownership, aesthetic judgment, and empathy for filmmakers/advertisers.

### Runway System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Multi-tier video generation pipeline: fast preview + high-fidelity render, GPU capacity planning, job queues | GPU pipelines |
| 2 | Credits/billing system for variable-cost generation jobs: cost estimation, credit reservation, reconciliation | Billing |
| 3 | Creative editor data model: AI-generated clips + classical editing, undo/redo, non-destructive edits | Data modeling |

---

## Snowflake (AI/Data)

> **Process**: Recruiter/HM screen -> 60-min technical screen (widely called the hardest stage) -> final panel of 3-5 interviews (technical, domain expertise, system design, behavioral). 2-4 weeks. Coding questions look standard but carry data-processing twists; big-data handling is always in scope. Backend/platform roles: distributed systems, indexing, storage trade-offs, concurrency, fault tolerance. AI/ML (Cortex) roles add LLM-platform content: Cortex functions, Cortex Search, Snowpark, feature stores.

### Snowflake Coding Problems

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Insert Interval](https://leetcode.com/problems/insert-interval) | Medium | Arrays |
| 2 | Class that processes a stream of input | Medium | Design / Streaming (custom) |
| 3 | Browser-tab behavior simulator (similar to [Design Browser History](https://leetcode.com/problems/design-browser-history)) | Medium | Design / Simulation |
| 4 | Duplicated character check in string | Easy | Strings |

### Snowflake System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Design a quota service / resource scheduling system | Data platform |
| 2 | Design a data security and governance system | Governance |
| 3 | Governed RAG service with Cortex Search (ingestion, RBAC enforcement, citation tracking, eval gates) | AI platform |
| 4 | Pipeline enriching raw data via Cortex LLM functions (incremental processing, cost control, output validation) | AI platform |
| 5 | Real-time feature serving for recommendations (feature-store materialization, caching, cold start) | ML platform |

---

## 2026 AI Interview Trends

Cross-company shifts documented across 2025-2026 (Karat, interviewing.io, Fabric, CodeSignal, company engineering blogs):

1. **AI-assisted interview rounds went mainstream at big tech.** Meta piloted an AI-enabled coding round in Oct 2025 (60-min CoderPad with GPT-5/Claude/Gemini/Llama built in) and rolled it across back-end and ops roles in 2026 (E6 and below: one traditional plus one AI round; E7+: AI round only); Google announced in May 2026 a pilot of an AI-assisted "code comprehension" round (read, debug and optimize an existing codebase with Gemini, graded on prompt quality, output validation and debugging) for junior to mid-level roles on select US teams in the second half of 2026; LinkedIn replaced one coding round with an AI-enabled round; some Microsoft teams allow GitHub Copilot. Evaluation shifts to judgment, verification of AI output, and communication. Not prompt tricks.
2. **AI cheating exploded and reshaped formats.** CodeSignal's Feb 2026 report puts cheating/fraud attempts on proctored assessments at 35% in 2025, up from 16% in 2024, with entry-level assessments at 40% (from 15%). Fabric's Jan 2026 analysis of 19,368 AI interviews (July 2025 to Jan 2026) flagged 38.5% of all candidates, 48% in technical roles against 12% in sales, with rates tripling between July and Sept 2025; junior candidates (0-5 years) cheated at about twice the senior rate. Invisible overlay tools (Interview Coder, Leetcode Wizard, Cluely, Final Round AI) are undetectable via screen share and account for 45% of detected cases; voice-mode LLMs account for another 34%.
3. **In-person interviews returned.** Google reinstated at least one in-person round for technical hires in 2026; multiple major employers quietly re-added mandatory onsite finals in Q1 2026.
4. **Take-homes grew a live-defense round.** 71% of engineering leaders say AI made technical assessment harder (Karat); companies now attach a "walk me through your code and your decisions" session, or replace multi-hour take-homes with 60-90-min live pairing.
5. **Work trials are the AI-startup norm.** Cursor: paid multi-day onsite projects on a real codebase; OpenAI: paid (~$1,000) 48-hour take-home work trials; Cognition/Kilo/Crosby: multi-day trials and bootcamps; Sierra: Plan -> Build (2h with AI) -> Review onsites.
6. **"AI fluency" is an explicit signal.** Companies open interviews with questions like "How many tokens are you consuming every week?"; several have candidates build with AI in-session.
7. **Interviewers retooled questions.** In an interviewing.io survey of 67 FAANG/startup interviewers, 58% changed the algorithmic questions they ask; debug-focused rounds (find bugs in supplied code) and real-time "why this data structure?" probes are the common anti-AI patterns.
8. **Anthropic redesigned its performance take-home three times** because Claude kept beating it. The current version is a Zachtronics-style constrained-instruction-set puzzle where building your own tooling is part of the test, and AI tools are explicitly permitted. Timeline (The Decoder, Jan 2026): Claude 3.7 Sonnet out-scored more than half of candidates, Claude Opus 4 forced the cut from 4 to 2 hours in May 2025, and Claude Opus 4.5 matched the best humans in 2 hours. Anthropic published the retired original at https://github.com/anthropics/original_performance_takehome; the README says a solution under 1,487 cycles (Opus 4.5's 11.5-hour result) qualifies for recruiting consideration via performance-recruiting@anthropic.com.
9. **Structural shifts:** system design now appears for mid-level (not just senior) roles; behavioral rounds are more structured and evidence-based; big tech keeps standardized AI-off algorithm loops while AI-native startups converge on practical AI-allowed building. Candidates must prep for both formats.
10. **Corporate churn moved the goalposts in 2026.** xAI became SpaceXAI (Feb 2026 acquisition, July 2026 rename); Amazon closed its San Francisco AGI Lab site (July 2026); Groq licensed its technology to Nvidia and lost its founder (Dec 2025); Scale AI installed a new CEO (Aug 2026); Character.AI's CEO left for Disney (Oct 2026); Thinking Machines Lab lost four of six co-founders; Cohere agreed to merge with Aleph Alpha (Apr 2026). Before a company-specific prep plan, confirm which org and manager the role now reports to; several of the process notes above describe loops that predate these changes.

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

**Preparing for a loop right now?** Book a mock interview or a 1:1 mentorship session with the maintainer: [Engine Bogie](https://enginebogie.com/u/om) for mock interviews, [Topmate](https://topmate.io/ombharatiya) for mentorship and consultancy.

</div>
