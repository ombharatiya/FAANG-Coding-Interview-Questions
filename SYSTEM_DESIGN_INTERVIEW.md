# 🚀 FAANG System Design Interview Guide 🚀

## 25 Must-Do System Design Problems for Tech Interviews

<div align="center">
  <a href="https://github.com/ombharatiya/FAANG-Coding-Interview-Questions">
    <img src="https://img.shields.io/badge/🏗️%20System%20Design%20Guide-000000?style=for-the-badge" alt="System Design Guide" />
  </a>
  
  <p><em>A curated collection of system design problems frequently asked in interviews at top tech companies</em></p>
  
  <p>
    <a href="https://github.com/ombharatiya/FAANG-Coding-Interview-Questions/stargazers">
      <img src="https://img.shields.io/badge/⭐%20STAR%20THIS%20REPO-yellow?style=for-the-badge" alt="Star This Repo" />
    </a>
    <a href="https://github.com/ombharatiya?tab=followers">
      <img src="https://img.shields.io/badge/👨‍💻%20FOLLOW%20@OMBHARATIYA-39D353?style=for-the-badge" alt="Follow @ombharatiya" />
    </a>
  </p>
</div>

## Table of System Design Interview Problems

This table presents 25 essential system design problems that are frequently asked in technical interviews at top technology companies. Each problem is categorized by complexity level (Low, Medium, High) and includes information about which companies commonly ask these questions and for which engineering roles.

| # | Problem | Complexity | Companies | Roles | Resources |
|---|---------|------------|-----------|-------|-----------|
| 1 | Design a URL Shortening Service (like Bit.ly) | Medium | Google, Amazon, Microsoft, Uber | SWE, SDE, Backend | [System Design Primer](https://github.com/donnemartin/system-design-primer/blob/master/solutions/system_design/pastebin/README.md), [Grokking](https://www.educative.io/courses/grokking-modern-system-design-interview-for-engineers-managers/tiny-url-design-tinyurl) |
| 2 | Design Twitter | High | Twitter, Meta, Google, Microsoft | SWE, SDE, Full-stack | [System Design Primer](https://github.com/donnemartin/system-design-primer/blob/master/solutions/system_design/twitter/README.md), [High Scalability](http://highscalability.com/blog/2013/7/8/the-architecture-twitter-uses-to-deal-with-150m-active-users.html) |
| 3 | Design a Rate Limiter | Medium | Stripe, Cloudflare, Google, Amazon | SDE, SRE, Backend | [Stripe Engineering Blog](https://stripe.com/blog/rate-limiters), [Grokking](https://www.educative.io/courses/grokking-modern-system-design-interview-for-engineers-managers/API-Rate-Limiter) |
| 4 | Design Netflix or YouTube (Video Streaming Service) | High | Netflix, YouTube, Amazon, Meta | SWE, Media, Backend | [Netflix Tech Blog](https://netflixtechblog.com/), [System Design Primer](https://github.com/donnemartin/system-design-primer/blob/master/solutions/system_design/youtube/README.md) |
| 5 | Design an Online Chat System (like WhatsApp) | Medium | Meta, Signal, Snap, Microsoft | SWE, Backend, Mobile | [WhatsApp Architecture](https://highscalability.com/blog/2022/1/25/whatsapp-architecture.html), [Grokking](https://www.educative.io/courses/grokking-modern-system-design-interview-for-engineers-managers/messenger-design) |
| 6 | Design Uber or Lyft | High | Uber, Lyft, DoorDash, Instacart | SWE, Backend, Mobile | [Uber Engineering Blog](https://eng.uber.com/), [Grokking](https://www.educative.io/courses/grokking-modern-system-design-interview-for-engineers-managers/uber-backend) |
| 7 | Design a Web Crawler | Medium | Google, Microsoft, Amazon, ByteDance | SWE, Search, Data | [Google Research](https://research.google/pubs/pub36701/), [System Design Primer](https://github.com/donnemartin/system-design-primer/blob/master/solutions/system_design/web_crawler/README.md) |
| 8 | Design Dropbox / Google Drive | High | Dropbox, Google, Microsoft, Box | SWE, Storage, Cloud | [Dropbox Tech Blog](https://dropbox.tech/), [System Design Primer](https://github.com/donnemartin/system-design-primer/blob/master/solutions/system_design/dropbox/README.md) |
| 9 | Design a Distributed Key-Value Store | High | Amazon, Google, Redis Labs, MongoDB | SWE, Database, Cloud | [DynamoDB Paper](https://www.allthingsdistributed.com/files/amazon-dynamo-sosp2007.pdf), [Google Spanner](https://research.google/pubs/pub39966/) |
| 10 | Design Instagram | Medium | Meta, Snap, ByteDance, Pinterest | SWE, Full-stack, Mobile | [Instagram Engineering](https://instagram-engineering.com/), [System Design Primer](https://github.com/donnemartin/system-design-primer/blob/master/solutions/system_design/instagram/README.md) |
| 11 | Design a Payment System | High | Stripe, PayPal, Square, Rippling | SWE, Financial, Security | [Stripe Engineering Blog](https://stripe.com/blog/engineering), [Grokking](https://www.educative.io/courses/grokking-modern-system-design-interview-for-engineers-managers/payment-processing-system-design) |
| 12 | Design a Search Autocomplete System | Medium | Google, Microsoft, Amazon, LinkedIn | SWE, Search, UX | [System Design Primer](https://github.com/donnemartin/system-design-primer/blob/master/solutions/system_design/autocomplete/README.md), [Grokking](https://www.educative.io/courses/grokking-modern-system-design-interview-for-engineers-managers/typeahead-suggestion) |
| 13 | Design a Recommendation System | High | Netflix, Amazon, Spotify, TikTok | SWE, ML, Data | [Netflix Recommendation](https://netflixtechblog.com/system-architectures-for-personalization-and-recommendation-e081aa94b5d8), [Amazon ML Blog](https://aws.amazon.com/blogs/machine-learning/) |
| 14 | Design an API Rate Limiter | Medium | AWS, Google Cloud, Cloudflare, Akamai | SWE, Cloud, Security | [AWS Architecture Blog](https://aws.amazon.com/blogs/architecture/), [Grokking](https://www.educative.io/courses/grokking-modern-system-design-interview-for-engineers-managers/API-Rate-Limiter) |
| 15 | Design a Notification Service | Medium | Meta, Slack, Discord, Salesforce | SWE, Mobile, Cloud | [Slack Engineering Blog](https://slack.engineering/), [Grokking](https://www.educative.io/courses/grokking-modern-system-design-interview-for-engineers-managers/notification-service-design) |
| 16 | Design Airbnb or Booking.com | High | Airbnb, Booking, Expedia, Tripadvisor | SWE, Full-stack, Search | [Airbnb Engineering Blog](https://medium.com/airbnb-engineering), [System Design Interview Vol 2](https://www.amazon.com/System-Design-Interview-Insiders-Guide/dp/1736049119) |
| 17 | Design a Content Delivery Network (CDN) | High | Cloudflare, Akamai, Fastly, AWS | SWE, Infrastructure, Network | [Cloudflare Blog](https://blog.cloudflare.com/), [AWS Architecture](https://aws.amazon.com/blogs/architecture/) |
| 18 | Design a Distributed Cache | Medium | Redis, Memcached, AWS, Google | SWE, Infrastructure, Cloud | [Redis Architecture](https://redis.com/redis-enterprise/technology/redis-architecture/), [Grokking](https://www.educative.io/courses/grokking-modern-system-design-interview-for-engineers-managers/key-value-store) |
| 19 | Design a Task Scheduler | Medium | Airflow, AWS, Google, Microsoft | SWE, Cloud, Data | [Apache Airflow](https://airflow.apache.org/docs/apache-airflow/stable/index.html), [AWS Architecture](https://aws.amazon.com/blogs/architecture/) |
| 20 | Design a Distributed Message Queue | High | Kafka, RabbitMQ, AWS, Google | SWE, Cloud, Infrastructure | [Kafka Architecture](https://kafka.apache.org/documentation/#design), [AWS Architecture](https://aws.amazon.com/blogs/architecture/) |
| 21 | Design a Distributed Logging System | Medium | Splunk, Elastic, Datadog, New Relic | SWE, DevOps, SRE | [Elastic Blog](https://www.elastic.co/blog/), [Splunk Architecture](https://docs.splunk.com/Documentation/Splunk/latest/Deploy/Distributedoverview) |
| 22 | Design Google Maps | High | Google, Apple, Uber, Tesla | SWE, Maps, Mobile | [Google Maps Platform Blog](https://cloud.google.com/blog/products/maps-platform), [System Design Interview Vol 2](https://www.amazon.com/System-Design-Interview-Insiders-Guide/dp/1736049119) |
| 23 | Design an AI Large Language Model (LLM) System | High | OpenAI, Google, Microsoft, Anthropic | SWE, ML, AI | [OpenAI System Card](https://openai.com/research/gpt-4-system-card), [LLM Architecture Papers](https://arxiv.org/abs/2303.18223) |
| 24 | Design a Real-time Collaboration Editor (like Google Docs) | High | Google, Microsoft, Notion, Coda | SWE, Frontend, Real-time | [Google Research](https://research.google/pubs/pub44830/), [System Design Interview Vol 2](https://www.amazon.com/System-Design-Interview-Insiders-Guide/dp/1736049119) |
| 25 | Design a Stock Trading System | High | Robinhood, Intuit, Citadel, JPMorgan | SWE, Financial, Real-time | [Robinhood Engineering Blog](https://robinhood.engineering/), [System Design Interview Vol 1](https://www.amazon.com/System-Design-Interview-insiders-Second/dp/B08CMF2CQF) |

## Latest System Design Questions for 2025

The system design landscape is rapidly evolving with new technologies and architectural patterns. Here are the most recent system design problems being asked in 2025 interviews at top tech companies:

| # | Problem | Complexity | Companies | Roles | Key Considerations |
|---|---------|------------|-----------|-------|-------------------|
| 1 | Design a Multi-Agent AI Orchestration System | Very High | OpenAI, Microsoft, Google, Anthropic | SWE-AI, ML Infra | Coordination protocols, safety mechanisms, observability, task delegation |
| 2 | Design an Edge Computing Platform for IoT | High | AWS, Google, Microsoft, Tesla | Cloud, IoT, Edge | Local processing, sync strategies, bandwidth optimization, hardware constraints |
| 3 | Design a Privacy-Preserving Analytics System | High | Apple, Meta, Google, Snap | Privacy, Data | Differential privacy, homomorphic encryption, federated analytics, compliance |
| 4 | Design a Real-time AI-assisted Coding Platform | High | GitHub, Microsoft, Google, JetBrains | SWE, Developer Tools | LLM integration, IDE extensions, model latency, context management |
| 5 | Design a Serverless Data Pipeline System | Medium | AWS, Google, Snowflake, Databricks | Data, Cloud | Event-driven processing, cost optimization, scaling, observability |
| 6 | Design a Voice-First Operating System | Very High | Amazon, Google, Apple, Meta | OS, Voice AI | Natural language understanding, ambient computing, privacy, context awareness |
| 7 | Design a Decentralized Social Network | High | Block, Consensys, Discord | Blockchain, Social | Content distribution, moderation, identity management, consensus mechanisms |
| 8 | Design a Spatial Computing OS | Very High | Apple, Meta, Microsoft, Magic Leap | AR/VR, OS | 3D rendering, gesture recognition, spatial mapping, device limitations |
| 9 | Design a Low-latency Global ML Inference System | High | OpenAI, Google, Anthropic, Meta | ML Infra, Cloud | Load balancing, model serving, region optimization, model quantization |
| 10 | Design a Quantum Computing Interface | Very High | IBM, Google, Microsoft, Amazon | Quantum, Cloud | Quantum-classical integration, error correction, abstraction layers |

### Emerging System Design Trends in 2025

Several key trends are shaping system design interviews in 2025:

1. **AI Integration at Scale**
   - Systems now commonly incorporate AI/ML components
   - Focus on handling model latency and unpredictability
   - Managing prompt engineering and context at scale
   - Robust handling of AI hallucinations and errors

2. **Multi-Agent Architectures**
   - Systems with multiple specialized AI agents working together
   - Orchestration and coordination mechanisms
   - Conflict resolution between agents
   - Safety guarantees and monitoring

3. **Edge-Cloud Hybrid Systems**
   - Processing sensitive data at the edge
   - Intelligent workload distribution
   - Handling intermittent connectivity
   - Resource-constrained optimization

4. **Privacy-Preserving Architectures**
   - Federated learning and analytics
   - Differential privacy implementations
   - Zero-knowledge proofs for verification
   - Data minimization and anonymization

5. **Real-time Collaboration at Scale**
   - Global distributed collaboration
   - Low-latency conflict resolution
   - Eventual consistency with immediate feedback
   - Multi-modal interaction (text, voice, visual)

## Advanced System Design Concepts for 2025

To excel in 2025 system design interviews, candidates should be familiar with these advanced concepts:

### 1. Serverless and Function-as-a-Service Evolution

The serverless paradigm has evolved beyond simple functions to complex workflows:

- **Stateful Serverless**: Managing state in serverless architectures
- **Serverless Workflows**: Orchestration of complex function chains
- **Cold Start Optimization**: Techniques to minimize cold start latency
- **FinOps for Serverless**: Cost optimization strategies for serverless at scale

### 2. AI Infrastructure Design

With AI becoming central to most systems, understanding AI infrastructure is critical:

- **Inference Optimization**: Techniques like quantization, batching, and KV caching
- **Model Lifecycle Management**: Versioning, A/B testing, and progressive rollouts
- **Prompt Engineering Infrastructure**: Systems for managing and optimizing prompts
- **Multi-Modal Integration**: Combining text, image, audio, and video models

### 3. Distributed Systems Resilience

Modern distributed systems require sophisticated resilience strategies:

- **Chaos Engineering**: Designing systems that withstand unexpected failures
- **Multi-Region Recovery**: Cross-region failover and replication strategies
- **Gray Failures**: Detecting and handling partial system failures
- **Backpressure Mechanisms**: Elegant degradation under load

### 4. Data Mesh Architectures

Data architecture has evolved from centralized lakes to distributed ownership:

- **Domain-Oriented Ownership**: Distributing data ownership to domain experts
- **Self-Serve Data Platforms**: Enabling teams to consume data without bottlenecks
- **Federated Governance**: Maintaining consistency while distributing control
- **Data Contracts**: Establishing clear interfaces between data producers and consumers

### 5. Event-Driven Systems

Event-driven architecture has become the backbone of reactive, scalable systems:

- **Event Sourcing at Scale**: Practical implementations for large-scale systems
- **CQRS Patterns**: Separating read and write models for performance
- **Stream Processing**: Real-time analytics and processing of event streams
- **Event Schema Evolution**: Managing changes to event structures over time

## Updated Interview Framework for 2025

The traditional system design interview framework has evolved to better assess candidates' ability to design modern systems:

### 1. Problem Exploration (5 minutes)
- Functional and non-functional requirements
- Scale, performance, and reliability expectations
- User profiles and access patterns
- **New**: AI/ML integration requirements
- **New**: Privacy and ethical considerations

### 2. High-Level Architecture (10 minutes)
- Core components and data flow
- API design and interfaces
- **New**: AI/ML component integration
- **New**: Edge-cloud distribution strategy

### 3. Component Deep Dive (15 minutes)
- Detailed design of 2-3 critical components
- Data models and schema design
- **New**: AI model selection and integration
- **New**: Privacy-preserving mechanisms

### 4. Scaling and Optimization (10 minutes)
- Horizontal vs. vertical scaling strategies
- Caching and performance optimizations
- **New**: AI inference optimization
- **New**: Cost optimization strategies

### 5. Operational Excellence (5 minutes)
- Monitoring and observability
- Deployment and rollback strategies
- **New**: Explainability and debugging
- **New**: Evolution and maintenance plans

### 6. Tradeoff Discussion (5 minutes)
- Explicit discussion of architectural tradeoffs
- Alternative approaches considered
- **New**: Ethical implications of design choices
- **New**: Future-proofing considerations

## Resources for 2025 System Design Preparation

Here are the latest resources to prepare for system design interviews in 2025:

1. **Books**
   - "System Design for AI Engineers" (New for 2025)
   - "Distributed Systems in the Age of AI" (Updated for 2025)
   - "Edge Computing: Architectures, Applications and Technologies" (2024)
   - "Designing Data-Intensive Applications" (Still relevant with 2025 updates)

2. **Engineering Blogs**
   - OpenAI System Design Blog
   - Microsoft AI Architecture Patterns
   - Google Cloud Architecture Center
   - AWS Serverless Land
   - Uber Engineering (Edge Computing section)

3. **Courses and Platforms**
   - "AI System Design Interviews" on Educative
   - "Modern System Design for Software Engineers" (Updated for 2025)
   - "EdgeComputing.io" - Specialized learning platform
   - "AIInfrastructure.dev" - New practice platform

## How to Stand Out in 2025 System Design Interviews

To truly excel in system design interviews in 2025, demonstrate these differentiating qualities:

1. **Balance Theoretical and Practical Knowledge**
   - Explain theoretical concepts but ground them in practical implementation details
   - Refer to real-world examples and case studies from industry

2. **Showcase T-Shaped Knowledge**
   - Demonstrate broad knowledge across multiple domains
   - Show deep expertise in at least one critical area (AI, distributed systems, etc.)

3. **Incorporate Emerging Technologies Judiciously**
   - Know when to apply new technologies vs. traditional approaches
   - Articulate clear reasoning for technology choices

4. **Address Cross-Cutting Concerns**
   - Proactively discuss security, privacy, and ethical considerations
   - Show awareness of regulatory requirements like GDPR, CCPA, or AI Act

5. **Demonstrate Systems Thinking**
   - Consider how components interact and affect the whole system
   - Anticipate emergent behaviors and failure modes

---

<div align="center">

### Connect With Me

If you found this resource helpful, please consider following me:

- **GitHub**: [@ombharatiya](https://github.com/ombharatiya)
- **Twitter**: [@ombharatiya](https://twitter.com/ombharatiya)
- **LinkedIn**: [ombharatiya](https://linkedin.com/in/ombharatiya)

I regularly share tech interview resources, system design concepts, and career advice for engineers. Your support helps keep these resources updated!

</div>

---

# Trending Coding Patterns for 2025

Beyond system design, coding interviews remain a crucial part of the technical interview process at top tech companies. Here are the most important coding patterns and questions trending in 2025 interviews:

## High-ROI Coding Patterns for 2025

Focusing on these patterns will give you the highest return on investment for your interview preparation:

### 1. Two Pointers Technique

**Applications**: Arrays, strings, linked lists
**Key Problems**:
- Two Sum variations (three sum, four sum)
- Container With Most Water
- Trapping Rain Water
- Palindrome verification
- Removing duplicates

**Example 2025 Question**:
```
Design an algorithm to find all unique quadruplets in an array that sum to a target, with O(n³) time complexity and optimized space usage.
```

### 2. Sliding Window

**Applications**: Arrays, strings, hash tables
**Key Problems**:
- Maximum sum subarray of size K
- Longest substring with K distinct characters
- Minimum window substring
- Longest substring without repeating characters

**Example 2025 Question**:
```
Given a string and a pattern, find all start indices of pattern's anagrams in the string with optimal time and space complexity.
```

### 3. Tree & Graph Traversals (DFS/BFS)

**Applications**: Binary trees, graphs, matrices
**Key Problems**:
- Path sum variations
- Binary tree level order traversal
- Course schedule (topological sort)
- Number of islands
- Word ladder

**Example 2025 Question**:
```
Design an algorithm to find the shortest path between two nodes in a weighted graph where weights represent time, but some edges can only be traversed during specific time windows.
```

### 4. Binary Search Variations

**Applications**: Sorted arrays, search space reduction
**Key Problems**:
- Search in rotated sorted array
- Find first and last position of element
- Median of two sorted arrays
- Kth smallest element in a sorted matrix

**Example 2025 Question**:
```
Design an algorithm to find the kth smallest element in a row-wise and column-wise sorted 2D array with optimal time complexity.
```

### 5. Dynamic Programming with Optimizations

**Applications**: Optimization problems, counting problems
**Key Problems**:
- Longest increasing subsequence
- Edit distance
- Coin change
- Unique paths
- Knapsack problem variants

**Example 2025 Question**:
```
Implement a space-optimized solution for the minimum cost to cut a rod into pieces of specific lengths, where each cut has a different cost.
```

### 6. Graph Algorithms (Advanced)

**Applications**: Social networks, routing, scheduling
**Key Problems**:
- Network delay time
- Minimum spanning tree
- Strongly connected components
- Shortest path algorithms (Dijkstra's, Bellman-Ford)

**Example 2025 Question**:
```
Design an algorithm to find the most efficient way to connect multiple servers where connection costs vary based on data transfer rates and physical distance.
```

### 7. Interval Merging and Processing

**Applications**: Calendar scheduling, resource allocation
**Key Problems**:
- Merge intervals
- Insert interval
- Meeting rooms
- Non-overlapping intervals

**Example 2025 Question**:
```
Implement an algorithm that can schedule optimal maintenance windows for a system with multiple components, each requiring different maintenance intervals.
```

## Latest Coding Questions at Top Companies (2025)

| Company | Question | Difficulty | Pattern |
|---------|----------|------------|---------|
| Google | Design a time-based key-value store with versioning and queryable history | Hard | Hash Table + Binary Search |
| Meta | Implement an algorithm to detect when a user's social feed should be refreshed based on friend activity patterns | Medium | Graph + Sliding Window |
| Amazon | Design an inventory management system that optimizes for both space utilization and retrieval time | Hard | Heap + DP |
| Microsoft | Implement a smart code autocomplete system that learns from user corrections | Hard | Trie + ML |
| OpenAI | Design an algorithm to detect and rank the relevance of hallucinated content in an LLM output | Hard | NLP + DP |
| Apple | Implement a privacy-preserving data structure for on-device analytics | Medium | Bloom Filter + Cryptography |
| Netflix | Design a content recommendation system that balances user preferences with content diversity | Hard | Graph + Prioritization |
| Uber | Optimize driver-to-rider matching in a dynamic environment with changing traffic conditions | Hard | Graph + Greedy |

## Preparation Strategy for 2025

1. **Master the Fundamentals**: Ensure you have a solid understanding of data structures, algorithms, and complexity analysis.

2. **Pattern Recognition**: Group problems by patterns rather than by data structures. This helps apply solutions across different contexts.

3. **Practice Optimization**: Don't stop at a working solution; focus on optimizing time and space complexity.

4. **Mock Interviews**: Schedule regular mock interviews to simulate real interview conditions.

5. **Verbalize Your Thinking**: Practice explaining your thought process while coding.

6. **Learn from Solutions**: After solving a problem, study multiple approaches to understand different perspectives.

7. **Consistent Practice**: Aim for consistent daily practice rather than cramming.

## Advanced Topics to Master in 2025

- **Quantum Algorithm Basics**: Understanding quantum computing principles is becoming relevant for specific roles.
- **AI/ML Algorithms**: Familiarity with fundamental ML algorithms and data structures.
- **Distributed Systems Coding**: Problems involving distributed data structures and algorithms.
- **Blockchain Data Structures**: Understanding merkle trees, cryptographic hashes, and consensus algorithms.
- **Edge Computing Optimizations**: Algorithms optimized for resource-constrained environments.

By focusing on these patterns and topics, you'll be well-prepared for coding interviews at top tech companies in 2025.

---

_Last updated: March 2025_ 