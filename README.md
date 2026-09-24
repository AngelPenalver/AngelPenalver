# 👋 Hi, I'm Ángel Peñalver
**Backend Engineer | Node.js · NestJS · TypeScript · Distributed Systems**
Focused on designing resilient, scalable backend architectures, managing concurrency at the database level, and building asynchronous event-driven pipelines.
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/angelpenalver)
[![Email](https://img.shields.io/badge/Email-apenalver4%40gmail.com-D14836?style=flat&logo=gmail&logoColor=white)](mailto:apenalver4@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-Live-2ea44f?style=flat&logo=vercel&logoColor=white)](https://portfolio-angelpenalver.vercel.app)
---
## 💡 About Me
I design and build backend services with a production-first mindset. I care deeply about **data integrity, system predictability, and architecture that doesn't collapse under load**.
Rather than chasing framework hype, my engineering focus is centered on:
- **Concurrency & State Consistency:** Mitigating race conditions using database-level locking strategies.
- **Asynchronous Processing:** Decoupling heavy workloads through message queues and background workers.
- **Maintainable Architecture:** Implementing Hexagonal Architecture (Ports & Adapters) and SOLID principles to keep business logic agnostic of frameworks and infrastructure.
- **AI Integration in Production:** Orchestrating LLMs reliably through asynchronous queues and resilient error handling.
---
## 📌 Featured Engineering Projects
### 🎫 [Atomic Ticket — High-Concurrency Reservation Engine](https://github.com/AngelPenalver)
> A transactional booking backend designed to prevent overbooking and double-allocation under burst traffic.
- **Challenge:** Preventing Race Conditions when hundreds of users attempt to reserve the same seat simultaneously.
- **Solution:** Implemented **Pessimistic Locking (`SELECT FOR UPDATE`)** in PostgreSQL managed through TypeORM transactions.
- **Payments:** Decoupled asynchronous checkout reconciliation using **Stripe Webhooks**.
- **Stack:** `NestJS`, `TypeScript`, `PostgreSQL`, `TypeORM`, `Docker`, `Stripe API`.
### ⚡ [ContactShip — Async Lead Pipeline & AI Processing](https://github.com/AngelPenalver)
> An event-driven lead management system integrating generative AI for automated summarization without degrading API latency.
- **Challenge:** Offloading slow LLM inference and third-party API calls outside the client request-response lifecycle.
- **Solution:** Architected background workers using **BullMQ on Redis** with automatic retry policies and dead-letter handling.
- **AI Integration:** Automated extraction and synthesis via **Google Gemini API**.
- **Stack:** `NestJS`, `TypeScript`, `Redis`, `BullMQ`, `Google Gemini API`, `Docker`.
### 🔍 [Search & Catalog Microservice — Hexagonal Architecture](https://github.com/AngelPenalver)
> A decoupled product catalog and search service built strictly following Domain-Driven Design (DDD) principles.
- **Challenge:** Creating a core domain completely insulated from external database drivers and search engines.
- **Solution:** Applied **Ports & Adapters**, using **Elasticsearch** for full-text querying and **Redis** for sub-millisecond caching.
- **Stack:** `NestJS`, `TypeScript`, `Elasticsearch`, `Redis`, `TypeORM`.
---
## 🛠 Tech Stack & Engineering Skills
Backend Core :: Node.js, NestJS, TypeScript, Express Databases :: PostgreSQL, Redis, MySQL, MongoDB Architecture :: Hexagonal (Ports & Adapters), DDD, Clean Architecture, REST APIs Async & Queues :: BullMQ, Redis Queues, Event-Driven Patterns Integrations & AI :: Google Gemini API, Stripe Payments & Webhooks, Auth0, OAuth2 DevOps & Quality :: Docker, Jest (Unit & Integration Testing), Swagger/OpenAPI, Git



---
## ⚙️ How I Work & Engineering Values
- **Simplicity Over Ego:** I advocate for a well-structured Modular Monolith before prematurely introducing distributed microservices complexity.
- **Database-First Integrity:** Business rules belong in the domain, but consistency guarantees must be backed by appropriate database constraints and transactions.
- **Resilient Asynchrony:** Any operation that takes longer than 150ms or depends on an external API (AI, payments, emails) is offloaded to a queue.
---
## 📬 Connect With Me
- **LinkedIn:** [linkedin.com/in/angelpenalver](https://www.linkedin.com/in/angelpenalver/)
- **Email:** [apenalver4@gmail.com](mailto:apenalver4@gmail.com)
- **Portfolio:** [portfolio-angelpenalver.vercel.app](https://portfolio-angelpenalver.vercel.app)
---
<p align="center">
  <i>"Simplicity is prerequisite for reliability." — Edsger W. Dijkstra</i>
</p>
