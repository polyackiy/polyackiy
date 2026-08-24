### Anton Poliatskii — AI engineer

I build AI products end to end, from the business problem to production. Before writing software full time I spent a decade running retail and wholesale businesses, so I tend to ask what a system is *for* before asking how to build it.

*Most of my recent work lives in private repositories. The links below are the running products — those are the portfolio.*

**What I'm building**

**[atools.vip](https://atools.vip)** — an AI manager for marketplace sellers: Ozon, Wildberries, Yandex Market, Avito. It watches prices, ads, supplies and reviews, catches problems early and proposes fixes, acting only inside the limits the seller sets. Ships a production MCP server (~30 tools) with per-shop OAuth consent and deny-by-default scoping at the dispatch layer. The part I like most: the agent scores its own past recommendations against what actually happened.

**[ponpon.life](https://ponpon.life)** — AI personal trainer and nutrition coach. PWA, six languages, iOS and Android betas. The model composes and talks, but every number comes from a deterministic engine, and safety limits live in code rather than prompts. Coach quality is measured on 25 scenarios: took it from 64% to 84%.

**[sozdai.app](https://sozdai.app)** — AI infographics for marketplace listings and Avito ads. Live SaaS with paying customers. Layered pipeline: a vision model reads the product, a second model works as art director, a classifier turns user wishes into structural overrides without breaking the hard core. ~1100 tests, CI/CD with zero-downtime deploys and auto-rollback.

**[camoufox-profile-manager](https://github.com/polyackiy/camoufox-profile-manager)** — open-source browser profile manager built on Camoufox. Python/FastAPI, Next.js, Playwright. MIT.

**[MacCam](https://github.com/polyackiy/MacCam)** — offline motion-detecting security camera for macOS. Lives in the menu bar, records HEVC on motion, no cloud. Swift, MIT.

**Stack**

Python, FastAPI, Celery, PostgreSQL, pgvector, Redis, Next.js, TypeScript, Docker, MCP, Gemini and Claude APIs, Playwright, Swift.

Daily driver: **Claude Code** (Max plan, daily since early releases); previously Cursor, Windsurf, Codex. In neural networks since 2019, in LLM products since the first public models.
