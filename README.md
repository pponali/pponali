<h1 align="center">Hi 👋, I'm Prakash Ponali</h1>
<h3 align="center">Senior Software Engineer · AI Systems · AgriTech · Agentic Pipelines</h3>

<p align="left">
  <img src="https://komarev.com/ghpvc/?username=pponali&label=Profile%20views&color=0e75b6&style=flat" alt="pponali" />
</p>

<p align="left">
  <a href="https://github.com/pponali">
    <img src="https://github-profile-trophy.vercel.app/?username=pponali" alt="pponali" />
  </a>
</p>

<p align="left">
  <a href="https://twitter.com/ponali231" target="blank">
    <img src="https://img.shields.io/twitter/follow/ponali231?logo=twitter&style=for-the-badge" alt="ponali231" />
  </a>
</p>

---

## 🚀 Featured Projects

### 🌾 [Kheti Sahayak](https://khetisahayak.com) — AI-Powered AgriTech Platform
> Empowering 1M+ Indian farmers with AI diagnostics, hyperlocal weather, digital marketplace, and expert consultations.

**What it is:** Production SaaS platform for Indian smallholder farmers — crop disease detection via vision AI, real-time mandi prices, expert consultations, and a full digital marketplace.

**Architecture highlights:**
- **28 Spring Boot microservices** (100% parity migration from Node.js monolith) — auth, marketplace, crop, weather, diagnosis, notifications, payments, and more
- **162 AI agents** defined as Claude Code subagents — engineering, QA, product, DevOps, security, ML, marketing, executive roles — orchestrated via CrewAI crews and a Virtual Software Company pattern
- **Claude Code deeply integrated** — 162 `.claude/agents/` definitions with YAML frontmatter, hooks (SessionStart, UserPromptSubmit, PreToolUse, PostToolUse, Stop), GPS MCP server for symbol graph indexing, Render MCP for deployments
- **Multi-model AI stack:** `claude-sonnet-4-6` (default), `claude-opus-4-8` (high-reasoning CFO/CTO roles), `claude-haiku-4-5` (lightweight ops), Cerebras (inference), Groq (audio transcription), Gemini
- **LLaVA vision model** — local CPU inference for crop disease detection across 38 PlantVillage classes, with 2000+ lines of India-specific treatment database (Hindi/English/Telugu/Marathi)
- **Multi-tenant SaaS** — PostgreSQL schema isolation per tenant, X-Tenant-Id header enforcement, row-level security
- **Observability:** ELK Stack, Prometheus + Grafana, Spring Sleuth + Zipkin, Sentry
- **Event streaming:** Kafka 3.7, Redis 7, PostgreSQL 14 + pgvector

**Agent-driven SDLC — 110+ workflows covering the full engineering lifecycle:**

| Phase | What's automated |
|---|---|
| **Planning** | 20 parity audit plans (auth → marketplace → weather → finance → profile), sprint backlog, PRD templates, architecture diagrams, UI specs |
| **Development** | 9 agent-chain workflow types (WF-1 new feature → WF-9 backend bug fix) — each dispatches multi-role chains: Product Manager → Architect → Backend Dev → Mobile Dev → QA → Security Engineer |
| **Testing** | Full-app emulator QA sweep: 7 sequential runtime agents + 16 parallel static auditors → P0/P1/P2/P3 defect triage → parallel fan-out fix dispatch per defect group |
| **Deployment** | Module-aware deploy (WF-10/11/12): detect changed modules → Docker/Render/Vercel/Play Store → health verify → auto-rollback on failure |
| **Monitoring** | 24/7 L1→L2→L3 agent escalation hierarchy: health scan → triage → remediate → investigate → stabilize → incident command → post-mortem |
| **CI/CD** | 30 GitHub Actions: multi-stack CI (Node.js, Spring Boot, Flutter, Kotlin), AI-powered PR code review, CodeQL SAST, Firebase Test Lab on real devices, smoke tests on every production push |
| **Self-improvement** | Nightly agent improvement loop: harvest GPS corrections → triage by agent → mutate prompts below 7.5 threshold → commit; real-time auto-learn stores feedback instantly; GEPA-style eval loop scores agents across 5 dimensions |

**Workflow runner:** single `./workflow-runner.sh WF-N TASK-ID` dispatches full agent chain, logs every step to shared GitHub issue as paper trail.

**Stack:** Java 17 / Spring Boot 3.4 · Node.js 18 / Express 5 · Flutter 3 · React 19 + Vite · Python / FastAPI · PostgreSQL · Redis · Kafka · Docker / Kubernetes · Render · Vercel

---

### 🤖 [Job Search AI](https://github.com/pponali/job-search-api) — Agentic Job Discovery & Auto-Apply
> End-to-end agentic pipeline: discover → ATS-score → auto-apply across Naukri, LinkedIn, and Indeed.

**What it is:** Multi-tenant job-search platform that started as a single-admin Notion CLI tool and grew into a full SaaS layer with magic-link auth, per-user quota tiers, an LLM tailor pipeline, a chat agent, and a React frontend — all in one Express process.

**Agentic highlights:**
- **Claude Code subagent fleet** — 15 specialized agents per portal (session-manager, job-discoverer, job-scorer, cover-letter-writer, apply-bot, pipeline-orchestrator) across Naukri / LinkedIn / Indeed
- **Auto-discover → ATS-score → auto-apply pipeline** — Playwright-driven headless apply with stealth mode, session persistence, and smart form-fill via ApplyAgent
- **11-step LLM tailor pipeline** — JD Analysis → Keywords → Company Research → Resume Match → Skill Gap → Rewrite Bullets → Cover Letter → Interview Qs → Recruiter Outreach → Critic → Revision → Finalize; hybrid ATS scoring with automatic revision loop
- **Chat agent** — router → specialist delegation (discovery / scoring / tailor / apply / resumes / schedule) over Anthropic SDK, tool-use loops, capped at depth 4
- **Self-improving apply agent** — learns from outcomes; persists qa_cache, selector_drift, portal_overrides, outcomes.jsonl
- **SSE streaming** for long-running operations; SQLite (better-sqlite3, WAL mode) for both app and pipeline state

**Stack:** Node.js 18 / Express · React 18 + Vite + TypeScript · Python / Playwright + playwright-stealth · SQLite · Anthropic SDK · JobSpy · Resend · Razorpay

---

## 🧠 What I'm Working On

- 🔭 **Kheti Sahayak** — scaling to 1M+ farmers, completing microservices migration, adding pgvector RAG
- 🤖 **Agentic systems** — Claude Code multi-agent orchestration, CrewAI crews, self-improving bots
- 🌱 **Spring Boot 3.4 + Kafka** microservices architecture at production scale

---

## 💬 Ask Me About

Java · Spring Boot · Node.js · Microservices · Claude Code & Agentic AI · Playwright automation · Multi-tenant SaaS · PostgreSQL · Kafka · Docker/Kubernetes

---

## 📫 Reach Me

**Email:** p.ponali@yahoo.com  
**Blog:** [prakashponali.wordpress.com](https://prakashponali.wordpress.com/)

---

<h3 align="left">Connect with me:</h3>
<p align="left">
<a href="https://codepen.io/pponali" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/codepen.svg" alt="pponali" height="30" width="40" /></a>
<a href="https://dev.to/pponali" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/devto.svg" alt="pponali" height="30" width="40" /></a>
<a href="https://twitter.com/ponali231" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/twitter.svg" alt="ponali231" height="30" width="40" /></a>
<a href="https://linkedin.com/in/prakashponali" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="prakashponali" height="30" width="40" /></a>
<a href="https://stackoverflow.com/users/pponali" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/stack-overflow.svg" alt="pponali" height="30" width="40" /></a>
<a href="https://kaggle.com/pponali" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/kaggle.svg" alt="pponali" height="30" width="40" /></a>
<a href="https://medium.com/pponali" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/medium.svg" alt="pponali" height="30" width="40" /></a>
<a href="https://www.youtube.com/c/pponali" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/youtube.svg" alt="pponali" height="30" width="40" /></a>
<a href="https://www.leetcode.com/pponali" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/leet-code.svg" alt="pponali" height="30" width="40" /></a>
<a href="https://discord.gg/pponali" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/discord.svg" alt="pponali" height="30" width="40" /></a>
</p>

<h3 align="left">Languages and Tools:</h3>
<p align="left">
<a href="https://aws.amazon.com" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/amazonwebservices/amazonwebservices-original-wordmark.svg" alt="aws" width="40" height="40"/></a>
<a href="https://azure.microsoft.com/en-in/" target="_blank" rel="noreferrer"><img src="https://www.vectorlogo.zone/logos/microsoft_azure/microsoft_azure-icon.svg" alt="azure" width="40" height="40"/></a>
<a href="https://www.docker.com/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original-wordmark.svg" alt="docker" width="40" height="40"/></a>
<a href="https://www.elastic.co" target="_blank" rel="noreferrer"><img src="https://www.vectorlogo.zone/logos/elastic/elastic-icon.svg" alt="elasticsearch" width="40" height="40"/></a>
<a href="https://firebase.google.com/" target="_blank" rel="noreferrer"><img src="https://www.vectorlogo.zone/logos/firebase/firebase-icon.svg" alt="firebase" width="40" height="40"/></a>
<a href="https://cloud.google.com" target="_blank" rel="noreferrer"><img src="https://www.vectorlogo.zone/logos/google_cloud/google_cloud-icon.svg" alt="gcp" width="40" height="40"/></a>
<a href="https://git-scm.com/" target="_blank" rel="noreferrer"><img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="40" height="40"/></a>
<a href="https://grafana.com" target="_blank" rel="noreferrer"><img src="https://www.vectorlogo.zone/logos/grafana/grafana-icon.svg" alt="grafana" width="40" height="40"/></a>
<a href="https://graphql.org" target="_blank" rel="noreferrer"><img src="https://www.vectorlogo.zone/logos/graphql/graphql-icon.svg" alt="graphql" width="40" height="40"/></a>
<a href="https://www.java.com" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" alt="java" width="40" height="40"/></a>
<a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/></a>
<a href="https://kafka.apache.org/" target="_blank" rel="noreferrer"><img src="https://www.vectorlogo.zone/logos/apache_kafka/apache_kafka-icon.svg" alt="kafka" width="40" height="40"/></a>
<a href="https://kubernetes.io" target="_blank" rel="noreferrer"><img src="https://www.vectorlogo.zone/logos/kubernetes/kubernetes-icon.svg" alt="kubernetes" width="40" height="40"/></a>
<a href="https://www.linux.org/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="linux" width="40" height="40"/></a>
<a href="https://www.mongodb.com/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original-wordmark.svg" alt="mongodb" width="40" height="40"/></a>
<a href="https://nodejs.org" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original-wordmark.svg" alt="nodejs" width="40" height="40"/></a>
<a href="https://www.nginx.com" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nginx/nginx-original.svg" alt="nginx" width="40" height="40"/></a>
<a href="https://www.postgresql.org" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original-wordmark.svg" alt="postgresql" width="40" height="40"/></a>
<a href="https://www.python.org" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/></a>
<a href="https://reactjs.org/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="react" width="40" height="40"/></a>
<a href="https://redis.io" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/redis/redis-original-wordmark.svg" alt="redis" width="40" height="40"/></a>
<a href="https://spring.io/" target="_blank" rel="noreferrer"><img src="https://www.vectorlogo.zone/logos/springio/springio-icon.svg" alt="spring" width="40" height="40"/></a>
<a href="https://www.typescriptlang.org/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-original.svg" alt="typescript" width="40" height="40"/></a>
<a href="https://flutter.dev" target="_blank" rel="noreferrer"><img src="https://www.vectorlogo.zone/logos/flutterio/flutterio-icon.svg" alt="flutter" width="40" height="40"/></a>
<a href="https://www.tensorflow.org" target="_blank" rel="noreferrer"><img src="https://www.vectorlogo.zone/logos/tensorflow/tensorflow-icon.svg" alt="tensorflow" width="40" height="40"/></a>
<a href="https://pytorch.org/" target="_blank" rel="noreferrer"><img src="https://www.vectorlogo.zone/logos/pytorch/pytorch-icon.svg" alt="pytorch" width="40" height="40"/></a>
</p>

---

<p><img align="center" src="https://github-readme-stats.vercel.app/api/top-langs?username=pponali&show_icons=true&locale=en&layout=compact" alt="pponali" /></p>
<p>&nbsp;<img align="center" src="https://github-readme-stats.vercel.app/api?username=pponali&show_icons=true&locale=en" alt="pponali" /></p>
<p><img align="center" src="https://github-readme-streak-stats.herokuapp.com/?user=pponali&" alt="pponali" /></p>
