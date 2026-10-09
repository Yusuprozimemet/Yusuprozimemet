## `$ whoami`

AI-native software developer in the Netherlands, formerly a molecular biologist. I'm not new to code: during my MSc and PhD I did data analysis, machine learning and deep learning in Python. Since October 2023 I've been building apps, mostly self-taught, learning each tool by shipping something real with it. In February 2026 I joined the HackYourFuture backend track to learn Java and Spring Boot systematically and to professional standards.

---

## `$ git log`

My first app was [TyporaX](https://github.com/Yusuprozimemet/TyporaX), for learning Dutch. Then I built [Prakly](https://github.com/Yusuprozimemet/praklyai) solo, a B2B SaaS that turns company documents into AI lessons, in the Delitelab entrepreneurship programme with intensive mentorship. Alongside the HackYourFuture backend track I've built side projects in Python, FastAPI, React and LLMs: [friendmap](https://github.com/Yusuprozimemet/friendmap), [LearnX-Radar](https://github.com/Yusuprozimemet/LearnX-Radar) and [LearnX-CLI](https://github.com/Yusuprozimemet/LearnX-CLI). Then I built JobMatch with a team of six, and now I'm turning it into microservices with AI agents, as an experiment in agentic development run like a lab study: a spec with checkable criteria for every step, and every mistake recorded and counted. Along the way I'm learning distributed systems and AWS (Terraform, ECS on Fargate).

---

## `$ ls stack/`

![Java](https://img.shields.io/badge/Java-1a1a2e?style=flat-square&logo=openjdk&logoColor=e94560)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-1a1a2e?style=flat-square&logo=springboot&logoColor=e94560)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-1a1a2e?style=flat-square&logo=postgresql&logoColor=e94560)
![Flyway](https://img.shields.io/badge/Flyway-1a1a2e?style=flat-square&logo=flyway&logoColor=e94560)
![Maven](https://img.shields.io/badge/Maven-1a1a2e?style=flat-square&logo=apachemaven&logoColor=e94560)
![OpenAPI](https://img.shields.io/badge/OpenAPI-1a1a2e?style=flat-square&logo=swagger&logoColor=e94560)
![JUnit](https://img.shields.io/badge/JUnit-1a1a2e?style=flat-square&logo=junit5&logoColor=e94560)
![Testcontainers](https://img.shields.io/badge/Testcontainers-1a1a2e?style=flat-square&logo=docker&logoColor=e94560)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-1a1a2e?style=flat-square&logo=opentelemetry&logoColor=e94560)
![Grafana](https://img.shields.io/badge/Grafana-1a1a2e?style=flat-square&logo=grafana&logoColor=e94560)
![Docker](https://img.shields.io/badge/Docker-1a1a2e?style=flat-square&logo=docker&logoColor=e94560)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-1a1a2e?style=flat-square&logo=githubactions&logoColor=e94560)
![AWS](https://img.shields.io/badge/AWS-1a1a2e?style=flat-square&logo=amazonwebservices&logoColor=e94560)
![Terraform](https://img.shields.io/badge/Terraform-1a1a2e?style=flat-square&logo=terraform&logoColor=e94560)
![DynamoDB](https://img.shields.io/badge/DynamoDB-1a1a2e?style=flat-square&logo=amazondynamodb&logoColor=e94560)
![Python](https://img.shields.io/badge/Python-1a1a2e?style=flat-square&logo=python&logoColor=e94560)
![FastAPI](https://img.shields.io/badge/FastAPI-1a1a2e?style=flat-square&logo=fastapi&logoColor=e94560)
![React](https://img.shields.io/badge/React-1a1a2e?style=flat-square&logo=react&logoColor=e94560)
![TypeScript](https://img.shields.io/badge/TypeScript-1a1a2e?style=flat-square&logo=typescript&logoColor=e94560)

---

## `$ cat projects.md`

### 🧩 JobMatch: HackYourFuture final project
A job-search platform built by six developers in agile sprints. My part: Google sign-in, account deletion, the profile API and the matching engine.
→ [Live demo](https://c55c.hyf.dev/) · [Repo](https://github.com/HackYourFutureProjects/c55-final-project-group-C)

### 🔬 JobMatch → Microservices: an experiment in agentic development *(in progress)*
I split that monolith into five services with AI agents, one spec at a time. 340+ PRs so far, and every finding is recorded, including the ones that make the method look bad:
- The agents' mistakes far outnumber the system's: 382 of 401 recorded defects were in the agents' own specs and code, caught by auditor agents, review or tests broken on purpose.
- A smaller model writes the code from my briefs. Review found a defect in 30 of the 63 tracks it wrote before they merged.
- The tests written before the split survived it with two approved edits.

Next: deploying to AWS with Terraform.
→ [Dashboard](https://yusuprozimemet.github.io/jobmatch-microservices/) · [Lab notebook](https://github.com/Yusuprozimemet/jobmatch-microservices/blob/main/docs/lab-notebook.md) · [Repo](https://github.com/yusuprozimemet/jobmatch-microservices)

---

## `$ cat workflow.md`

**No code without a spec. No spec without checkable acceptance criteria.**

- **Me:** the plan, the specs, review of every change, and every merge
- **AI agents:** audit the specs, write the code, and break it on purpose to prove the tests can catch it; they never merge
- **CI:** tests, lint and a 400-line PR limit, all required before merging

```
spec → audit → implement → review → CI → human merge
```

Every mistake, mine and the agents', goes in a [lab notebook](https://github.com/Yusuprozimemet/jobmatch-microservices/blob/main/docs/lab-notebook.md).

---

## `$ cat publication.bib`

Vincenzetti S, **Rozimemet Y**, et al. *NAD Metabolism and Proteomic Profile in a Yeast Model Expressing a Neurotoxic polyQ Protein.* [Preprints.org, 2024](https://www.preprints.org/manuscript/202402.1499)

**Languages:** Uyghur, Chinese, English, Dutch (learning) · **Outside code:** chess, cycling, traveling
