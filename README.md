<img src="https://capsule-render.vercel.app/api?type=waving&color=0:121413,100:c6f432&height=200&section=header&text=Swamil%20Randive&fontSize=48&fontColor=e9ece8&fontAlignY=38&desc=Backend%20%C2%B7%20Distributed%20Systems%20%C2%B7%20AI&descSize=16&descAlignY=58&descColor=e9ece8" width="100%" />

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=20&pause=1200&color=C6F432&center=true&vCenter=true&width=620&lines=Backend+Engineering;Distributed+Systems;Storage+Engines+%26+Messaging;Software+Architecture;Artificial+Intelligence;Computer+Vision" alt="Backend Engineering, Distributed Systems, Storage Engines and Messaging, Software Architecture, AI, Computer Vision" />
</p>

<p align="center">
Computer Science Engineer · Software Developer · Master's student at the University of Siegen
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=swamil-5504&label=PROFILE+VIEWS&color=c6f432&style=flat-square&labelColor=121413" />
  <img src="https://img.shields.io/github/followers/swamil-5504?label=FOLLOWERS&style=flat-square&color=c6f432&labelColor=121413" />
  <img src="https://img.shields.io/badge/LOCATION-Siegen%2C%20DE-c6f432?style=flat-square&labelColor=121413" />
</p>

I'm a backend engineer who likes understanding systems from the inside out. I build things from first principles (logs, sockets, protocols, coordination) so I know *why* production systems behave the way they do, not just how to use them.

---

## ⚡ Currently

- 🔨 Building **[BLACKBOX](https://github.com/swamil-5504/BLACKBOX)**, a Kafka-inspired message broker in plain Java
- 🎓 Pursuing my M.Sc. in Computer Science (*Complex and Intelligent Software Systems*) at the **University of Siegen**
- 📚 Going deeper into distributed systems, storage engines and computer vision

---

## 🚀 Projects

### [BLACKBOX](https://github.com/swamil-5504/BLACKBOX): Kafka-inspired distributed messaging broker

`Java` · `Java NIO` · `TCP` · `Jackson` · `Gradle`

A message broker built from scratch with no messaging framework, to understand how systems like Kafka work internally.

- **Storage:** append-only binary partition logs on `FileChannel`, sequential per-partition offsets, and automatic recovery of topics and offsets on restart.
- **Messaging:** topics with configurable partitions, a thread-safe round-robin producer, and offset-based consumers.
- **Consumer groups:** membership, topic subscriptions, round-robin partition assignment and **automatic rebalancing** when consumers join or leave.
- **Safety:** assignment-aware fetching (a consumer can only read partitions it owns) and validated, persistent per-group committed offsets for at-least-once consumption.
- **Protocol:** newline-delimited JSON over TCP with 10 commands and a thread per client connection.
- **Multi-broker networking:** shared cluster config, separate client and internal ports, a validated handshake (broker ID and cluster name), startup retries, and persistent inter-broker connections with PING/PONG.

Replication, metadata sync, leader election and failover are the next steps.

```mermaid
flowchart LR
    P[Producers] -->|JSON over TCP| B1
    CG[Consumer Groups] -->|JSON over TCP| B1

    subgraph Cluster["Cluster: blackbox-local"]
        direction LR
        B1[Broker 1] <-->|"internal port<br/>handshake + PING/PONG"| B2[Broker 2]
        B2 <--> B3[Broker 3]
        B1 <--> B3
    end

    subgraph Broker["Inside a broker"]
        direction TB
        TM[Topic Manager] --> L[("Partition logs<br/>append-only")]
        GM[Group Manager] --> PA[Assignment and rebalancing]
        OM[Offset Manager] --> O[("Committed offsets<br/>JSON")]
    end

    B1 -.-> Broker
```

### PropertiesAnywhere: full-stack Android app for property rental

`Flutter` · `Dart` · `Java` · `Spring Boot` · `PostgreSQL`

A property-rental app with user authentication, property listings, city-based search and listing management. It includes a messaging system between users with read/unread status and unread-message counters, and connects the mobile app to REST APIs and a PostgreSQL-backed Spring Boot service.

### Altrium: blockchain-based degree verification

`React` · `TypeScript` · `FastAPI` · `MongoDB` · `Solidity` · `Docker`

A platform where universities issue tamper-proof **Soulbound Tokens** on Ethereum Sepolia and employers verify degree credentials instantly. It includes role-based access control, validation of university accreditation, Telegram notifications and Docker-based deployment.

---

## 💼 Experience

| Role | Company | When | Stack | Highlights |
|---|---|---|---|---|
| Product Engineer Intern | **Allstate India** | Feb – Jul 2026 | Java, Spring Boot, React | Backend services and REST APIs for the Vendor Assignment Tool (VAT) |
| Software Engineering Intern | **ThriveStack.ai** | Sep – Dec 2025 | Go, gRPC, GraphQL, Next.js, ClickHouse | **42%** ClickHouse query performance improvement |
| Backend Engineer Intern | **GoQuant** | Jun – Sep 2025 | FastAPI, OEMS backend, FIX protocol | OTC desk integrations, **28%** order throughput increase |

---

## 📄 Publications

- *Automated Psychological Profiling from Children's Drawings Using Deep Learning and NLP*, IEEE ICoICC 2025
- *IoT and AI-Driven Dynamic Traffic Signal Manipulation using V2I Communication*, IEEE ICICCS 2025
- *Leveraging Computer Vision to create an Intelligent Threat Detection System for Visually Impaired*, IEEE IITCEE 2025

---

## 🧰 Tech

<p>
  <img src="https://skillicons.dev/icons?i=cpp,java,py,go,js,ts,spring,fastapi,react,nextjs,flutter,graphql,postgres,mysql,mongodb,docker,linux,git,gradle&theme=dark" />
</p>

**Where I'm strongest:** backend services (Java/Spring Boot, Go, Python/FastAPI), data-heavy query paths (ClickHouse, GraphQL, gRPC), low-level systems work (storage, sockets, protocols), and financial-systems integration (FIX).

---

## 📫 Contact

<p align="center">
  <a href="https://www.linkedin.com/in/swamil-randive-00070a246/"><img src="https://img.shields.io/badge/LinkedIn-121413?style=for-the-badge&logo=linkedin&logoColor=c6f432" /></a>
  <a href="mailto:swamilrandive47@gmail.com"><img src="https://img.shields.io/badge/Email-121413?style=for-the-badge&logo=gmail&logoColor=c6f432" /></a>
  <a href="https://github.com/swamil-5504"><img src="https://img.shields.io/badge/GitHub-121413?style=for-the-badge&logo=github&logoColor=c6f432" /></a>
</p>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:121413,100:c6f432&height=100&section=footer" width="100%" />
