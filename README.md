# Hi, I'm Diego

I'm a full-stack engineer and founder of Lumara Technologies in Dallas. I build products with React, TypeScript, Go, Python and PostgreSQL, from architecture and APIs through deployment and operations. I'm interested in senior and lead full-stack roles that also draw on my cloud and infrastructure experience.

I also build and run my own GPU inference systems. That work has led to merged performance and reliability fixes in ExLlamaV3 and TabbyAPI.

[Portfolio](https://www.digitaldiego.xyz/) · [LinkedIn](https://www.linkedin.com/in/developerdiego/) · [Resume (1 page)](resume/Diego_Espino_Resume.pdf) · [Detailed resume (2 pages)](resume/Diego_Espino_Resume_Detailed.pdf) · [Email](mailto:diegoespinowork@gmail.com)

## Recent work

My consulting work runs through Lumara, including my primary engagement with DFW Software Consulting.

- **Full-stack delivery at DFW Software Consulting.** Architecture, data modeling and releases for a property platform serving 1,000+ units. Invoicing and reporting automation reduced daily administrative work from 3 hours to 1 hour per employee. I also led a five-developer team building a truck damage estimator with image analysis and VIN extraction.
- **Cloud migration at Craft Digital.** Migrated seven production lead-intake workflows from Kestra on AWS to n8n on Railway for Joshua Tree Experts. Built durable intake, reporting pipelines for 27 franchise locations plus corporate, and PostgreSQL dashboard readers with tenant-scoped access and consistent snapshots.
- **Backend and infrastructure for a confidential mixed reality platform.** FastAPI/PostgreSQL APIs, Redis-backed shared state, resumable event streaming, Cognito authentication, scoped permissions and Unity/C# contract checks. Defined development ElastiCache infrastructure with Terraform, private subnets and scoped network access.
- **Volunteer frontend work at Games For Love.** Next.js, TypeScript and accessible components for a nonprofit streaming and donation platform.

## Open source

- **[ExLlamaV3 #447](https://github.com/turboderp-org/exllamav3/pull/447), merged.** Multithreaded the AVX2 CPU all-reduce path for tensor-parallel inference. Cold prompt throughput improved **18%, from 1,238 to 1,458 tokens/second**, on my six-GPU benchmark. Decode speed was unchanged.
- **[TabbyAPI #493](https://github.com/theroyallab/tabbyAPI/pull/493), merged.** Fixed generator replacement after an engine error so the old generator's main-process host caches are released before the replacement is allocated. Added a regression test for object release.
- **[ExLlamaV3 #448](https://github.com/turboderp-org/exllamav3/pull/448), proposed.** An open contribution exploring fair scheduling between prompt processing and generation. It trades longer prompt ingestion for more responsive concurrent streams; benchmark details and limitations are in the PR.

## Infrastructure I run

- **Local AI:** six NVIDIA RTX 3090 GPUs with 144 GB of combined GPU memory, ExLlamaV3 and TabbyAPI, and an OpenAI-compatible gateway for coding agents.
- **Homelab:** Proxmox VMs, Linux, Docker Compose and Caddy. I maintain provisioning scripts with Tailscale-only SSH, metrics and logs from first boot.
- **Developer tooling:** shared agent configuration across Linux, macOS and Windows, with preview, verification and rollback. A Go service with an embedded React frontend monitors scheduled automations.

## Selected projects

- **[React and Go SaaS starter](https://github.com/DailyDisco/react-golang-starter-kit):** React/TypeScript, Go/Chi and PostgreSQL, with multi-tenant access, authentication, Stripe billing, background jobs, tests, Docker deployment and observability. [Live demo](https://react-golang-starter-kit.vercel.app)
- **[Claude Code setup](https://github.com/DailyDisco/claude-code-setup):** a public version of the rules, skills, hooks and agent workflows I use, with machine-specific configuration removed.
- **[Photography and videography portfolio](https://github.com/DailyDisco/photography-videography-portfolio-site):** galleries, bookings and Stripe payments with React and Go.

## How I work

I measure performance changes, test failure and recovery paths, and keep rollback practical. Data freshness, tenant boundaries and explicit failure states matter as much as the happy path.

**Tools:** React, Next.js, TypeScript, Go, Python/FastAPI, PostgreSQL, Redis, AWS, Railway, Terraform, Docker, GitHub Actions, n8n, dbt, Prometheus and Grafana.

**Certifications:** AWS Certified Developer - Associate and AWS Certified Cloud Practitioner.

Outside of code, I produce bass music in Ableton and I'm learning piano. I speak English and Spanish and I'm learning Japanese.
