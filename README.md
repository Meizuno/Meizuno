# Yurii Myronov

**Lead Developer @ [Dlubal Software](https://www.dlubal.com)** · Prague, Czechia 🇨🇿

Full-stack engineer focused on **clean architecture**, **type-safe end-to-end systems**, and **self-hosted infrastructure**. I write production backends in **Go** and **Python**, build reactive frontends with **Nuxt / Vue**, and ship everything through **Docker + GitHub Actions** onto my own **Cloudflare-fronted VPS**. Lately I've been wiring my apps together with the **Model Context Protocol (MCP)** so an LLM can drive them as tools.

---

### What I care about

- **Architecture that's enforced, not aspirational** — Ports & Adapters / DDD, with test suites that fail the build when a dependency rule is broken.
- **Typed boundaries everywhere** — Zod / Pydantic at the edges, types inferred end-to-end, no `any`.
- **Owning the whole cycle** — from a use-case class to a multi-stage Docker image, a GHCR push, a CI gate, and a container running behind a Cloudflare tunnel.

### Tech

![Go](https://img.shields.io/badge/go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![Python](https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/typescript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)

![FastAPI](https://img.shields.io/badge/fastapi-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Django](https://img.shields.io/badge/django-092E20?style=for-the-badge&logo=django&logoColor=white)
![Gin](https://img.shields.io/badge/gin-008ECF?style=for-the-badge&logo=gin&logoColor=white)
![Nuxt](https://img.shields.io/badge/nuxt-00DC82?style=for-the-badge&logo=nuxtdotjs&logoColor=white)
![Vue](https://img.shields.io/badge/vue-4FC08D?style=for-the-badge&logo=vuedotjs&logoColor=white)

![PostgreSQL](https://img.shields.io/badge/postgresql-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Prisma](https://img.shields.io/badge/prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white)

![Docker](https://img.shields.io/badge/docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Cloudflare](https://img.shields.io/badge/cloudflare-F38020?style=for-the-badge&logo=cloudflare&logoColor=white)
![Nginx](https://img.shields.io/badge/nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/github_actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)

### Featured projects

| Project | Stack | What it shows |
|---|---|---|
| **[Library](https://github.com/Meizuno/Library)** | Python · FastAPI · SQLAlchemy | Clean Architecture / DDD reference — 400+ tests that *enforce* the dependency rule, contract-tested ports, Redis caching, structured logging |
| **[Docket](https://github.com/Meizuno/Docket)** | Python · FastAPI · Postgres | Pull-based task queue with lease + heartbeat crash recovery, `FOR UPDATE SKIP LOCKED` concurrency proven via testcontainers — no Redis/Celery needed |
| **[AI Chat](https://github.com/Meizuno/AIChat)** | Nuxt · OpenAI · MCP | A chat hub that drives my other apps (Notes, Money Manager, Recipes) as **MCP tools** — streaming completions, per-user MCP connection pooling, self-hosted Whisper for voice |
| **[Notes](https://github.com/Meizuno/Notes)** ([demo](https://notes.meizuno.com/)) | Nuxt · Prisma · Postgres | Self-hosted notes vault — per-note visibility (private/protected/public), graph + folder views, trigram full-text search, and one data-access layer shared across HTTP, MCP, and SSR |
| **[Authentication](https://github.com/Meizuno/Authentication)** | Go · Gin · JWT | Auth microservice: JWT + refresh-token rotation, Google OAuth, clean layered architecture — one service all my apps delegate to |

### Infrastructure

Everything runs on a self-managed Debian VPS: ~15 Docker services across isolated Compose stacks, a single Go auth service, shared PostgreSQL, a self-hosted **SeaweedFS** S3-compatible cluster, Cloudflare Zero-Trust tunnels for ingress, and Uptime-Kuma for monitoring. Images built by GitHub Actions, pushed to GHCR, pulled on deploy. Also comfortable with Cloudflare **Workers, Pages, D1, and R2**.

### Reach me

[![Portfolio](https://img.shields.io/badge/portfolio-meizuno.com-000000?style=for-the-badge&logo=safari&logoColor=white)](https://meizuno.com/)
[![LinkedIn](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/yurii-myronov-694b99249/)
