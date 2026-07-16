# AI Labs & AI Companies. Interview Questions (2025-2026)

> Interview processes, coding questions, ML questions, and system design prompts at the top AI labs and AI-first companies, compiled from 1,500+ candidate reports, engineering blogs, and interview guides (Reddit, Blind, Glassdoor, 1point3acres, LeetCode Discuss, interviewing.io, Exponent, and company sources). For OpenAI and Anthropic deep-dives, see [FAANG-Recent-Questions.md](./FAANG-Recent-Questions.md#openai).

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

> **Process**: Recruiter screen -> hiring manager screen -> **technical quiz round** (~2 hours: four ~30-min sections on CS fundamentals, mathematics, statistics, and ML, rapid-fire and definition-heavy; veterans fail on forgotten formal definitions like eigenvalues, rank, SVD) -> 2 coding rounds on CoderPad (code is expected to *run*, unlike core Google) -> ML/system design -> paper discussion round (present and defend a paper, sometimes given 2-3 days prior) -> behavioral -> hiring committee. 6-10 weeks total. AI tools prohibited in technical rounds (2026 policy).

### Coding Problems

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

### System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Design a training system for a model that does not fit on a single accelerator | Pipeline/tensor parallelism, ZeRO/DeepSpeed |
| 2 | Design evaluation infrastructure | Benchmark contamination, reproducibility |
| 3 | Solve the straggler problem in synchronous training across thousands of GPUs | Distributed training |
| 4 | Design distributed telemetry ingestion from millions of training jobs | Streaming / scale |

---

## xAI

> **Process**: Engineer screen (often no recruiter; "explain your most technical project in 30 seconds") -> **proctored CodeSignal OA** (~60-70 min, camera + mic + screen recording; one problem with five escalating complexity levels) -> 2-3 live coding rounds (practical/production-flavored: class design, iterators, KV stores, caches; one 45-min format = 20 min working solution + 15 min extending to concurrency at "millions of queries") -> system design -> brief behavioral. Fast (2-3 weeks) but scheduling reported as chaotic. Candidates report failing on coding bar, not ML. Python and TypeScript most common.

### Coding Problems

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

### ML Questions

| No. | Topic | Category |
| --- | ----- | -------- |
| 1 | Why Transformers beat RNNs for LLMs; core Transformer components | Architecture |
| 2 | Data parallelism vs model parallelism for 100B+ models; tensor vs pipeline parallelism, pipeline-bubble management | Distributed Training |
| 3 | Memory-efficient training of billion-parameter models; CUDA kernel acceleration | Systems |
| 4 | Efficient attention for 100K-token contexts | Architecture |

### System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Design a distributed rate limiter for an API gateway at 100k req/s across multiple instances | Per-user/per-IP limits, cross-node consistency |
| 2 | Real-time inference serving at 100,000 req/s | GPU serving, batching |
| 3 | Data pipeline for massive text-dataset ingestion/training | Data infrastructure |
| 4 | Real-time logging system for model inference | Observability |

---

## Mistral AI

> **Process**: Recruiter screen -> technical screen (60 min, one medium-hard problem in Python/Rust; C++/CUDA for some roles) -> take-home for select/research roles (4-8h; design a small LLM/agent experiment, write-up judged with academic-paper expectations) -> **LLM knowledge quiz** (45-75 min structured deep-dive) -> system design (AI-infrastructure flavored) -> behavioral/values. Research roles add a research presentation with 20+ min of hard questioning. Ground "why Mistral" in the open-weight mission; read the Mistral 7B/Mixtral/Codestral papers.

### Coding Problems

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

### ML Questions

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

### System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Design the inference-serving system for a 70B MoE model at 10K req/sec with p95 < 1 sec | GPU serving |
| 2 | Design the training pipeline for a 70B dense model across 2K H100 GPUs | Distributed training |
| 3 | Design La Plateforme's multi-tenant API with fair rate-limiting, per-customer quotas, cost tracking | API platform |
| 4 | Design an enterprise on-premise deployment with model updates, A/B testing, data-sovereignty guarantees | Enterprise |
| 5 | Deploy across 3 EU regions with data residency; handle a 10x traffic spike | Operations |

---

## Meta Superintelligence Labs

> **Process**: MSL research hiring is a distinct track, initial ~50-person team recruited by mining most-cited paper authors, with Zuckerberg personally interviewing; candidates tested on ability to identify and quantify gaps in current AI models. Engineering roles follow the standard Meta loop **plus the AI-enabled coding round** (piloted Oct 2025, default for backend roles in 2026, levels E5-E7/M2): 60 min in a 3-panel CoderPad (file explorer, editor, AI chat, GPT-5, Claude Sonnet, Gemini, Llama 4 available; AI reads files but cannot edit). Three phases: (1) find/fix a non-algorithmic bug, (2) build a 120+ line feature with AI expected, (3) optimize for larger datasets. Rubric: Problem Solving, Code Quality, **Verification** (test before trusting AI output), Communication. Candidates report the in-interview AI is "nerfed" vs practice environments.

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

> **Process**: The AGI SF Lab phone screen covers coding + system design + backend tasks + Leadership Principles. Onsite for ML roles: coding, ML application/design, behavioral with heavy LP emphasis, bar raiser in the loop. The Nova team follows the standard Amazon AGI / Applied Scientist process. ML coding style compared by candidates to OpenAI's.

### Reported Problems

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | Debug a broken Transformer implementation | Hard | ML Coding |
| 2 | Build/train a small classifier live | Medium | ML Coding |
| 3 | Reinforcement learning fundamentals + coding | Medium-Hard | ML |
| 4 | Standard LC coding + backend task in phone screen | Medium | DSA / Practical |

See [Amazon in FAANG-Recent-Questions.md](./FAANG-Recent-Questions.md#amazon) for the standard question bank.

---

## Safe Superintelligence & Thinking Machines Lab

> **Safe Superintelligence (SSI)**: No public interview-question data exists, consistent with extreme secrecy. Credibly reported: in-person candidates must place phones in a Faraday cage before entering SSI offices; ~20-50 employees split between Palo Alto and Tel Aviv; hiring is network-driven; staff discouraged from listing SSI on LinkedIn. No OA platform, loop structure, or question bank has leaked.
>
> **Thinking Machines Lab**: Young lab (founded Feb 2025), hires heavily through networks around the **Tinker** fine-tuning platform (Research Engineer/SWE, $350K-$500K per postings). Reported loop (thin, single-source): recruiter screen -> hiring manager -> research/coding interview -> cross-functional panel. No verified question bank yet. Note: Glassdoor's "Thinking Machines" entry is a Manila data-science consultancy, different company.

---

## Perplexity AI

> **Process**: Recruiter screen (45 min) -> technical phone screen (~45 min coding) -> virtual onsite 4-5 rounds (coding, system design, infrastructure, hiring-manager deep dive) -> final round with a **founder/senior leader**. Very fast: ~11-23 days end-to-end; resume-to-first-interview within three business days. OA on HackerRank/CodeSignal (75-90 min, 2-3 questions). Python strongly preferred (codebase is Python-first). Evaluated on production-ready code, edge cases, velocity, RAG/search-domain reasoning.

### Coding Problems

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

### ML/AI Questions

| No. | Topic | Category |
| --- | ----- | -------- |
| 1 | RAG end-to-end: retrieval -> context assembly -> generation with citations; chunking, dense vs sparse (BM25) vs hybrid retrieval, re-ranking | RAG |
| 2 | Hallucination mitigation and context-window management | LLM |
| 3 | SFT vs RLHF vs DPO, when would you choose one over another | Alignment |
| 4 | "How do you know Model A beats Model B for search?", calibration, factuality, A/B design | Evaluation |
| 5 | Cost/latency optimization of LLM serving (token budgets, caching, concurrency) | Inference |

### System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | "Design a system that knows about something that happened 30 minutes ago" | Real-time crawling, event detection, cache invalidation |
| 2 | Design a recommender system for Perplexity's Discover page | Recommendations |
| 3 | Design a personal finance platform syncing spend data from multiple credit-card accounts | Integrations |
| 4 | Kubernetes infrastructure debugging: system overloaded, debug via metrics | Infrastructure |

---

## Scale AI

> **Process**: Recruiter screen -> HackerRank OA / technical screen (~60 min, 2 mediums) -> hiring-manager screen -> virtual onsite 4-5 rounds: coding, **backend practical**, **debugging round** (unfamiliar multi-file codebase, find/fix 2-3 logical bugs in 60 min), system design or ML, and "Credo" behavioral. Explicitly "not standard LeetCode", implementation-heavy, production realism, speed and working code over algorithmic cleverness.

### Coding Problems

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

### ML/AI Questions

| No. | Topic | Category |
| --- | ----- | -------- |
| 1 | Transformers, attention, decoding strategies, RLHF, evaluation, optimization | LLM Fundamentals |
| 2 | LLM post-training methods and trade-offs (SFT/RLHF/DPO pipeline for a base model) | Post-Training |
| 3 | Adversarial attacks; evaluation and deployment failure modes; pipeline debugging | Robustness |
| 4 | Human-in-the-loop labeling quality: automated + human evaluation frameworks | Data Quality |

### System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Design a streaming job scheduler (continuous task ingestion + dispatch) | Scheduling |
| 2 | Design an LLM API pipeline (hosted LLM APIs resolving user tasks) | LLM Integration |
| 3 | Design a data-annotation/labeling pipeline; LLM evaluation system | Core Domain |
| 4 | Design a large-scale ticketing system (high concurrency) | Distributed Systems |

---

## Cohere

> **Process**: Recruiter screen -> technical screen (60 min live coding, **Python or Go**) -> ML round or system design (team-dependent) -> behavioral -> team match. ~4-6 weeks. Style: production-quality infrastructure code over LeetCode tricks, "no segment trees, advanced DP, or competitive programming." Tests-first, edge cases, explicit concurrency/locking. MLE track adds a ~3-hour assessment spanning language modelling, math for ML, and coding, plus numpy ML coding and a research presentation.

### Coding Problems

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | Token rate limiter: N tokens/sec per customer, sliding-window semantics, thread-safe | Medium | Concurrency / Design (custom) |
| 2 | Request batch aggregator: batch inference requests up to size 32 or 50 ms wait | Medium | Concurrency / Systems (custom) |
| 3 | [LRU Cache](https://leetcode.com/problems/lru-cache) with TTL expiry | Medium | Design |
| 4 | Streaming response parser handling partial chunks | Medium | Strings / Systems (custom) |
| 5 | Retry-with-backoff; token bucket implementations | Easy-Medium | Systems Utilities (custom) |
| 6 | Create a dataset for sentence completion using BERT | Medium | ML Coding (custom) |
| 7 | ML coding with numpy (implement model components) | Medium-Hard | ML Coding (custom) |

### ML/AI Questions

| No. | Topic | Category |
| --- | ----- | -------- |
| 1 | RAG pipeline failure modes; chunking strategies; when BM25 beats dense embeddings | RAG |
| 2 | Embedding evaluation: NDCG, MRR, recall@k; multilingual retrieval; when to fine-tune embeddings | Evaluation |
| 3 | LoRA vs full fine-tune; mitigating catastrophic forgetting | Fine-Tuning |
| 4 | "Build an eval suite for our Rerank model on a new vertical" | Evaluation |
| 5 | "Fine-tune Command for a regulated industry where hallucinations cost the customer money" | Applied |
| 6 | Attention mathematics, write the equation; encoder-only vs decoder-only vs encoder-decoder | Architecture |

### System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Multi-tenant inference platform on a shared GPU fleet: Customer A needs 50ms p95, Customer B runs overnight batch embeddings, Customer C does RAG with strict data isolation | GPU economics, latency budgets, isolation, cost-per-query |
| 2 | Inference servers, fine-tuning pipelines, eval harnesses, customer-facing APIs | Platform |

---

## Hugging Face

> **Process**: Application review (cover letter explicitly weighted, passion for open source) -> recruiter screen -> 1-2 conversational technical interviews (~60 min) -> **take-home project** for junior/intern roles (build a HF Spaces demo, dataset card project, or fix a bug in their OSS tooling) with follow-up presentation; senior roles get architecture discussions or a "job talk." Open-source track record (PRs to HF repos) counts heavily. De-emphasizes rote algorithm memorization. Note: interview data volume is low. Treat specifics as low-sample.

### Coding Problems

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Merge Two Sorted Lists](https://leetcode.com/problems/merge-two-sorted-lists) | Easy | Linked List |
| 2 | [Missing Number](https://leetcode.com/problems/missing-number) | Easy | Math / Bit |
| 3 | SQL: select 2nd highest salary in the engineering department | Easy-Medium | SQL |
| 4 | Take-home: build a Hugging Face Spaces demo / dataset card project | Medium | Applied ML Project (custom) |
| 5 | Fine-tune a BERT model end-to-end; build an inference pipeline | Medium | Applied ML (custom) |

### ML/AI Questions

| No. | Topic | Category |
| --- | ----- | -------- |
| 1 | "What innovative approaches do you envision for enhancing transformer efficiency and performance?" | Architecture |
| 2 | Fine-tuning workflows with the HF Trainer API; dataset preprocessing, training loops, evaluation metrics | Applied ML |
| 3 | Your open-source contributions and how you'd contribute to specific HF projects | Open Source |

---

## Cursor (Anysphere)

> **Process**: Recruiter/manager screen (covers "why Cursor" and tolerance for heavy workload) -> 1-3 technical phone screens (60 min, one medium-hard problem, sometimes against part of Cursor's actual codebase) -> **paid onsite project: 8-9 hours** (one or two 8-hour days for senior roles; real codebase access, a Slack channel, build a feature autonomously, ending with a presentation, this round decides the offer) -> culture-fit discussion (often over meals). Some senior/staff roles get a 4-8h take-home. AI tools: reports conflict. Some say unrestricted AI in all rounds, others say prohibited in the first coding round; all agree pasting raw model output without judgment is a fast rejection. Languages: TypeScript (editor), Rust (perf-critical), Python (ML).

### Coding Problems

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

### System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Design Cursor's tab-prediction system with sub-100ms latency end-to-end for millions of users | Latency / ML serving |
| 2 | Design Cursor's agent mode executing multi-file edits with verification and rollback | Agents |
| 3 | Design the privacy-preserving inference architecture keeping enterprise code confidential | Privacy |
| 4 | Design the custom-model training pipeline producing coding-specialized variants | Training |

---

## Together AI

> **Process**: Recruiter screen -> technical phone screen (60 min, one medium-hard problem in Python/C++/CUDA) -> take-home for senior/research roles (4-8h; CUDA kernel implementation for inference roles) -> onsite 4-5 rounds: two coding (algorithms + applied ML-systems), system design, one or two ML/research rounds, behavioral -> VP round. ~3 weeks. Real CUDA fluency expected for inference-engine roles (difficulty compared to NVIDIA core GPU teams).

### Coding Problems

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | Detect cycles and break them in pod dependencies | Medium | Graphs / Topological Sort (custom) |
| 2 | Implement an attention primitive with batching, causal masking, numerical stability | Hard | ML Systems (custom) |
| 3 | CUDA kernels: element-wise op, reduction, softmax (memory coalescing, warp divergence) | Hard | GPU Programming (custom) |
| 4 | Batching scheduler matching requests to GPU capacity with preemption | Medium-Hard | Scheduling / Heaps (custom) |
| 5 | Streaming token generation with client-disconnect propagation | Medium | Async Systems (custom) |
| 6 | Two LeetCode Mediums in the final round (graph / DP / priority-queue with ML twists) | Medium | DSA |

### ML/Research Topics

| No. | Topic | Category |
| --- | ----- | -------- |
| 1 | Speculative decoding trade-offs: draft overhead vs acceptance rate | Inference |
| 2 | INT8 vs FP8 quantization: outlier activations, per-channel vs per-tensor scaling | Inference |
| 3 | PagedAttention, continuous batching, KV-cache + FlashAttention | Inference |
| 4 | GPU memory hierarchy (HBM/shared), occupancy, Tensor Cores; tensor parallelism | GPU |
| 5 | Mixtral MoE routing; Llama RMSNorm; RoPE | Architecture |

### System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Design the inference-serving system supporting 100+ open-source models with shared GPU capacity | Multi-model serving |
| 2 | Design a GPU-aware pod scheduler | Orchestration |
| 3 | Design the fine-tuning service with multi-tenant LoRA adapter management and per-customer isolation | Fine-tuning platform |
| 4 | Design the speculative-decoding pipeline working across diverse model architectures | Inference |

---

## Groq

> **Process**: Recruiter call -> 1-hour phone with live coding (compiler roles) -> technical round(s) with staff engineers -> 1-hour "personality"/leadership interview with a VP. ~32 days average. **NDA before the first interview**: which is why specific questions rarely leak (treat all data as low-confidence). Compiler new-grad candidates report problems "harder than FAANG." Stack: Haskell prototypes, C++/Python tooling; domain centers on the Tensor Streaming Processor (LPU): spatial compiler passes, deterministic scheduling, mapping NN graphs to hardware. LLVM/MLIR experience preferred.

### Reported Topics

| No. | Topic | Difficulty | Category |
| --- | ----- | ---------- | -------- |
| 1 | Compiler fundamentals: BNF grammars, visitor pattern, ASTs, LLVM concepts | Hard | Compilers |
| 2 | FAANG-style DSA live coding, reportedly harder than FAANG | Hard | DSA |
| 3 | Kernel-optimization and infrastructure-optimization discussions | Hard | Systems / Performance |

---

## Cerebras

> **Process**: OA, **two LeetCode Mediums in 45 minutes** on HackerRank (very time-pressured, short behavioral at the end) -> phone screen -> final round with two more LC Mediums. Alternate reported shape: 4 rounds (2 coding + 2 behavioral), ~1 month. Uses Microsoft Teams + HackerRank. Performance-engineer candidates get parallel programming and matrix multiplication questions on top of coding. Emphasis: Arrays + Strings.

### Coding Problems

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

> **Process**: Recruiter screen -> **async take-home coding screen: CoderPad, 90 minutes, 2-3 problems (2 Medium + 1 Medium-Hard), auto-graded, no interviewer, Python strongly preferred** -> behavioral round testing "founder mindset" (they favor ex-founders) -> practical coding round (60 min, realistic product scenarios with function stubs + sample data) -> **product decomposition round** (45-60 min, signature round: design an end-to-end solution including UI, backend architecture, and database schema). Forward Deployed Engineer roles use a 1-hour CodeSignal assessment instead. 3-5 weeks.

### Coding Problems

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | String manipulation / parsing problems (take-home) | Medium | Strings |
| 2 | Array processing with hash-map + two-pointer patterns (take-home) | Medium | Arrays / Hashing |
| 3 | Tree/graph traversal; data-stream processing (take-home) | Medium-Hard | Trees / Streams |
| 4 | Audio file management / video processing / dubbing pipeline task (practical round) | Medium-Hard | Applied Backend (custom) |
| 5 | Rate-limited API client; streaming audio processing; caching layer (practical round) | Medium-Hard | Systems Coding (custom) |

### Product Decomposition Round

Decompose a customer-facing product problem into components; define UI + backend + DB architecture; discuss trade-offs. No code written. Behavioral samples: "Tell me about a project where you were the sole decision-maker", "What's the fastest idea-to-production timeline you've achieved?"

---

## Waymo

> **Process**: Recruiter screen -> technical phone screen (45-60 min, one medium-hard or two smaller problems; edge cases + concurrency probing) -> virtual onsite 4-5 rounds: two coding, system design (experienced hires), behavioral; some loops add a domain/"data fluency" round -> hiring committee. ~4-6 weeks. Modern C++ (C++17/20) for onboard/robotics roles. Interviewers test move semantics, memory management, threading primitives; Python for data/ML-eval roles. **Correctness weighted over speed** (safety-critical culture). Behavioral centers on safety mindset.

### Coding Problems

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

### System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Design the IPC architecture to stream 4K camera data to the perception NN with zero-copy memory | On-board real-time (~10ms decision loops) |
| 2 | Design a "Black Box" recording system for anomaly-detected uploads | Off-board / storage |
| 3 | Design a tele-assistance service for stuck vehicles | Real-time operations |
| 4 | Architect validation of motion-planning software against 1M historical miles | Simulation / evaluation |
| 5 | Petabyte-scale vehicle-log ETL pipelines; LiDAR data ingestion/indexing | Data infrastructure |
| 6 | LLD: traffic-signal state machine, in-vehicle pub-sub message broker, sensor scene graph | Low-level design |

---

## Character.AI

> **Process**: Four rounds. LeetCode-style coding, system design, ML coding, culture fit. 3-4 weeks (~2 with referral). Tone reported as relaxed and collaborative, interviewers give hints. Mix of algorithmic challenges (strings, recursion, data structures), system design for real-time consumer platforms, AI/ML integration, some front-end problems, plus product-sense questions on engaging user experiences.

### Reported Problems & Topics

| No. | Problem / Topic | Difficulty | Category |
| --- | --------------- | ---------- | -------- |
| 1 | String manipulation / recursion / data structure problems | Medium | DSA |
| 2 | Design a transformer that solves the traveling salesman problem | Hard | ML Theory (custom) |
| 3 | Fine-tuning vs RAG for conversational AI, when and why | Medium | LLM Concepts |
| 4 | Design a high-traffic real-time chat system (modularity, data flow, bottlenecks, failure handling) | Hard | System Design |
| 5 | Design a recommendation engine (user/content features, model selection, feedback loops) | Hard | ML System Design |

---

## Sierra AI

> **Process**: Sierra **publicly removed coding/algorithms interviews** ("The AI-native interview," sierra.ai engineering blog). Phone screen is a system-design screen focused on production-readiness. The AI-native onsite has three phases: **Plan** (drive ideation of a product with interviewers) -> **Build** (2 hours solo, any AI tools/frameworks allowed; scope pivots allowed) -> **Review** (demo + defend product decisions, data models, abstractions, and how AI was used). Also piloting a debugging round using coding agents on an existing codebase. Agent SWE loop: CoderPad practical screen -> debugging round (multi-file agent codebase, find ~3 bugs by running tests) -> agent-building take-home (build an agent with a provided API key) + 60-min presentation -> hiring-manager behavioral.

### Reported Problems

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | Flaky-API caller + product-ID resolution, multi-part extensible OOP | Medium | Practical Coding (custom) |
| 2 | Keyboard object with undo/redo, expanding requirements | Medium | OOP Design (custom) |
| 3 | Find and fix ~3 bugs in a multi-file agent codebase | Medium | Debugging (custom) |
| 4 | Build a working AI agent (take-home with provided LLM API key), then extend live | Medium-Hard | Agent Building (custom) |
| 5 | Design an AI customer-service agent for a hypothetical company; extend for new use cases live | Medium-Hard | Agents / Product |

---

## Glean

> **Process**: Recruiter screen + LeetCode-style coding round (medium/hard, escalating difficulty) -> onsite: 1 coding round + **signature 2-hour on-the-spot build assignment** (build a functional mini-application that runs) + system design + behavioral. Some candidates report up to 6 rounds. Emphasis on practical engineering speed, "build working software quickly." 2-4 weeks.

### Coding Problems

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

### System Design

Enterprise search systems: indexing pipelines, ranking algorithms, document retrieval at scale, **permissions-aware search**; improving search relevance while balancing performance and accuracy.

---

## Runway

> **Process**: Recruiter screen -> 60-min coding screen (Python or TypeScript) -> virtual onsite: 2 coding rounds, ML system design or product system design, craft deep-dive, behavioral. Research candidates add a paper-discussion round. ~4-5 weeks (company aims for screen-to-offer in ~10 days). The coding rounds are medium-hard DSA (arrays, strings, graphs, DP). Craft deep-dive emphasizes ownership, aesthetic judgment, and empathy for filmmakers/advertisers.

### System Design

| No. | Question | Key Focus |
| --- | -------- | --------- |
| 1 | Multi-tier video generation pipeline: fast preview + high-fidelity render, GPU capacity planning, job queues | GPU pipelines |
| 2 | Credits/billing system for variable-cost generation jobs: cost estimation, credit reservation, reconciliation | Billing |
| 3 | Creative editor data model: AI-generated clips + classical editing, undo/redo, non-destructive edits | Data modeling |

---

## Snowflake (AI/Data)

> **Process**: Recruiter/HM screen -> 60-min technical screen (widely called the hardest stage) -> final panel of 3-5 interviews (technical, domain expertise, system design, behavioral). 2-4 weeks. Coding questions look standard but carry data-processing twists; big-data handling is always in scope. Backend/platform roles: distributed systems, indexing, storage trade-offs, concurrency, fault tolerance. AI/ML (Cortex) roles add LLM-platform content: Cortex functions, Cortex Search, Snowpark, feature stores.

### Coding Problems

| No. | Problem | Difficulty | Category |
| --- | ------- | ---------- | -------- |
| 1 | [Insert Interval](https://leetcode.com/problems/insert-interval) | Medium | Arrays |
| 2 | Class that processes a stream of input | Medium | Design / Streaming (custom) |
| 3 | Browser-tab behavior simulator (similar to [Design Browser History](https://leetcode.com/problems/design-browser-history)) | Medium | Design / Simulation |
| 4 | Duplicated character check in string | Easy | Strings |

### System Design

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

1. **AI-assisted interview rounds went mainstream at big tech.** Meta piloted an AI-enabled coding round in Oct 2025 (60-min CoderPad with GPT-5/Claude/Gemini/Llama built in) rolling out across roles in 2026; Google is piloting an AI-assisted "code comprehension" round with Gemini; LinkedIn replaced one coding round with an AI-enabled round; some Microsoft teams allow GitHub Copilot. Evaluation shifts to judgment, verification of AI output, and communication. Not prompt tricks.
2. **AI cheating exploded and reshaped formats.** CodeSignal reports cheating/fraud attempts rose from 16% to 35% of assessments (2024->2025); Fabric reports 48% of technical candidates triggered cheating markers. Invisible overlay tools (Interview Coder, Leetcode Wizard, Cluely) are undetectable via screen share.
3. **In-person interviews returned.** Google reinstated at least one in-person round for technical hires in 2026; multiple major employers quietly re-added mandatory onsite finals in Q1 2026.
4. **Take-homes grew a live-defense round.** 71% of engineering leaders say AI made technical assessment harder (Karat); companies now attach a "walk me through your code and your decisions" session, or replace multi-hour take-homes with 60-90-min live pairing.
5. **Work trials are the AI-startup norm.** Cursor: paid multi-day onsite projects on a real codebase; OpenAI: paid (~$1,000) 48-hour take-home work trials; Cognition/Kilo/Crosby: multi-day trials and bootcamps; Sierra: Plan -> Build (2h with AI) -> Review onsites.
6. **"AI fluency" is an explicit signal.** Companies open interviews with questions like "How many tokens are you consuming every week?"; several have candidates build with AI in-session.
7. **Interviewers retooled questions.** In an interviewing.io survey of 67 FAANG/startup interviewers, 58% changed the algorithmic questions they ask; debug-focused rounds (find bugs in supplied code) and real-time "why this data structure?" probes are the common anti-AI patterns.
8. **Anthropic redesigned its performance take-home three times** because Claude kept beating it. The current version is a Zachtronics-style constrained-instruction-set puzzle where building your own tooling is part of the test, and AI tools are explicitly permitted.
9. **Structural shifts:** system design now appears for mid-level (not just senior) roles; behavioral rounds are more structured and evidence-based; big tech keeps standardized AI-off algorithm loops while AI-native startups converge on practical AI-allowed building. Candidates must prep for both formats.

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
