# 👋 Manas Srivastava

💼 Backend engineer at **Intuit**. Previously **Sumo Logic** and **Paytm Payments Bank**.

🔗 [LinkedIn](https://www.linkedin.com/in/mastermanas/) &nbsp;·&nbsp; ✉️ mastermanas805@gmail.com

🛠️ 4+ years building and operating production Go services at scale, with experience across Kubernetes, distributed systems, zero-downtime database migrations, and observability infrastructure on multi-tenant platforms.

✍️ I write code in the open. The projects and contributions below are the easiest way to see how I work — reproduction-first, narrow-scope changes, and PR descriptions that aim to make a reviewer's job easy.

## 🌱 Open-source contributions

- **[supabase/auth](https://github.com/supabase/auth)** — the JWT-based authentication service that powers Supabase Auth. Recent contributions across OIDC discovery, web3 (SIWE) sign-in, identity creation flows, and test coverage for previously-untested helpers in the observability and utilities packages.
- **[garrytan/gstack](https://github.com/garrytan/gstack)** — AI-driven engineering toolkit. Contributing `/plan-rollout` and `/spill-check`: skills that decompose large LLM-generated changes into reviewable PR stacks and detect mid-implementation scope creep. SYSTEM.md as a declarative semantic-contract graph at the repo root.

## 🧰 Technical experience

⚙️ Production languages: **Go** (primary, 4+ years), Python, Java, Scala, C++.

- 🗃️ **Data path** — PostgreSQL, MySQL, Redis, Kafka, Elasticsearch.
- ☸️ **Infrastructure** — Kubernetes, AWS, Docker, ArgoCD, Hashicorp Vault.
- 📊 **Observability** — Prometheus, Grafana, Loki, OpenTelemetry.
- 🔁 **CI/CD** — Jenkins, GitHub Actions.
- 🤖 **LLM tooling** — LangChain, MCP servers.

🏗️ Production patterns I've designed and shipped: zero-downtime database migrations across multi-tenant platforms, distributed job scheduling (Kafka queues, Redis caching, consistent hashing, distributed locks), change-data-capture pipelines, on-call incident response automation, secure payment processing, and AI-agent integrations against Postgres / Slack / PagerDuty / Splunk.

## 🧭 How I work

- 🔬 **Reproduce before fixing.** When I claim a bug exists, the PR includes a deterministic reproducer that fails on master and passes after the fix. For non-trivial fixes the PR body also includes a live-environment reproduction (`curl`, signed JWT, DB query) so a reviewer doesn't have to take my word for it.
- 🎯 **Narrow scope, single commit.** A bug fix is one commit and one logical change. Adjacent improvements ride in their own PRs.
- 🧩 **Match the existing house style.** Before writing tests or a refactor I read the surrounding code to figure out the conventions — table-driven tests, assertion library choices, comment density. Diverging from house style is a real cost: reviewers have to ask why.
- 📝 **Technical writing as a deliverable.** Design docs and PR descriptions are part of the work, not an afterthought. A good PR explains the bug, the reproduction, the fix, and the trade-offs in a single read.

## 🚀 Active projects

- 🔍 **[comparator](https://github.com/mastermanas805/comparator)** — client-side semantic diff for YAML / JSON / TOML / XML. No data leaves the browser. TypeScript.
- 🧠 **[AIContext](https://github.com/mastermanas805/AIContext)** — interactive exploration of AI IDE architecture, RAG retrieval, and LLM optimization patterns.
- ⏱️ **[jobmanager](https://github.com/mastermanas805/jobmanager)** — Go service for scheduling, cancelling, and tracking functional jobs.

## 📫 How to reach me

✉️ mastermanas805@gmail.com &nbsp;·&nbsp; 🔗 [LinkedIn](https://www.linkedin.com/in/mastermanas/) &nbsp;·&nbsp; 🐙 [github.com/mastermanas805](https://github.com/mastermanas805)

---

### 📌 Selected pull requests

**supabase/auth**

- 🔧 [#2504](https://github.com/supabase/auth/pull/2504) &nbsp;`fix(provider): preserve non-standard claims in generic OIDC parser` — fixes [#2494](https://github.com/supabase/auth/issues/2494)
- 🔧 [#2507](https://github.com/supabase/auth/pull/2507) &nbsp;`fix(siwe): normalize Ethereum address to lowercase to prevent duplicate identities` — fixes [#2264](https://github.com/supabase/auth/issues/2264)
- 🔧 [#2505](https://github.com/supabase/auth/pull/2505) &nbsp;`fix(api): default OIDC discovery issuer to API_EXTERNAL_URL` — fixes [#2487](https://github.com/supabase/auth/issues/2487)
- 🔧 [#2509](https://github.com/supabase/auth/pull/2509) &nbsp;`fix(api): create email identity when setting password on OAuth-only user` — fixes [#2085](https://github.com/supabase/auth/issues/2085)
- ✅ [#2511](https://github.com/supabase/auth/pull/2511) &nbsp;`chore(observability): add tests for previously-uncovered helpers` — package coverage 17.7% → 81.4%
- ✅ [#2510](https://github.com/supabase/auth/pull/2510) &nbsp;`chore(utilities): add tests for previously-uncovered helpers`
