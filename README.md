<div align="center">

                                                  ```
                                                    ░██████╗██╗░░░██╗███╗░░░███╗██╗████████╗
                                                    ██╔════╝██║░░░██║████╗░████║██║╚══██╔══╝
                                                    ╚█████╗░██║░░░██║██╔████╔██║██║░░░██║░░░
                                                   ░ ╚═══██╗██║░░░██║██║╚██╔╝██║██║░░░██║░░░
                                                    ██████╔╝╚██████╔╝██║░╚═╝░██║██║░░░██║░░░
                                                   ╚═════╝░░╚═════╝░╚═╝░░░░░╚═╝╚═╝░░░╚═╝░░░
                                                  ```

### Sumit Kumar Gupta
**Backend Engineer · Distributed Systems · AI Integrator**

*I don't just use frameworks — I build what frameworks are built on.*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/sumit-kumar-gupta-9b4970285/)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sumit.gupta.14486@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/sumit-kumar-guptaa)
[![Profile Views](https://komarev.com/ghpvc/?username=sumit-kumar-guptaa&style=for-the-badge&color=blueviolet)](https://github.com/sumit-kumar-guptaa)

</div>

---

## `$ whoami`

```yaml
name    : Sumit Kumar Gupta
role    : Backend Developer (Fresher · Final Year)
degree  : B.Tech CSE — 4th Year, 7th Semester

core_strengths:
  - Distributed Systems & Event-Driven Architecture
  - JVM Internals, Concurrency, Thread Modeling
  - Cloud Infra on AWS (Deployed. Not just configured.)
  - AI/LLM Integration — RAG, MCP, Agents

currently:
  - Solving Blind 75 + LC 150 with full understanding
  - Building systems that benchmark, not just compile

belief: "If I can't explain why the thread pool won — I don't understand it yet."
```

---

## `$ cat tech_stack.json`

**Core Backend**

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white)
![Spring](https://img.shields.io/badge/Spring-6DB33F?style=flat-square&logo=spring&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

**Messaging & Caching**

![Apache Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=flat-square&logo=apache-kafka&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)

**Cloud & DevOps**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazon-aws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)

**Testing**

![JUnit](https://img.shields.io/badge/JUnit5-25A162?style=flat-square&logo=junit5&logoColor=white)

**Frontend & Realtime**

![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![React Native](https://img.shields.io/badge/React_Native-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Socket.io](https://img.shields.io/badge/Socket.io-010101?style=flat-square&logo=socket.io&logoColor=white)

**AI / ML Stack**

![RAG](https://img.shields.io/badge/RAG_Pipeline-412991?style=flat-square&logo=openai&logoColor=white)
![MCP](https://img.shields.io/badge/MCP_Protocol-blueviolet?style=flat-square)
![LLMs](https://img.shields.io/badge/LLM_Integration-FF6F00?style=flat-square)

**Currently Exploring**

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)

---

## `$ ls -la projects/`

---

### ⚙️ [Custom HTTP Web Server](https://github.com/sumit-kumar-guptaa)
> *Built HTTP from scratch. Then benchmarked it to 600K requests.*

```
Stack : Core Java · JUnit · Single Thread · Multi Thread · Thread Pool
Tests : JUnit-based load simulation with concurrent request spawning
```

This isn't a "hello world" server. It's a full concurrency study:

| Model | Requests Handled | Notes |
|---|---|---|
| Single Threaded | Limited | Baseline — blocks on each connection |
| Multi Threaded | Moderate | One thread per request — high overhead |
| **Thread Pool** | **~600,000** | **Winner — bounded threads, max throughput** |

- Implemented raw **HTTP/1.1 request parsing** — method, path, headers, body
- Custom **routing layer** and response builder without any framework
- **JUnit test suite** that spawns concurrent requests to simulate real load
- Benchmarks documented with results — not just "it works", but *why* Thread Pool wins

> 💡 *The point wasn't to build another server. It was to understand what Tomcat, Netty, and every web framework has already figured out — and prove it with numbers.*

---

### 💸 [Live Expense Tracker](https://github.com/sumit-kumar-guptaa)
> *Distributed financial system. Deployed. Dockerized. CI/CD wired.*

```
Stack : Spring Boot · React Native · Kafka · Redis · RabbitMQ
Cloud : AWS (Elastic Beanstalk + Lightsail) · Docker · GitHub Actions
Arch  : Microservices · Event-Driven · Async Processing
```

- **Kafka** as the event backbone — every transaction is a stream event, not a direct DB write
- **Redis** caching layer for balance reads — hot data never hits the DB
- **RabbitMQ** handles async workers — notifications, summaries, background jobs fully decoupled
- **Dockerized** services with proper `docker-compose` for local dev parity
- **CI/CD via GitHub Actions** — push to main → build → test → deploy to AWS automatically
- Architecture diagrams and service communication flow documented in the repo

---

### 🔗 [PeerLink — P2P File Sharing](https://github.com/sumit-kumar-guptaa)
> *Peer-to-peer file transfer. Core Java. No shortcuts.*

```
Stack : Core Java · Sockets · IOUtils · Handlers
Cloud : AWS LightSail · Nginx (Reverse Proxy) · Docker
```

- Zero frameworks — raw **Java socket programming**, custom protocol, byte-level I/O
- Multi-threaded **connection handlers** managing simultaneous peer sessions
- **IOUtils** for efficient stream management during file transfer
- **Deployed on AWS LightSail** — not just localhost, actual production server
- **Nginx** configured as reverse proxy — TLS termination, port forwarding, traffic routing
- The project that taught what every framework abstracts away

---

### 🧠 [MediMax](https://github.com/IAteNoodles/MediMax) · [MedAssist](https://github.com/IAteNoodles/MedAssist) · [Nirpeksh](https://github.com/IAteNoodles/Nirpeksh)
> Multi-agent healthcare AI · Clinical LLM chatbot · Dataset bias detection

```
Stack : Python · RAG · LLMs · Multi-Agent Orchestration · MCP
```

---

## `$ systemctl status skills`

```
● Core Java & JVM Concurrency       [●●●●●] PRODUCTION-READY
● Spring Boot / Spring Framework    [●●●●●] PRODUCTION-READY
● Distributed Systems (Kafka/MQ)    [●●●●○] DEPLOYED
● AWS Cloud Infrastructure          [●●●●○] DEPLOYED
● Docker & CI/CD Pipelines          [●●●●○] DEPLOYED
● Nginx & Reverse Proxy             [●●●●○] DEPLOYED
● LLM / RAG / MCP Integration       [●●●●○] ACTIVE
● DSA (Blind 75 + LC 150)           [●●●○○] IN PROGRESS
● Rust                              [●●○○○] LEARNING
```

---

## `$ git log --graph --stat`

<p align="center">
  <img src="https://github-stats-brown-nu.vercel.app/api?username=sumit-kumar-guptaa&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&include_all_commits=true" height="160" />
  <img src="https://github-readme-streak-stats-delta-gray.vercel.app/?user=sumit-kumar-guptaa&theme=tokyonight&hide_border=true" height="160" />
</p>

<p align="center">
  <img src="https://github-stats-brown-nu.vercel.app/api/top-langs/?username=sumit-kumar-guptaa&theme=tokyonight&hide_border=true&layout=compact&langs_count=8" height="150"/>
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=sumit-kumar-guptaa&theme=tokyo-night&hide_border=true&hide_title=true&area=true" height="200" />
</p>

---

<p align="center">
  <img src="https://raw.githubusercontent.com/sumit-kumar-guptaa/sumit-kumar-guptaa/output/github-contribution-grid-snake-dark.svg" alt="Contribution Snake"/>
</p>

---

<div align="center">

```
Open to: Backend SDE roles · Distributed Systems · Platform/Infra · AI-integrated backend
```

*"Most people learn by reading docs. I learn by breaking things and reading the stack trace."*

**→ Let's build something that actually handles load.**

</div>
