<h1 align="center">Hey, I'm Aman 👋</h1>
<h3 align="center">Senior Software Engineer · I build the backend that moves money</h3>

<p align="center">
  <a href="https://linkedin.com/in/aman5vats"><img src="https://img.shields.io/badge/LinkedIn-aman5vats-0A66C2?style=flat&logo=linkedin&logoColor=white" /></a>
  <a href="mailto:aman810433@gmail.com"><img src="https://img.shields.io/badge/Email-aman810433%40gmail.com-D14836?style=flat&logo=gmail&logoColor=white" /></a>
  <img src="https://img.shields.io/badge/Based%20in-Gurugram%2C%20India-555?style=flat" />
</p>

---

### 💸 What I do

I'm a backend engineer on the **Peer-to-Peer team at PayPay**, Japan's largest payments app
(**75M+ registered users, more than half of Japan's population**). I work on the systems behind sending and
requesting money, used by tens of millions of people every month. Before that I worked on payments and cashback at
PayPay, and on loyalty, onboarding and credit-score products at **ZET**.

I care about the unglamorous parts that make payments trustworthy: **idempotency, reconciliation, safe retries,
backward-compatible rollouts, and knowing exactly why a service woke someone up at 3 a.m.**

### 🏗️ Things I've shipped

- **P2P payments inside the LINE super-app**: owned it end to end, from API contracts to production launch.
  Send money, request money and bank sync across three microservices, with idempotency and risk checks,
  and zero regression on PayPay's own flows.
- **25× more friends per account (200 → 5,000)**: benchmarked Aurora MySQL across 200K+ relationships,
  proved the indexes scale sub-linearly, wrote the design doc, and shipped it to production.
- **PayPay Points for shopping on LINE**: built the backend that credits PayPay Points when users shop on LINE Yahoo services.
- **Payment flows that recover safely**: debit, refund, reversal, partial capture and re-authorization.
- **A 160M-record customer migration** at ZET, plus cutting MySQL CPU from 98% to 20%.

### 🔍 Favourite debugging story

A long-running Kafka consumer kept dying with `OutOfMemoryError`, and the problem kept recurring across teams.
I traced it to Micrometer metrics piling up in the JVM's Old Gen. The cause turned out to be a
Prometheus whitelist mismatch: metrics were being created but never scraped, so nothing ever released them.

The fix was **two lines**. Metric growth dropped from **52/hour to 0.11/hour**, and it ran clean across
**19.85M messages** with no OOM since.

### 🧰 Tools of the trade

![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat&logo=kotlin&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
![Scala](https://img.shields.io/badge/Scala-DC322F?style=flat&logo=scala&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat&logo=springboot&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat&logo=apachekafka&logoColor=white)
![MySQL](https://img.shields.io/badge/Aurora%20MySQL-4479A1?style=flat&logo=mysql&logoColor=white)
![TiDB](https://img.shields.io/badge/TiDB-DD0031?style=flat&logo=tidb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)
![DynamoDB](https://img.shields.io/badge/DynamoDB-4053D6?style=flat&logo=amazondynamodb&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazonwebservices&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat&logo=terraform&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat&logo=prometheus&logoColor=white)
![New Relic](https://img.shields.io/badge/New%20Relic-1CE783?style=flat&logo=newrelic&logoColor=black)

### 🌱 Right now

- Scaling P2P social features at PayPay
- Using LLM tools and agentic workflows to explore unfamiliar services and debug faster
- Mentoring junior engineers on owning a service in production

### ✨ Outside the code

- Featured in PayPay Inside-Out: [**Owning Decisions at 70 Million Scale**](https://insideout.paypay.ne.jp/en/2026/04/13/pay2-dev-speaks-vol18-en/), on engineering ownership in P2P
- Featured in ZET's [**Life of a Backend Engineer**](https://www.linkedin.com/pulse/life-backend-engineer-zet-zetapp-in/) series
- Founding member of *Periods and You*, Pad Bank Prayaas
- IIIT Allahabad alum

---

<p align="center"><i>Happy to talk about payments, distributed systems, or a good production mystery.</i></p>
