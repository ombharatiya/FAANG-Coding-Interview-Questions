# 🚀 FAANG System Design Interview Guide 🚀

## 25 Must-Do System Design Problems for Tech Interviews

| No. | System Design Problem | Complexity | Common in Companies | Target Roles |
|-----|----------------------|------------|---------------------|-------------|
| 1 | [Design a URL Shortening Service (TinyURL)](https://leetcode.com/discuss/interview-question/124658/Design-a-URL-Shortener-(-TinyURL-)-System/) | Medium | Google, Microsoft, Twitter, Salesforce | SWE, Senior SWE |
| 2 | [Design Twitter/X](https://leetcode.com/discuss/interview-question/system-design/124689/Design-Twitter) | Hard | Twitter, Meta, Microsoft, OpenAI | Senior SWE, Staff Engineer |
| 3 | [Design Netflix/Video Streaming Platform](https://leetcode.com/discuss/interview-question/system-design/158698/Design-Netflix) | Hard | Netflix, Amazon, Google, Meta | Senior SWE, Systems Architect |
| 4 | [Design a Distributed Cache](https://leetcode.com/discuss/interview-question/system-design/125751/Design-a-distributed-cache) | Hard | Google, Amazon, Microsoft, Rippling | Senior SWE, Infrastructure Engineer |
| 5 | [Design Instagram](https://leetcode.com/discuss/interview-question/system-design/124802/Design-Instagram) | Hard | Meta, Snap, ByteDance, Tesla | Senior SWE, Backend Engineer |
| 6 | [Design Uber/Ride-sharing Service](https://leetcode.com/discuss/interview-question/system-design/124542/Design-Uber-or-Lyft) | Hard | Uber, Lyft, Intuit, Tesla | Senior SWE, Backend Engineer |
| 7 | [Design WhatsApp/Messaging System](https://leetcode.com/discuss/interview-question/system-design/124613/Design-WhatsApp) | Medium-Hard | Meta, Microsoft, Telegram | Senior SWE, Mobile Engineer |
| 8 | [Design Google Drive/Dropbox](https://leetcode.com/discuss/interview-question/system-design/123605/Design-Google-Drive-or-Dropbox-File-Sharing-and-Storage-Service) | Hard | Google, Dropbox, Microsoft, Box | Senior SWE, Storage Engineer |
| 9 | [Design a Web Crawler](https://leetcode.com/discuss/interview-question/system-design/124657/Design-a-Web-Crawler) | Medium-Hard | Google, Microsoft, Amazon, OpenAI | Senior SWE, Search Engineer |
| 10 | [Design Ticketmaster/Booking System](https://www.hellointerview.com/learn/system-design/answer-keys/ticketmaster) | Medium-Hard | Microsoft, Salesforce, Intuit | Senior SWE, Full Stack Engineer |
| 11 | [Design Google Maps](https://leetcode.com/discuss/interview-question/system-design/124673/Design-Google-Maps) | Hard | Google, Uber, Tesla, Amazon | Senior SWE, ML Engineer |
| 12 | [Design YouTube](https://leetcode.com/discuss/interview-question/system-design/133251/Design-YouTube) | Hard | Google, Meta, Netflix, ByteDance | Senior SWE, Media Engineer |
| 13 | [Design Facebook Newsfeed](https://leetcode.com/discuss/interview-question/system-design/124682/Design-Facebook-Newsfeed) | Hard | Meta, LinkedIn, Twitter | Senior SWE, Data Engineer |
| 14 | [Design Spotify/Music Streaming Service](https://www.educative.io/blog/favorite-system-design-question) | Medium-Hard | Spotify, Apple, Amazon, Salesforce | Senior SWE, Full Stack Engineer |
| 15 | [Design Typeahead Suggestion/Autocomplete](https://leetcode.com/discuss/interview-question/system-design/124671/Design-typeahead-search-or-autocomplete) | Medium | Google, Meta, Amazon, Intuit | Senior SWE, Search Engineer |
| 16 | [Design a Rate Limiter](https://leetcode.com/discuss/interview-question/system-design/124558/Designing-API-Rate-Limiter) | Medium | Stripe, Rippling, AWS, Cloudflare | Senior SWE, Backend Engineer |
| 17 | [Design Nearby Friends Feature](https://leetdesign.com/problems/nearby-friends) | Medium | Meta, Snap, Tinder, Uber | Senior SWE, Mobile Engineer |
| 18 | [Design Google Search](https://leetcode.com/discuss/interview-question/system-design/124584/Design-a-search-engine-like-Google) | Very Hard | Google, Microsoft, OpenAI | Staff Engineer, Search Engineer |
| 19 | [Design a Collaborative Document Editing System (Google Docs)](https://leetcode.com/discuss/interview-question/system-design/133751/Design-Google-Docs) | Hard | Google, Microsoft, Salesforce | Senior SWE, Full Stack Engineer |
| 20 | [Design an LLM-powered Enterprise Search System](https://igotanoffer.com/blogs/tech/system-design-interviews) | Hard | OpenAI, Google, Microsoft, Salesforce | Senior SWE, ML Engineer |
| 21 | [Design an E-commerce Platform](https://leetcode.com/discuss/interview-question/system-design/124752/Design-an-E-commerce-Website) | Medium-Hard | Amazon, Walmart, Intuit, Salesforce | Senior SWE, Full Stack Engineer |
| 22 | [Design a Notification System](https://leetcode.com/discuss/interview-question/system-design/123881/Design-a-notification-system) | Medium | Meta, Slack, Twitter, Rippling | Senior SWE, Backend Engineer |
| 23 | [Design a Distributed Job Scheduler](https://leetcode.com/discuss/interview-question/system-design/124628/Design-a-distributed-job-scheduler) | Hard | AWS, Google, Microsoft, Tesla | Senior SWE, Infrastructure Engineer |
| 24 | [Design a Payment System](https://leetcode.com/discuss/interview-question/system-design/158842/Design-Payment-System) | Hard | PayPal, Stripe, Square, Intuit | Senior SWE, Financial Tech Engineer |
| 25 | [Design a Stock Trading System](https://leetcode.com/discuss/interview-question/system-design/125218/Design-a-stock-trading-system) | Very Hard | Robinhood, Bloomberg, Intuit, Rippling | Senior SWE, Financial Tech Engineer |

## Key Complexity Factors for System Design Interviews

When preparing for these system design problems, focus on these key aspects that determine their complexity:

1. **Scale**: How many users/requests must the system handle?
2. **Availability**: What level of uptime is required?
3. **Consistency**: What consistency model is needed (eventual vs. strong)?
4. **Latency**: What are the response time requirements?
5. **Data Storage**: What volume and type of data must be managed?
6. **Security**: What security considerations are critical?

## Interview Tips for System Design

1. **Clarify Requirements**: Begin by asking questions to understand exactly what you need to design.
2. **Define Scope**: Establish what's in and out of scope for the discussion.
3. **High-Level Architecture**: Start with a high-level design before diving into details.
4. **Focus on Trade-offs**: Discuss the pros and cons of your design choices.
5. **Consider Scale**: Always think about how your system would scale to millions of users.
6. **Data Model**: Define a clear data model with appropriate relationships.
7. **Be Pragmatic**: Use existing technologies and patterns rather than inventing new ones.

## Company-Specific Focus Areas

- **Google**: Search systems, distributed computing, scalability
- **Meta**: Social networks, content delivery, real-time systems
- **Amazon**: E-commerce, inventory systems, recommendation engines
- **Microsoft**: Enterprise software, collaboration tools, cloud infrastructure
- **Apple**: User experience, privacy-focused design, device integration
- **Netflix**: Content delivery, recommendation systems, A/B testing
- **OpenAI**: ML systems, content moderation, large-scale inference
- **Tesla**: Real-time systems, sensor data processing, autonomous features
- **Rippling**: HR systems, identity management, enterprise integrations
- **Salesforce**: CRM systems, multi-tenancy, enterprise security

---

## 💫 Connect With Me! 💫

If you found this guide helpful, please consider following me on:

- **GitHub**: [@ombharatiya](https://github.com/ombharatiya)
- **Twitter**: [@ombharatiya](https://twitter.com/ombharatiya)
- **LinkedIn**: [ombharatiya](https://linkedin.com/in/ombharatiya)

I regularly share more tech interview preparation resources, coding tips, and career advice for developers aiming for top tech companies. Your support means a lot! ⭐

**Got questions or suggestions?** Feel free to reach out or contribute to this repository.

---

_Last updated: March 2025_ 