<img src="https://capsule-render.vercel.app/api?type=waving&color=0:121413,100:c6f432&height=200&section=header&text=Swamil%20Randive&fontSize=48&fontColor=e9ece8&fontAlignY=38&desc=Backend%20%C2%B7%20Distributed%20Systems%20%C2%B7%20AI&descSize=16&descAlignY=58&descColor=e9ece8" width="100%" />

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=20&pause=1200&color=C6F432&center=true&vCenter=true&width=620&lines=Backend+Engineering;Distributed+Systems;Software+Architecture;Artificial+Intelligence;Computer+Vision" />
</p>

<p align="center">
Computer Science Engineer · Software Developer · Master's student at the University of Siegen
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=swamil-5504&label=PROFILE+VIEWS&color=c6f432&style=flat-square&labelColor=121413" />
  <img src="https://img.shields.io/github/followers/swamil-5504?label=FOLLOWERS&style=flat-square&color=c6f432&labelColor=121413" />
  <img src="https://img.shields.io/github/stars/swamil-5504?label=TOTAL%20STARS&style=flat-square&color=c6f432&labelColor=121413&affiliations=OWNER" />
  <img src="https://img.shields.io/badge/LOCATION-Siegen%2C%20DE-c6f432?style=flat-square&labelColor=121413" />
</p>

---

## ⚡ Currently
- 🔨 Building **BLACKBOX**, a message broker from scratch in Java
- 🎓 Pursuing my Master's at the **University of Siegen**
- 📚 Digging deeper into distributed systems, storage engines and computer vision

---

## 🚀 Featured project

<p align="center">
  <a href="https://github.com/swamil-5504/BLACKBOX">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=swamil-5504&repo=BLACKBOX&show_owner=false&hide_border=true&bg_color=121413&title_color=c6f432&icon_color=c6f432&text_color=e9ece8" />
  </a>
</p>

**[BLACKBOX](https://github.com/swamil-5504/BLACKBOX)** is a Kafka-inspired message broker built from scratch in Java: persistent partition logs, topics, producers, consumer groups with committed offsets, and a JSON-over-TCP protocol.

```mermaid
flowchart LR
    P1[Producer] -->|JSON over TCP| B
    P2[Producer] -->|JSON over TCP| B

    subgraph B[BLACKBOX Broker]
        direction TB
        T[Topic Manager] --> L0[(Partition 0 Log)]
        T --> L1[(Partition 1 Log)]
        T --> L2[(Partition 2 Log)]

        GM[Consumer Group Manager]
        GM --> PA[Partition Assignment / Rebalancing]
    end

    L0 --> C1[Consumer 1]
    L1 --> C2[Consumer 2]
    L2 --> C1

    C1 --> CG[Consumer Group]
    C2 --> CG
    CG --> O[Persistent Committed Offsets]
```

---

## 💼 Experience

| Role | Company | When | Stack | Highlights |
|---|---|---|---|---|
| Product Engineer Intern | **Allstate India** | Feb – Jul 2026 | Java, Spring Boot, React | Full-stack product engineering |
| Software Engineering Intern | **ThriveStack.ai** | Sep – Dec 2025 | Go, gRPC, GraphQL, ClickHouse | **42%** query performance improvement |
| Backend Engineer Intern | **GoQuant** | Jun – Sep 2025 | FastAPI, OEMS backend, FIX protocol | Trading-system backend work |

---

## 🧰 Tech

<p>
  <img src="https://skillicons.dev/icons?i=cpp,java,py,go,js,spring,fastapi,react,graphql,postgres,mysql,docker,linux,git&theme=dark" />
</p>
<p>
  <img src="https://img.shields.io/badge/ClickHouse-121413?style=flat-square&logo=clickhouse&logoColor=c6f432" />
  <img src="https://img.shields.io/badge/FIX%20Protocol-121413?style=flat-square&logoColor=c6f432" />
</p>

---

## 📊 GitHub stats

<p align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=swamil-5504&show_icons=true&hide_border=true&bg_color=121413&title_color=c6f432&icon_color=c6f432&text_color=e9ece8&rank_icon=github&include_all_commits=true&count_private=true" />
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=swamil-5504&layout=donut-vertical&hide_border=true&bg_color=121413&title_color=c6f432&text_color=e9ece8" />
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=swamil-5504&hide_border=true&background=121413&ring=c6f432&fire=c6f432&currStreakLabel=c6f432&sideLabels=e9ece8&currStreakNum=e9ece8&sideNums=e9ece8&dates=98a09a" />
</p>

<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=swamil-5504&theme=matrix&no-frame=true&no-bg=true&row=1&column=7&margin-w=10" />
</p>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=swamil-5504&bg_color=121413&color=e9ece8&line=c6f432&point=ffffff&area=true&hide_border=true" width="100%" />

---

## 📫 Contact

<p align="center">
  <a href="https://www.linkedin.com/in/swamil-randive-00070a246/"><img src="https://img.shields.io/badge/LinkedIn-121413?style=for-the-badge&logo=linkedin&logoColor=c6f432" /></a>
  <a href="mailto:swamilrandive47@gmail.com"><img src="https://img.shields.io/badge/Email-121413?style=for-the-badge&logo=gmail&logoColor=c6f432" /></a>
  <a href="https://github.com/swamil-5504"><img src="https://img.shields.io/badge/GitHub-121413?style=for-the-badge&logo=github&logoColor=c6f432" /></a>
</p>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:121413,100:c6f432&height=100&section=footer" width="100%" />
