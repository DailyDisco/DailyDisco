# Hi, I'm Diego

I'm a full-stack engineer in Dallas. I build web products with React, TypeScript, Go and Python, and I look after the CI and cloud infrastructure around them. I also run my own LLM inference server on six RTX 3090s, and when something in that stack is slow or broken I try to fix it upstream.

[Portfolio](https://www.digitaldiego.xyz/) · [LinkedIn](https://www.linkedin.com/in/developerdiego/) · [Resume](https://tinyurl.com/yc2f2d7b) · [Email](mailto:diegoespinowork@gmail.com)

## Open source

Recent work on the ExLlamaV3 inference stack:

- **[ExLlamaV3 #447](https://github.com/turboderp-org/exllamav3/pull/447)** (merged). Multi-threaded the AVX2 path of the CPU all-reduce used for tensor-parallel inference. On a six-GPU host without AVX-512, cold prompt ingestion went from 1,238 to 1,458 tokens per second, with decode speed unchanged.
- **[TabbyAPI #493](https://github.com/theroyallab/tabbyAPI/pull/493)** (merged). Releases the old generator before building its replacement after an engine error. I found it while tracing an out-of-memory crash in which both generators' host caches were resident at once.
- **[ExLlamaV3 #448](https://github.com/turboderp-org/exllamav3/pull/448)** (open). Fair scheduling between prompt ingestion and generation, so one long prompt no longer stalls every other stream. In my tests a second chat kept about 27 tokens per second instead of 3.

## Projects

- **[react-golang-starter-kit](https://github.com/DailyDisco/react-golang-starter-kit)**. A SaaS starter with React 19, TanStack Router and Query on the front end and Go with Chi, GORM and PostgreSQL on the back end. It comes with JWT auth with 2FA and OAuth, multi-tenant organizations with role-based access, Stripe billing, background jobs, WebSockets, Prometheus and Grafana, and CI/CD. It also ships its own agent setup (a CLAUDE.md, pattern-checking hooks, scaffolding skills and decision records), so coding agents follow the project's conventions. [Live demo](https://react-golang-starter-kit.vercel.app)
- **[claude-code-setup](https://github.com/DailyDisco/claude-code-setup)**. The rules, skills, hooks and agents I use with Claude Code every day: 16 rule files, 42 skills, 45 hooks and six specialist agents, with everything tied to my own machines taken out.
- **[linkedin-recommendation-writer](https://github.com/DailyDisco/linkedin-recommendation-writer)**. Reads a developer's GitHub activity and drafts a LinkedIn recommendation from it. FastAPI, React, TypeScript and Gemini.
- **[photography-videography-portfolio-site](https://github.com/DailyDisco/photography-videography-portfolio-site)**. A portfolio site for photographers and videographers with categorized galleries, bookings and Stripe payments. React, Tailwind CSS, ShadCN UI and Go.

## What I run

Most of what I build for myself lives in private repos because it is wired to my own machines. The short version:

- **Local inference.** Six RTX 3090s serving open-weight models through ExLlamaV3 and TabbyAPI behind an OpenAI-compatible gateway, shared by the coding agents on all my machines. The upstream fixes above came out of tuning it.
- **Agent tooling.** One shared set of rules and skills for Claude Code and Codex, kept in sync across Linux, macOS and Windows by an installer that previews, verifies and can roll back. A public copy of the rules, skills and hooks is in [claude-code-setup](https://github.com/DailyDisco/claude-code-setup).
- **Homelab.** Proxmox VMs provisioned by a bootstrap script I maintain (Tailscale-only SSH, metrics and logs from first boot), and a Docker Compose stack of a dozen self-hosted services behind Caddy.
- **Ops dashboard.** A single Go binary, standard library only, with an embedded React front end that shows the state of my scheduled automations.

## How I work

- Small pull requests with conventional commits that explain why.
- Tests check behavior, not implementation.
- Measure before and after any performance change.
- A dashboard never shows missing data as healthy.

## What I work with

- **Frontend:** React, TypeScript, TanStack Router and Query, Tailwind CSS, ShadCN UI, Next.js, React Native
- **Backend:** Go (Chi, GORM), Python (FastAPI), Node.js, PostgreSQL, Redis
- **Infrastructure:** Docker, GitHub Actions, AWS, Terraform, Linux
- **AI:** self-hosted LLM inference (ExLlamaV3, TabbyAPI, vLLM), coding agents, ComfyUI

## Outside of code

I produce bass music in Ableton and I'm learning piano. I speak English and Spanish and I'm learning Japanese.
