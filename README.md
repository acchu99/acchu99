<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:1f6feb&height=110&section=header" />
  <source media="(prefers-color-scheme: light)" srcset="https://capsule-render.vercel.app/api?type=waving&color=0:ffffff,100:0969da&height=110&section=header" />
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:ffffff,100:0969da&height=110&section=header" alt="Ashwin Balasubramanian" />
</picture>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=22&duration=2800&pause=900&color=58A6FF&center=true&vCenter=true&width=720&height=50&lines=Applied+AI+Engineer;ML+Engineer;Agentic+Development;Software+Architecture;Agents+%C2%B7+Prompts+%C2%B7+Infra;DL+tinkerer+by+habit;AI+builder+by+obsession" />
  <source media="(prefers-color-scheme: light)" srcset="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=22&duration=2800&pause=900&color=0969DA&center=true&vCenter=true&width=720&height=50&lines=Applied+AI+Engineer;ML+Engineer;Agentic+Development;Software+Architecture;Agents+%C2%B7+Prompts+%C2%B7+Infra;DL+tinkerer+by+habit;AI+builder+by+obsession" />
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=22&duration=2800&pause=900&color=0969DA&center=true&vCenter=true&width=720&height=50&lines=Applied+AI+Engineer;ML+Engineer;Agentic+Development;Software+Architecture;Agents+%C2%B7+Prompts+%C2%B7+Infra;DL+tinkerer+by+habit;AI+builder+by+obsession" alt="Applied AI Engineer, ML Engineer, Agentic Development, Software Architecture, Agents, Prompts, Infra" />
</picture>

# Hi, I'm Ashwin Balasubramanian

**Applied AI Engineer @ Vizly.ai | M.S. in CS from ASU | ML engineer by trade, DL tinkerer by habit, AI builder by obsession.**

[Vizly.ai](https://vizly.ai) · [Portfolio](https://www.ashwinbala.com/) · [LinkedIn](https://linkedin.com/in/ashwin1999) · [X](https://x.com/acchu99) · [GitHub](https://github.com/acchu99)

Southfield, MI · Remote

</div>

---

## About

I am an Applied AI Engineer at [Vizly.ai](https://vizly.ai). My work is agentic software development and architecting complex production software: prompt and agent behavior, backend services, and cloud infrastructure. I hold an M.S. in Computer Science from Arizona State University, and I build practical AI that improves quality, reduces cost, and solves real user problems.

---

## What I'm working on

- **MacroSense AI** (in progress, Feb 2026 – Present). Multi-tenant SaaS health platform with provider-agnostic AI routing, enterprise RBAC, Postgres RLS, and Langfuse observability. Fitbit OAuth 2.0 PKCE with encrypted token storage, resumable 90-day Inngest backfill workflows, cache-first food search, and privacy-focused data export and deletion.
- **Vizly.ai**. Agentic software development and systems architecture: I design the system, define service boundaries and contracts, and build with AI coding agents under engineering guardrails. The platform work includes prompt and agent behavior, a production MCP server with OAuth 2.0, enterprise prompt governance, and a JupyterHub re-architecture on Terraform and AWS.

---

## Building at Vizly

Vizly is an AI-assisted analytical workspace: users bring datasets, work in AI-assisted notebook threads, and produce dashboards, reports, and slide decks. It is multi-tenant, with subscription-aware usage controls. I work across five units that fit together as one platform.

| Unit | What it does | Stack |
| --- | --- | --- |
| Web application | Product front end and orchestrator for sessions, workspaces, notebook threads, dashboards, reports, and slides, including durable workers for offline reasoning, prompt guardrails, report and slide generation, and notifications. | TypeScript, Next.js, React, Supabase, Vercel AI SDK, Anthropic, OpenAI, Langfuse, OpenTelemetry, Sentry, Stripe, Playwright, Jest |
| MCP server | Production Model Context Protocol server that gives AI agents authenticated, authorized access to platform tools, skills, and datasets over HTTP/SSE. | Python, Starlette/Uvicorn, MCP SDK, Supabase, Docker, Kubernetes |
| Datasets service | Internal data engine for dataset access from notebooks and agents, plus an async enrichment pipeline that validates datasets and produces schema, statistics, and semantic summaries, with budget controls and retry/recovery. | Python, RPC, Supabase, S3, Kubernetes |
| JupyterHub runtime | Per-user, isolated Python analytical environments with a custom spawner, persistent storage, dedicated node groups, and autoscaling. | JupyterHub, Kubernetes (EKS), Helm, Terraform, Docker |
| Shared infrastructure | Cloud foundation for the platform: multi-AZ networking, EKS, load balancing, centralized observability, remote Terraform state, and dev, staging, and prod promotion through CI/CD. | AWS, Terraform, EKS, GitHub Actions |

The Next.js app on Vercel sits on Supabase for auth, data, and durable queues. It spawns user kernels in JupyterHub and gives agents context through the MCP server; both JupyterHub and the MCP server reach data through the Datasets service, container workers consume the queues, and everything on AWS runs on EKS provisioned by shared Terraform.

Agent-native engineering: architecture, guardrails, and review gates that let AI coding agents ship production changes safely. The repos carry agent guidance, reusable skills and workflows, dependency and ownership maps, evaluation suites, role-aware end-to-end tests, and human-approval gates for risky changes.

---

## Impact at a glance

| Result | Where it came from |
| --- | --- |
| −40% monthly cloud spend | Re-architected JupyterHub with Terraform and AWS |
| 257 ms execution latency | Maintained through that re-architecture |
| Zero downtime incidents | Maintained through that re-architecture |
| 12+ production and P0 issues | Billing, authentication, and agent response behavior |
| Production MCP server | OAuth 2.0 so agents can securely invoke data integrations |

---

## Tech stack

**Languages**

<p align="center"><img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-1D4ED8?style=flat-square&logo=typescript&logoColor=white" /> <img alt="Python" src="https://img.shields.io/badge/Python-1D4ED8?style=flat-square&logo=python&logoColor=white" /> <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-1D4ED8?style=flat-square&logo=javascript&logoColor=white" /> <img alt="SQL (Postgres)" src="https://img.shields.io/badge/SQL_(Postgres)-1D4ED8?style=flat-square&logo=postgresql&logoColor=white" /> <img alt="HTML/CSS" src="https://img.shields.io/badge/HTML%2FCSS-1D4ED8?style=flat-square" /> <img alt="Java" src="https://img.shields.io/badge/Java-1D4ED8?style=flat-square&logo=openjdk&logoColor=white" /> <img alt="R" src="https://img.shields.io/badge/R-1D4ED8?style=flat-square&logo=r&logoColor=white" /></p>

**Agentic AI & LLM**

<p align="center"><img alt="Agentic Development" src="https://img.shields.io/badge/Agentic_Development-6D28D9?style=flat-square" /> <img alt="Prompt Engineering" src="https://img.shields.io/badge/Prompt_Engineering-6D28D9?style=flat-square" /> <img alt="MCP (Model Context Protocol)" src="https://img.shields.io/badge/MCP_(Model_Context_Protocol)-6D28D9?style=flat-square" /> <img alt="Anthropic Claude" src="https://img.shields.io/badge/Anthropic_Claude-6D28D9?style=flat-square" /> <img alt="OpenAI" src="https://img.shields.io/badge/OpenAI-6D28D9?style=flat-square&logo=openai&logoColor=white" /> <img alt="Google Gemini" src="https://img.shields.io/badge/Google_Gemini-6D28D9?style=flat-square" /> <img alt="xAI Grok" src="https://img.shields.io/badge/xAI_Grok-6D28D9?style=flat-square" /> <img alt="Vercel AI SDK" src="https://img.shields.io/badge/Vercel_AI_SDK-6D28D9?style=flat-square&logo=vercel&logoColor=white" /> <img alt="LangChain" src="https://img.shields.io/badge/LangChain-6D28D9?style=flat-square" /> <img alt="RAG" src="https://img.shields.io/badge/RAG-6D28D9?style=flat-square" /> <img alt="Langfuse (LLM observability)" src="https://img.shields.io/badge/Langfuse_(LLM_observability)-6D28D9?style=flat-square" /></p>

**Frontend & Backend**

<p align="center"><img alt="Next.js" src="https://img.shields.io/badge/Next.js-0F766E?style=flat-square&logo=nextdotjs&logoColor=white" /> <img alt="React" src="https://img.shields.io/badge/React-0F766E?style=flat-square&logo=react&logoColor=white" /> <img alt="Node.js" src="https://img.shields.io/badge/Node.js-0F766E?style=flat-square&logo=nodedotjs&logoColor=white" /> <img alt="FastAPI" src="https://img.shields.io/badge/FastAPI-0F766E?style=flat-square&logo=fastapi&logoColor=white" /> <img alt="Flask" src="https://img.shields.io/badge/Flask-0F766E?style=flat-square&logo=flask&logoColor=white" /> <img alt="Starlette" src="https://img.shields.io/badge/Starlette-0F766E?style=flat-square" /></p>

**Data & Database**

<p align="center"><img alt="Supabase" src="https://img.shields.io/badge/Supabase-047857?style=flat-square&logo=supabase&logoColor=white" /> <img alt="PostgreSQL (RLS)" src="https://img.shields.io/badge/PostgreSQL_(RLS)-047857?style=flat-square&logo=postgresql&logoColor=white" /> <img alt="Pandas" src="https://img.shields.io/badge/Pandas-047857?style=flat-square&logo=pandas&logoColor=white" /> <img alt="NumPy" src="https://img.shields.io/badge/NumPy-047857?style=flat-square&logo=numpy&logoColor=white" /> <img alt="SciPy" src="https://img.shields.io/badge/SciPy-047857?style=flat-square&logo=scipy&logoColor=white" /></p>

**Cloud & DevOps**

<p align="center"><img alt="AWS" src="https://img.shields.io/badge/AWS-C2410C?style=flat-square&logo=amazonaws&logoColor=white" /> <img alt="Kubernetes (EKS)" src="https://img.shields.io/badge/Kubernetes_(EKS)-C2410C?style=flat-square&logo=kubernetes&logoColor=white" /> <img alt="Terraform" src="https://img.shields.io/badge/Terraform-C2410C?style=flat-square&logo=terraform&logoColor=white" /> <img alt="Helm" src="https://img.shields.io/badge/Helm-C2410C?style=flat-square&logo=helm&logoColor=white" /> <img alt="Docker" src="https://img.shields.io/badge/Docker-C2410C?style=flat-square&logo=docker&logoColor=white" /> <img alt="GitHub Actions (CI/CD)" src="https://img.shields.io/badge/GitHub_Actions_(CI%2FCD)-C2410C?style=flat-square&logo=githubactions&logoColor=white" /> <img alt="JupyterHub" src="https://img.shields.io/badge/JupyterHub-C2410C?style=flat-square" /> <img alt="Vercel" src="https://img.shields.io/badge/Vercel-C2410C?style=flat-square&logo=vercel&logoColor=white" /> <img alt="Git" src="https://img.shields.io/badge/Git-C2410C?style=flat-square&logo=git&logoColor=white" /> <img alt="ECS" src="https://img.shields.io/badge/ECS-C2410C?style=flat-square" /></p>

**ML & Research**

<p align="center"><img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-9F1239?style=flat-square&logo=pytorch&logoColor=white" /> <img alt="TensorFlow" src="https://img.shields.io/badge/TensorFlow-9F1239?style=flat-square&logo=tensorflow&logoColor=white" /> <img alt="Scikit-learn" src="https://img.shields.io/badge/Scikit--learn-9F1239?style=flat-square&logo=scikitlearn&logoColor=white" /> <img alt="XGBoost" src="https://img.shields.io/badge/XGBoost-9F1239?style=flat-square" /> <img alt="NLTK" src="https://img.shields.io/badge/NLTK-9F1239?style=flat-square" /> <img alt="SpaCy" src="https://img.shields.io/badge/SpaCy-9F1239?style=flat-square&logo=spacy&logoColor=white" /> <img alt="CUDA" src="https://img.shields.io/badge/CUDA-9F1239?style=flat-square" /></p>

**Quality & Observability**

<p align="center"><img alt="Playwright" src="https://img.shields.io/badge/Playwright-334155?style=flat-square&logo=playwright&logoColor=white" /> <img alt="Jest" src="https://img.shields.io/badge/Jest-334155?style=flat-square&logo=jest&logoColor=white" /> <img alt="pytest" src="https://img.shields.io/badge/pytest-334155?style=flat-square&logo=pytest&logoColor=white" /> <img alt="Sentry" src="https://img.shields.io/badge/Sentry-334155?style=flat-square&logo=sentry&logoColor=white" /> <img alt="OpenTelemetry" src="https://img.shields.io/badge/OpenTelemetry-334155?style=flat-square&logo=opentelemetry&logoColor=white" /> <img alt="Stripe API" src="https://img.shields.io/badge/Stripe_API-334155?style=flat-square&logo=stripe&logoColor=white" /> <img alt="n8n" src="https://img.shields.io/badge/n8n-334155?style=flat-square" /> <img alt="VS Code" src="https://img.shields.io/badge/VS_Code-334155?style=flat-square&logo=visualstudiocode&logoColor=white" /> <img alt="API Development" src="https://img.shields.io/badge/API_Development-334155?style=flat-square" /> <img alt="Model Deployment" src="https://img.shields.io/badge/Model_Deployment-334155?style=flat-square" /></p>

---

## Featured projects

| Project | Status | What it does | Stack | Link |
| --- | --- | --- | --- | --- |
| **MacroSense AI** | In progress · Feb 2026 – Present | Multi-tenant SaaS health platform: provider-agnostic AI routing, enterprise RBAC, Postgres RLS, Langfuse observability, Fitbit OAuth 2.0 PKCE with encrypted token storage, resumable 90-day Inngest backfill, cache-first food search, and privacy-focused data export and deletion. | Next.js, React, Supabase, Inngest, Vercel AI SDK, Anthropic, OpenAI, Langfuse, Fitbit API | [Portfolio](https://www.ashwinbala.com/) |
| **BioCAD** | Research · Aug–Dec 2023 | ASU × Mayo Clinic joint medical imaging research. Unified deep learning pipeline across CheXpert, ChestX-ray14, MIMIC, VinDr-CXR, and ChestX-Det to classify, localize, and segment chest X-rays. Student-teacher contrastive learning with cyclic pretraining to mitigate catastrophic forgetting. ConvNeXt (classification), Faster R-CNN-ResNet (localization), UNet-Swin (segmentation). AUC 0.7348 on ChestX-ray14, mAP 0.115 on VinDr-CXR, Dice 0.4711 on ChestX-Det. 2× A100 GPUs. | PyTorch, TensorFlow, Python, CUDA | [Poster](https://drive.google.com/file/d/1k9IEWwV--laNQxXH9KADFisDp0vlWhtq/view?usp=sharing) |

Public gist: [llm-faq-chatbot-challenge.md](https://gist.github.com/acchu99/924c44fc9aeac09b85a07ae431a1bea0)

---

## Experience

| When | Role |
| --- | --- |
| Jun 2025 – Present | **Applied AI Engineer - agentic development and systems architecture**, [Vizly.ai, Inc.](https://vizly.ai) · Southfield, MI (hybrid) |
| May 2024 – Aug 2024 | **Data Science Summer Intern**, Aggregate Intelligence Inc. · AI assistant using OpenAI APIs and company REST APIs; Next.js chatbot interface |
| Sep 2022 – May 2023 | **Data Analyst and Python Developer**, Aggregate Intelligence Inc. · Coimbatore · RV park market scoring models using statistical and geospatial methods |

At Vizly.ai:

- Tuned prompts and model behavior so agents follow user intent more closely, generate cleaner code, and draw fewer customer-reported quality issues.
- Architected a production Model Context Protocol (MCP) server with OAuth 2.0 so AI agents can securely invoke data integrations across the platform.
- Re-architected JupyterHub with Terraform and AWS, reducing monthly cloud spend by 40% while maintaining 257 ms execution latency and zero downtime incidents.
- Designed enterprise prompt governance for teamspaces: inherited custom prompts, conflict resolution, and guardrail-based policy alignment.
- Resolved 12+ production and P0 issues spanning billing, authentication, and agent response behavior.

---

## Education

| When | Program |
| --- | --- |
| Aug 2023 – May 2025 | **M.S. Computer Science**, Arizona State University · Tempe, AZ |
| Jul 2017 – Jun 2021 | **B.Tech Computer Science & Engineering**, Amrita Vishwa Vidyapeetham · Coimbatore, India |

---

## Reach me

<div align="center">

[![Portfolio](https://img.shields.io/badge/Portfolio-0969DA?style=for-the-badge)](https://www.ashwinbala.com/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/ashwin1999)
[![X](https://img.shields.io/badge/X-334155?style=for-the-badge&logo=x&logoColor=white)](https://x.com/acchu99)
[![GitHub](https://img.shields.io/badge/GitHub-0969DA?style=for-the-badge&logo=github&logoColor=white)](https://github.com/acchu99)

Get in touch through the contact form on [ashwinbala.com](https://www.ashwinbala.com/).

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://capsule-render.vercel.app/api?type=waving&color=0:1f6feb,100:0d1117&height=90&section=footer" />
  <source media="(prefers-color-scheme: light)" srcset="https://capsule-render.vercel.app/api?type=waving&color=0:0969da,100:ffffff&height=90&section=footer" />
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0969da,100:ffffff&height=90&section=footer" alt="" />
</picture>

</div>
