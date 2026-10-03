## `$ whoami`

AI-native backend engineer (Java / Spring Boot) based in the Netherlands, previously a molecular biologist. Research taught me to design careful experiments and not trust a result until I've checked it; I now bring that to APIs, data models, and testing.

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
Migrating the JobMatch monolith to Spring Boot services, one day spec at a time. So far: a gateway with RS256 JWT auth, job search and matching extracted into their own containers (job-service on its own PostgreSQL database, matching-service on DynamoDB), service-to-service tokens, and OpenTelemetry traces across every hop. Now in progress: GDPR-safe account deletion, where a transactional outbox publishes `user.deleted` over SNS/SQS and each service deletes its own data. I own the architecture and the specs; AI agents implement and I review every PR. Decisions I'm proud of:
- A/B-tested the OpenTelemetry Java agent against the running stack and removed it after it suppressed Spring's HTTP instrumentation
- Fixed flaky CI by moving Maven dependencies into their own cached Docker layer

→ [Progress dashboard](https://yusuprozimemet.github.io/jobmatch-microservices/) · [Repo](https://github.com/yusuprozimemet/jobmatch-microservices)

### 🎧 LearnX-CLI
Turns Markdown notes into an LLM-written curriculum, TTS audio and MP4 video (Python). My first spec-driven project: built spec by spec from v0 to v4, with 235 tests and a Docker sandbox for the agent.
→ [Repo](https://github.com/Yusuprozimemet/LearnX-CLI)

---

## `$ cat workflow.md`

**No code without a spec. No spec without checkable acceptance criteria.**

Each spec names the goal, what's in and out of scope, the tracks, the acceptance criteria, and a `Verify` command anyone can run. In [jobmatch-microservices](https://github.com/Yusuprozimemet/jobmatch-microservices) the roles are split so no agent grades its own work:

- **Me**: the plan, the specs, review of every diff, and every merge
- **Auditors** (read-only, fresh context): check each spec against the plan and the code before work starts; fixes land in a spec-change PR first
- **Main session** (Claude Opus): writes each track's brief, reviews the code, breaks it on purpose to prove the tests can fail, opens the PR
- **Implementer** (Claude Haiku): writes code from the brief and never commits

Enforced by CI, not good intentions: PRs over 400 changed lines fail, the PR template is required, and tests, lint and build must be green, all required by branch protection on `main`.

```
spec → audit → brief → implement → review & break on purpose → CI gates → human merge
```


---

## `$ cat publication.bib`

Vincenzetti S, **Rozimemet Y**, et al. *NAD Metabolism and Proteomic Profile in a Yeast Model Expressing a Neurotoxic polyQ Protein.* [Preprints.org, 2024](https://www.preprints.org/manuscript/202402.1499)

Outside code: chess, and learning Dutch.
