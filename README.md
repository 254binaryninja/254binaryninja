# Arnold Musandu

**Platform / Backend Engineer** in Nairobi. I build and run high-traffic systems: betting, ticketing, payments, and AI-backed learning tools.
I care about systems that are fast, observable, cost-efficient, and **boring in production**.

<p align="center">
  <img src="./assets/request-trace.svg" alt="Animated request trace: client → Cloudflare → Kong → Go service → Postgres, with a fraud-detect branch" width="100%">
</p>

<p align="center"><a href="https://claude.ai/artifact/P572fkpkEJeSm8n8JAx7A7"><b>↗ Explore the interactive system map</b></a></p>

---

## What I run in production

| Product | What I do | Live |
|---|---|---|
| **Tucheze**: betting platform, 1M+ users | Moved Django to a Go V2 stack on DigitalOcean behind Kong. I tune Postgres query plans and schema to cut infra cost, built the fraud-detection services, and own CI/CD and the staged staging → prod rollouts. | [tucheze.com](https://tucheze.com) |
| **MyTickets.africa**: event ticketing | Runs on the same gateway and deploy pipeline as Tucheze. | [mytickets.africa](https://mytickets.africa) |
| **CloudPay**: payments | Gateway, infra, and rollout workflow; patched Kong across all three stacks for the Nov 2026 nginx CVEs. | [cloudpay.africa](https://cloudpay.africa) |
| **FaidaBet**: betting site | Next.js frontend with Payload CMS, a back office, and an embedded sportsbook and games. | [faidabet.co.ke](https://faidabet.co.ke) |
| **GigForce**: gig-work marketplace | API, frontend, and infra. | [gigforce.africa](https://gigforce.africa) |
| **PropMS**: property management | Core backend plus an internal ops console that imports the core as a library. | |

## Campus Connect: AI learning platform (200+ students)

Split into two services on a shared Postgres:

* **nightwing**: a Go gateway and CRUD API (chi · pgx · sqlc)
* **robin**: an AI service (Bun · Hono · Vercel AI SDK). It does RAG over Pinecone with Gemini embeddings and runs a document ingestion pipeline (extract → summarize → chunk → embed). A **multi-provider model router** handles failover with cooldowns, monthly spend caps, and per-call usage logging.

## Earlier

**Savannah Informatics** (healthcare): sped up NX monorepo CI and led the Keycloak auth migration · Angular · TypeScript · NX

---

## Open source

* **[graphindex](https://github.com/254binaryninja/graphindex)**: a lightweight Go MCP server that indexes codebases so AI coding agents can navigate them faster and cheaper
* **[ngao-kijani](https://github.com/254binaryninja/ngao-kijani)**: open-source ESG tooling
* **[Daily Bible API](https://github.com/254binaryninja/daily-bible-api)**: a REST API serving structured scripture
* **[NSE Data Pipeline](https://github.com/254binaryninja/project-soko-data)**: ingestion and processing for the Nairobi Stock Exchange

## Toolbox

* **Backend**: Go, Python, TypeScript/Node, Bun · PostgreSQL, MongoDB · REST, gRPC
* **Infra**: Docker, Kong, DigitalOcean, GCP, Cloudflare · GitHub Actions, GitLab CI · zero-surprise migrations
* **AI**: Vercel AI SDK, RAG, Pinecone, multi-provider LLM routing, MCP
* **Frontend (when needed)**: React, Next.js, Angular

## Learning deeply

PostgreSQL internals & query planning · schema design under load · Java & Spring Boot · container orchestration

## Education

**BSc Economics & Statistics**, Kenyatta University *(expected 2027)*

---

Building **developer tools, platform infrastructure, or data-heavy systems**? Let's talk.
[arnoldmusandu@gmail.com](mailto:arnoldmusandu@gmail.com) · [LinkedIn](https://www.linkedin.com/in/arnold-musandu-3489b2293/) · Nairobi, Kenya

> *Systems that scale, and stay sane in production.*
