## `$ whoami`

AI-native Backend engineer (Java / Spring Boot) based in the Netherlands, previously a molecular biologist. Research taught me to design careful experiments and not trust a result until I've checked it; I now bring that to APIs, data models, and testing.


---

## `$ cat focus.txt`

- 🏗️ **Backend**: Java/Spring Boot services, PostgreSQL schema design and migrations, REST APIs, auth
- 🔭 **Reliability**: testing with real databases (Testcontainers), tracing and metrics (OpenTelemetry, Grafana)
- 🤖 **Spec-driven work with AI agents**: I own the architecture, write the specs and acceptance criteria, and review every change; agents implement inside hard gates and never merge

---

## `$ ls stack/`

![Java](https://img.shields.io/badge/Java-1a1a2e?style=flat-square&logo=openjdk&logoColor=e94560)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-1a1a2e?style=flat-square&logo=springboot&logoColor=e94560)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-1a1a2e?style=flat-square&logo=postgresql&logoColor=e94560)
![Flyway](https://img.shields.io/badge/Flyway-1a1a2e?style=flat-square&logo=flyway&logoColor=e94560)
![JUnit](https://img.shields.io/badge/JUnit-1a1a2e?style=flat-square&logo=junit5&logoColor=e94560)
![Testcontainers](https://img.shields.io/badge/Testcontainers-1a1a2e?style=flat-square&logo=docker&logoColor=e94560)
![Maven](https://img.shields.io/badge/Maven-1a1a2e?style=flat-square&logo=apachemaven&logoColor=e94560)
![Docker](https://img.shields.io/badge/Docker-1a1a2e?style=flat-square&logo=docker&logoColor=e94560)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-1a1a2e?style=flat-square&logo=githubactions&logoColor=e94560)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-1a1a2e?style=flat-square&logo=opentelemetry&logoColor=e94560)
![Grafana](https://img.shields.io/badge/Grafana-1a1a2e?style=flat-square&logo=grafana&logoColor=e94560)
![Python](https://img.shields.io/badge/Python-1a1a2e?style=flat-square&logo=python&logoColor=e94560)
![FastAPI](https://img.shields.io/badge/FastAPI-1a1a2e?style=flat-square&logo=fastapi&logoColor=e94560)
![React](https://img.shields.io/badge/React-1a1a2e?style=flat-square&logo=react&logoColor=e94560)
![TypeScript](https://img.shields.io/badge/TypeScript-1a1a2e?style=flat-square&logo=typescript&logoColor=e94560)
![OpenAPI](https://img.shields.io/badge/OpenAPI-1a1a2e?style=flat-square&logo=swagger&logoColor=e94560)

---

## `$ cat projects.md`

### 🔬 JobMatch → Microservices *(in progress)*
Splitting the JobMatch monolith into Spring Boot services behind a gateway with RS256 JWT, traced with OpenTelemetry. Next phase: SQS events with a transactional outbox for GDPR-safe deletion across services. I own the architecture and the day-by-day specs; AI agents implement and I review every PR. Decisions I'm proud of:
- A/B-tested the OpenTelemetry Java agent against the running stack and removed it after it suppressed Spring's HTTP instrumentation
- Fixed flaky CI by moving Maven dependencies into their own cached Docker layer

→ [Progress dashboard](https://yusuprozimemet.github.io/jobmatch-microservices/) · [Repo](https://github.com/yusuprozimemet/jobmatch-microservices)

### 🎧 LearnX-CLI + DevLoop
<!-- VERIFY before publishing: sandbox, review pipeline, and any numbers you add -->
A CLI that turns Markdown notes into audio and video lessons (Python). The same repo is my testbed for spec-driven, multi-agent development: agents implement inside a Docker sandbox, a separate multi-agent review pipeline checks every change, and nothing merges without passing tests and my review.
→ [Repo](https://github.com/Yusuprozimemet/LearnX-CLI)


---

## `$ cat workflow.md`

Every feature starts as a written spec with the deliverable, acceptance criteria and files touched. An agent implements on a branch; tests, lint and an AI review run; then I read the diff and decide whether it merges.

<!-- VERIFY: keep only the rules your repos actually enforce -->
- **No agent grades its own work**: the reviewing agent is never the one that wrote the change
- **Small PRs**: changes are kept within a size limit so every diff is reviewable
- **Hard gates**: branch protection on `main`; nothing lands without passing tests, and only a human merges

```
spec → branch → implement → test → AI review → human review & merge
```

---

## `$ cat publication.bib`

Vincenzetti S, **Rozimemet Y**, et al. *NAD Metabolism and Proteomic Profile in a Yeast Model Expressing a Neurotoxic polyQ Protein.* [Preprints.org, 2024](https://www.preprints.org/manuscript/202402.1499)

Outside code: chess, and learning Dutch.
