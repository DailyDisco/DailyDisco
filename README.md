# Hi, I'm Diego

I'm a full-stack engineer in Dallas. I build web products with React, TypeScript, Go and Python, and I look after the CI and cloud infrastructure around them. I also run my own LLM inference server on six RTX 3090s, and when something in that stack is slow or broken I try to fix it upstream.

[Portfolio](https://www.digitaldiego.xyz/) · [LinkedIn](https://www.linkedin.com/in/developerdiego/) · [Resume](https://tinyurl.com/yc2f2d7b) · [Email](mailto:diegoespinowork@gmail.com)

## Open source

Recent work on the ExLlamaV3 inference stack:

- **[ExLlamaV3 #447](https://github.com/turboderp-org/exllamav3/pull/447)** (merged). Multi-threaded the AVX2 path of the CPU all-reduce used for tensor-parallel inference. On a six-GPU host without AVX-512, cold prompt ingestion went from 1,238 to 1,458 tokens per second, with decode speed unchanged.
- **[TabbyAPI #493](https://github.com/theroyallab/tabbyAPI/pull/493)** (merged). Releases the old generator before building its replacement after an engine error. I found it while tracing an out-of-memory crash in which both generators' host caches were resident at once.
- **[ExLlamaV3 #448](https://github.com/turboderp-org/exllamav3/pull/448)** (open). Fair scheduling between prompt ingestion and generation, so one long prompt no longer stalls every other stream. In my tests a second chat kept about 27 tokens per second instead of 3.

## Projects

- **[react-golang-starter-kit](https://github.com/DailyDisco/react-golang-starter-kit)**. A SaaS starter with React 19, TanStack Router and Query on the front end and Go with Chi, GORM and PostgreSQL on the back end. It comes with JWT auth with 2FA and OAuth, multi-tenant organizations with role-based access, Stripe billing, background jobs, WebSockets, Prometheus and Grafana, and CI/CD. [Live demo](https://react-golang-starter-kit.vercel.app)
- **[linkedin-recommendation-writer](https://github.com/DailyDisco/linkedin-recommendation-writer)**. Reads a developer's GitHub activity and drafts a LinkedIn recommendation from it. FastAPI, React, TypeScript and Gemini.
- **[photography-videography-portfolio-site](https://github.com/DailyDisco/photography-videography-portfolio-site)**. An open-source portfolio template for photographers and videographers. React, Tailwind CSS, ShadCN UI and Go.

## What I work with

- **Frontend:** React, TypeScript, TanStack Router and Query, Tailwind CSS, ShadCN UI, Next.js, React Native
- **Backend:** Go (Chi, GORM), Python (FastAPI), Node.js, PostgreSQL, Redis
- **Infrastructure:** Docker, GitHub Actions, AWS, Terraform, Linux
- **AI:** self-hosted LLM inference (ExLlamaV3, TabbyAPI, vLLM), coding agents, ComfyUI

## Outside of code

I produce bass music in Ableton and I'm learning piano. I speak English and Spanish and I'm learning Japanese.
