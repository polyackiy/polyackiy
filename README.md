### Anton Poliatskii — AI engineer

I build AI products end to end, from the business problem to production. Before writing software full time I spent a decade running retail and wholesale businesses, so I tend to ask what a system is *for* before asking how to build it.

*Most of my recent work lives in private repositories. The links below are the running products — those are the portfolio.*

**What I'm building**

**[ponpon.life](https://ponpon.life)** — AI personal trainer and nutrition coach. PWA, six languages, iOS and Android betas in progress. Multimodal: meals logged from a photo or by voice, form checked from a short clip, body composition estimated from an image. A background agent reviews yesterday's logs each morning and decides whether there is anything worth saying — usually there isn't.

Two design choices I'd defend anywhere. **The model proposes, the code disposes**: working weights, periodization and calorie corrections all come from a deterministic engine, and everything the model generates is validated before it reaches a human. And **the safety limits are code, not prompts** — eating-disorder protections that hold at any weight, a pregnancy mode that rebuilds both nutrition and training, a handoff to human support on a dark day. I don't guess whether the coach is any good; I measure it on 25 scenarios and took it from 64% to 84%.

**atools** *(private, demo on request)* — multi-tenant analytics and automation platform for Ozon / Wildberries / Yandex Market sellers. FastAPI, Next.js, PostgreSQL, pgvector, Redis, Celery, Docker. Ships a **production MCP server**: roughly 30 tools over unit economics, stock, pricing, supply, ads and reviews, with a company to shops to roles access model, per-shop OAuth consent, deny-by-default scoping at the dispatch layer, plan-based rate limits and response-size budgeting for model context. One tool implementation serves both the internal chat agent and external MCP clients.

The part I'm most pleased with: the agent scores its own past recommendations against what actually happened, and writes up where it was wrong and why.

**[sozdai.app](https://sozdai.app)** — AI infographics for marketplace listings and Avito ads. Live commercial SaaS with paying customers. A pipeline of several LLM roles: a vision model reads the product like a marketer, a second model plays art director and writes a per-generation brief on typography and composition. Prompts are layered — a hard core carrying platform rules, soft style defaults the user overrides in plain text. Text is rendered by code, never by the model. Around 1100 automated tests, CI/CD with zero-downtime deploys and auto-rollback.

**[camoufox-profile-manager](https://github.com/polyackiy/camoufox-profile-manager)** — open-source browser profile manager built on Camoufox. Python and FastAPI backend, Next.js interface, Playwright automation. MIT.

**[MacCam](https://github.com/polyackiy/MacCam)** — offline motion-detecting security camera for macOS. Lives in the menu bar, records HEVC clips on motion. No cloud, no network. Swift, MIT.

**Stack**

Python, FastAPI, Celery, PostgreSQL, pgvector, Redis, Next.js, TypeScript, Docker, MCP, Gemini and Claude APIs, Playwright, Swift.

Daily driver: **Claude Code** (Max plan, daily since early releases); previously Cursor, Windsurf, Codex. In neural networks since 2019, in LLM products since the first public models.

**How I think about this work**

Agents should measure whether their own advice worked. Numbers come from code, prose comes from models. Guardrails belong in tests, not in instructions.

Open to contract work — taking AI prototypes to production, agent systems, MCP servers, RAG.

[Telegram](https://t.me/Bravotangocharlie)
