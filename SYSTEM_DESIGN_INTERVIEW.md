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

## How to Prepare for System Design Interviews

### Framework for Approaching System Design Questions

Follow this structured approach to tackle system design problems effectively:

1. **Clarify Requirements (3-5 minutes)**
   - Functional requirements (what the system should do)
   - Non-functional requirements (scale, performance, latency, reliability)
   - Ask clarifying questions to narrow down the scope

2. **High-Level Design (10-15 minutes)**
   - Draw the major components and their connections
   - Identify the core services and subsystems
   - Discuss data flow between components

3. **Deep Dive (15-20 minutes)**
   - Pick 2-3 key components to detail further
   - Discuss database schema, API design, algorithms
   - Address potential bottlenecks and their solutions

4. **Scaling & Optimization (5-10 minutes)**
   - Discuss how to scale the system (horizontal vs. vertical)
   - Propose optimizations for performance and reliability
   - Consider caching strategies, load balancing, etc.

5. **Wrap-up (3-5 minutes)**
   - Summarize your approach
   - Discuss additional considerations or improvements
   - Reflect on trade-offs made in your design

### Key Topics to Study

To prepare thoroughly for system design interviews, ensure you understand these fundamental concepts:

1. **Scalability Fundamentals**
   - Horizontal vs. Vertical scaling
   - Load balancing techniques
   - Database sharding and partitioning

2. **High Availability & Reliability**
   - Redundancy and replication
   - Failover strategies
   - Disaster recovery

3. **Performance Optimization**
   - Caching strategies (CDN, in-memory, database)
   - Content delivery optimization
   - Read/write optimizations

4. **Data Storage**
   - SQL vs. NoSQL databases
   - Data partitioning strategies
   - Storage hierarchies (hot/warm/cold)

5. **Communication Patterns**
   - REST API design
   - Synchronous vs. asynchronous communication
   - Pub/Sub models
   - Websockets & real-time communication

6. **Monitoring & Error Handling**
   - Metrics and logging
   - Alerting systems
   - Graceful degradation

## Company-Specific Focus Areas

Different companies tend to emphasize certain aspects of system design in their interviews:

- **Google**: Scalability, distributed systems, and search-related components
- **Amazon**: Highly available systems, microservices, and AWS infrastructure
- **Microsoft**: API design, scalable architecture, and integration with Microsoft services
- **Meta**: Social graph systems, content delivery, and real-time features
- **Netflix**: Video streaming, recommendation engines, and global content delivery
- **Uber/Lyft**: Location services, real-time matching, and distributed systems
- **OpenAI/Anthropic**: ML infrastructure, model serving, and scaling AI systems
- **Financial Companies** (Stripe, PayPal): Security, consistency, and transaction processing

## Resources for Further Learning

- [System Design Primer](https://github.com/donnemartin/system-design-primer)
- [Grokking the System Design Interview](https://www.educative.io/courses/grokking-modern-system-design-interview-for-engineers-managers)
- [System Design Interview: An Insider's Guide](https://www.amazon.com/System-Design-Interview-insiders-Second/dp/B08CMF2CQF)
- [Designing Data-Intensive Applications](https://www.amazon.com/Designing-Data-Intensive-Applications-Reliable-Maintainable/dp/1449373321)
- [High Scalability Blog](http://highscalability.com/)
- [Company Engineering Blogs](https://github.com/kilimchoi/engineering-blogs) (great for real-world architecture)

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

_Last updated: March 2025_ 