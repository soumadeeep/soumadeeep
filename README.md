# Hi, I'm Soumadeep 👋

## Backend Engineer building reliable, event-driven payment systems

I design and build backend systems that remain reliable under retries, traffic spikes, duplicate events, and partial failures. My current focus is production-oriented fintech infrastructure, asynchronous processing, distributed systems, and transactional correctness.

I’m open to conversations about **Backend Engineer**, **Node.js**, **Distributed Systems**, and **Fintech** opportunities.

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&color=58A6FF&center=true&vCenter=true&width=760&lines=Backend+Engineer;Event-Driven+Systems+Builder;Fintech+%26+Distributed+Systems+Enthusiast;Open+to+engineering+opportunities" alt="Backend Engineer | Event-Driven Systems Builder | Fintech Enthusiast" />
</p>

## Featured Project

### High-Throughput Fintech Payment Webhook & Ledger Pipeline

**[Payment-Webhook](https://github.com/soumadeeep/Payment-Webhook)** is an event-driven backend system designed to process high-volume payment webhooks safely and asynchronously.

The project focuses on the engineering challenges that matter in payment infrastructure:

- ⚡ **Fast acknowledgment:** verifies HMAC-SHA256 signatures and acknowledges requests quickly before heavy database work
- 📨 **Reliable asynchronous processing:** uses RabbitMQ to absorb traffic bursts and decouple ingestion from workers
- 🔁 **Idempotency:** combines Redis atomic locks with MySQL unique constraints to prevent duplicate financial transactions
- 🔐 **Correct state transitions:** handles out-of-order payment events with pessimistic row locking and a finite state machine
- 💰 **Double-entry accounting:** records immutable ledger entries while ensuring debits and credits remain balanced
- 🛡️ **Production-minded security:** designed for deployment behind Cloudflare/WAF with edge rate limiting and DDoS mitigation

### Architecture

```text
Payment Gateway
      │
      ▼
Express Ingestion API
(HMAC verification + fast ACK)
      │
      ▼
RabbitMQ Durable Queue
      │
      ▼
Background Workers
(Redis idempotency + FSM validation)
      │
      ▼
MySQL / Sequelize
(ACID transactions + double-entry ledger)
```

## Technology Stack

### Backend & Runtime

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=flat-square&logo=express&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

### Data & Messaging

![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Sequelize](https://img.shields.io/badge/Sequelize-52B0E7?style=flat-square&logo=sequelize&logoColor=white)

### Engineering Interests

- Event-driven architecture
- Distributed systems and backpressure
- Payment processing and financial consistency
- Idempotency and exactly-once business effects
- ACID transactions and database locking
- API security and webhook verification
- Scalable backend architecture

## What I Bring

- A systems-first approach to backend engineering
- Strong attention to correctness in financial workflows
- Practical understanding of queues, retries, locks, and failure handling
- Curiosity and willingness to learn from experienced engineering teams
- Motivation to build dependable products that solve real problems

## Open to Opportunities

I’m currently interested in:

- Backend Engineer roles
- Node.js Engineer roles
- Fintech and payment infrastructure teams
- Distributed systems and platform engineering opportunities
- Backend-focused internships and collaborations

If you’re building reliable products or payment infrastructure, I’d be happy to connect and discuss how I can contribute.

## Let's Connect

- GitHub: [@soumadeeep](https://github.com/soumadeeep)
- LinkedIn: **add your LinkedIn profile URL**
- Email: **add your professional email address**

<p align="center">
  <a href="https://github.com/soumadeeep/Payment-Webhook">
    <img src="https://img.shields.io/badge/Featured%20Project-Payment--Webhook-0A66C2?style=for-the-badge&logo=github" alt="Featured Payment Webhook Project" />
  </a>
</p>
