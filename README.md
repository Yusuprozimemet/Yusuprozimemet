<!-- Header typing animation -->
[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=22&pause=1000&color=E94560&background=00000000&center=false&vCenter=true&width=600&lines=mol.+biologist+%E2%86%92+backend+%2B+AI+engineer;spec-driven+//+multi-agent+//+human-merged)](https://git.io/typing-svg)

## `$ whoami`

Backend and AI engineer, formerly a molecular biologist (RNA splicing, spliceosome mechanics). Biology taught me to reason about complex systems; I now apply that to software architecture, data flow, and building reliable workflows around AI agents.

I learn by building, so there is always a project in progress, from small tools to full SaaS.

Based in the Netherlands 🇳🇱 · Currently completing HackYourFuture's Java & Spring Boot track

---

## `$ cat focus.txt`

- 🤖 **Agentic engineering**: multi-agent systems, LLM pipelines, and review setups where no agent grades its own work
- 🏗️ **Backend development**: Java/Spring Boot, Python/FastAPI, Node.js, PostgreSQL
- 🧬 **Computational biology**: where it all started
- ♟️ **Chess**: I enjoy building my own strategic frameworks

---

## `$ ls stack/`

![Java](https://img.shields.io/badge/Java-1a1a2e?style=flat-square&logo=openjdk&logoColor=e94560)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-1a1a2e?style=flat-square&logo=springboot&logoColor=e94560)
![Python](https://img.shields.io/badge/Python-1a1a2e?style=flat-square&logo=python&logoColor=e94560)
![FastAPI](https://img.shields.io/badge/FastAPI-1a1a2e?style=flat-square&logo=fastapi&logoColor=e94560)
![JavaScript](https://img.shields.io/badge/JavaScript-1a1a2e?style=flat-square&logo=javascript&logoColor=e94560)
![Node.js](https://img.shields.io/badge/Node.js-1a1a2e?style=flat-square&logo=node.js&logoColor=e94560)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-1a1a2e?style=flat-square&logo=postgresql&logoColor=e94560)
![Docker](https://img.shields.io/badge/Docker-1a1a2e?style=flat-square&logo=docker&logoColor=e94560)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-1a1a2e?style=flat-square&logo=githubactions&logoColor=e94560)
![Railway](https://img.shields.io/badge/Railway-1a1a2e?style=flat-square&logo=railway&logoColor=e94560)
![JUnit](https://img.shields.io/badge/JUnit-1a1a2e?style=flat-square&logo=junit5&logoColor=e94560)
![Playwright](https://img.shields.io/badge/Playwright-1a1a2e?style=flat-square&logo=playwright&logoColor=e94560)
![Maven](https://img.shields.io/badge/Maven-1a1a2e?style=flat-square&logo=apachemaven&logoColor=e94560)
![OpenAPI](https://img.shields.io/badge/OpenAPI-1a1a2e?style=flat-square&logo=swagger&logoColor=e94560)
![Postman](https://img.shields.io/badge/Postman-1a1a2e?style=flat-square&logo=postman&logoColor=e94560)
![Git](https://img.shields.io/badge/Git-1a1a2e?style=flat-square&logo=git&logoColor=e94560)
![Claude Code](https://img.shields.io/badge/Claude_Code-1a1a2e?style=flat-square&logo=claude&logoColor=e94560)

---

## `$ cat projects.md`

### 🔬 JobMatch → Microservices *(in progress)*

Migrating a Java monolith to microservices, one day and one PR at a time, with separated roles and limited permissions:

```
spec (Opus) → audit (read-only) → implement (Haiku) → break-it test → review (Opus) → human merge
     ↑                                                                                        ↓
     └───────────────────────────── next PR, never skip steps ──────────────────────────────┘
```

- **Opus** writes specs and reviews diffs
- **Read-only auditors** try to break every claim in the plan and spec before work starts
- **Haiku** writes code from a precise brief and never commits
- **Break-it test:** every change deliberately breaks the code first to prove the new test can fail
- **Human (me)** owns the merge button

→ [Progress dashboard](https://yusuprozimemet.github.io/jobmatch-microservices/) · [Repo](https://github.com/yusuprozimemet/jobmatch-microservices) · [Writing on Medium](https://medium.com/@yusupr)


### 🎧 LearnX-CLI

A `.md → LLM curriculum → TTS audio → MP4 video` pipeline, built spec by spec from v0 to v4, with 235 tests and a Docker sandbox in place of branch-only isolation.

→ [Repo](https://github.com/Yusuprozimemet/LearnX-CLI)

---

## `$ cat workflow.md`

### Spec-driven development

Every feature starts as a written spec: the exact deliverable, acceptance criteria, files touched, and exit conditions. The agent implements against the spec, and a human reviews the diff and merges only when every gate passes.

```
spec → branch → implement → test → multi-agent review → human merge
         ↑                                                    ↓
         └──────────────── never skip steps ─────────────────┘
```


**Hard rules**
- `NEVER` commit to main directly
- `NEVER` start the next spec until the current one is merged and green
- `NEVER` let an agent merge; a human does that after review
- `NEVER` skip the gate: unit tests + E2E + lint

---

## `$ cat publication.bib`

> **NAD Metabolism and Proteomic Profile in a Yeast Model Expressing a Neurotoxic polyQ Protein: Effect of Phenolics from Extra-virgin Olive Oil**
> Vincenzetti S, **Rozimemet Y**, et al. [preprints.org, 2024 →](https://www.preprints.org/manuscript/202402.1499)

---
