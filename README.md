# 👨‍💻 David Joni

**AI-Driven Developer**
Full-Stack across WordPress · WooCommerce · Laravel · Statamic · Vue · React · Next.js · Svelte · Go · and whatever the job needs
Romania (UK & Czech citizen) · 100% Remote
📧 [davidjoni.dev@gmail.com](mailto:davidjoni.dev@gmail.com)
📞 +40 751 988 867 (RO) · +44 7477 363376 (UK)

---

## 🧭 About Me

I'm a **full-stack WordPress / Laravel developer** at heart — 10+ years inside agencies shipping custom themes, plugins, WooCommerce work, and front-end builds. The last stretch I've turned that same craft toward two new customers: **internal teams** and **AI as a serious tool, not a buzzword**.

When I see repetitive work moving through Operations, Sales, Marketing, or Customer Success, my first instinct is to map it properly: what's the workflow, where's the friction, what could be a clean automation, what genuinely still needs a human. Then I build the agent, integration, or internal tool that fits — designed to last, not to demo well. Same instinct in my own work: when my team needed to push WordPress sites from local → staging → live and the only "real" options were paid CI/CD platforms, I built our own internal sync CLI in Go so we'd own the workflow end-to-end instead of paying a monthly subscription.

I work natively with **LLMs** (Claude, Grok, GPT, Cerebras) via their APIs, and I run a heavy **Claude Code** workflow day to day — **MCP servers, custom hooks, slash commands, OpenGrep, marketplace plugins, fal.ai for image generation in-context**. I glue systems together with **REST, webhooks, JSON**, and reach for **Go, Python, or Node** to build the right tool rather than renting one.

I'm honest about where my decade of muscle memory sits (PHP and the WordPress / WooCommerce / Laravel / Statamic ecosystem) and where the AI-assisted workflow extends the range (modern React / Next / Svelte ecosystems). My Claude Code setup with project-aware context, custom hooks, and skills lets me ship in stacks I haven't lived in for years, while staying production-shaped.

I'm a by-the-book builder, not a corner-cutter. I plan in depth before I write a line of code — the stack, the workflow, the data shape, the backend, the frontend, the failure modes — because I want what I build to still be standing six months later, not held together by a stack of "we'll fix that next sprint" notes.

I came up in client-services agencies, which means I'm wired for what client work actually needs: **listening to non-technical stakeholders**, translating fuzzy frustrations into a working tool, shipping fast, gathering feedback, and iterating.

> 🛠 _Joke compiled with this build of the README:_
> Why do programmers prefer dark mode?
> Because **light attracts bugs.** 🐛

---

## 🚀 Things I've Actually Built

### 🌐 Live & Public

**[eternalbeautybyb.co.uk](https://eternalbeautybyb.co.uk)** — _2026, family business site_

- Custom WordPress theme built from scratch (no page builders, no templates) for a Japanese head spa salon.
- Performance-tuned: WebP imagery, video hero with graceful fallback, fast initial paint, semantic HTML.
- Full SEO foundation: canonical URLs, Open Graph & Twitter Card meta, sitemap, structured nav.
- GDPR-compliant cookie consent (real reject/accept, not a dark pattern), GTM integration.

**[getthedomain.app](https://getthedomain.app)** — _live, solo product_

- Bulk domain availability checker with AI-generated business-name suggestions. Solo full-stack build, end-to-end.
- **Backend:** Laravel 13 + Octane (FrankenPHP) + PostgreSQL + Redis. Filament v5 admin panel with dashboard widgets (search volume, TLD popularity, top demanded domains).
- **Frontend:** React 19 + TypeScript + Tailwind CSS v4 + Shadcn/ui via Inertia.js v3.
- **Server-Sent Events** stream concurrent domain results with per-row loading / error / available states.
- **4-step verification pipeline** (DNS → RDAP → WHOIS over raw TCP port 43 → paid DomScan API as fallback) cuts paid API spend ~90% by exhausting free sources first.
- AI name generation via Cerebras + Groq (Llama 3.3 70B) with automatic failover.
- **Automated SEO content pipeline**: 2 articles per day via Claude API, on-brand imagery via fal.ai MCP, published on autopilot via a scheduled Laravel command. Marginal cost ~$0.04 per article.

**[voolu.co.uk](https://voolu.co.uk)** — _2024, main frontend dev_

- Marketing site live for an AI geospatial property platform (UKRI / RICS / Google Cloud / NatWest-backed startup).
- I was main frontend dev on the production web app: **Next.js 14 (App Router) / React 18 / TypeScript / Tailwind**.
- Shipped real-time WebSocket AI chat UI, interactive Mapbox GL globe-projection map with polygon drawing and live area calculation (Turf.js), edge-authenticated Firebase sessions via `next-firebase-auth-edge`.
- The app itself is no longer publicly hosted, but the marketing site is still live as a reference build.

---

### 🔨 Pre-launch / In Active Development

**EchoBedtime** — _solo-built, pre-launch consumer voice-AI app_

- Cross-platform mobile app shipping to **iOS, Android, and web from one codebase** — Expo SDK 55 / React Native / TypeScript / Expo Router.
- **Voice pipeline (turn-based REST):** expo-audio WAV capture → ElevenLabs STT → Claude Haiku → ElevenLabs TTS → base64 MP3 client-side playback. Chose REST after persistent breakages from Expo + package-version updates made the realtime SDK unreliable.
- **Auth + data:** Clerk JWT integrated into Supabase as a third-party provider with row-level security on every table; service-role key isolated to backend; on-device tokens in `react-native-keychain`.
- **Backend:** Node.js / Hono on Hetzner via Coolify; Stripe Checkout Sessions + signed webhooks for subscriptions and one-off upgrades.
- **GDPR by design:** UK data residency (eu-west-2), consent flow before voice capture, on-device audio deleted immediately after upload, Varlock + 1Password secrets architecture keeping sensitive keys out of the client bundle.
- Working dev build is feature-complete on core flows. Targeting public release within ~one month. Product positioning withheld until launch.

---

### 🏗️ Client / Internal Production

**Bespoke WooCommerce Product Configurator** — _client engagement, in staging_

- Fully custom configurable-product interface, well beyond what any off-the-shelf plugin offers.
- Multi-step forms, conditional pricing rules, validation, live preview.
- Component architecture built from scratch with reusable form primitives and state hand-off between steps.
- Integrated against the WooCommerce REST API for product data, order flow, and persistence.
- Currently on staging ahead of the client's public launch — staging link available on request under a short NDA.

**WordPress Sync CLI** — _internal tool, in daily production use_

- Custom Go CLI built to replace paid CI/CD subscriptions with something fitted to the team's actual workflow.
- Single binary, no runtime dependencies. Fast enough to feel instant.
- Syncs local WordPress builds to staging / live servers without monthly fees, custom YAML pipelines, or vendor lock-in.
- Built with the full Claude Code workflow (MCP servers, custom hooks, slash commands, OpenGrep). Cancelled the subscription the week it shipped.

---

### 🧪 Planning

**Competitor / market-gap app**

- Next personal product. Picked because the existing options in the space are slow, expensive, or just badly built.
- Same playbook: identify a real friction, plan the architecture properly, AI-assist where it adds value, ship something built to last.

---

_Additional client agency work (custom WordPress, WooCommerce, Statamic, Vue.js builds across multiple agencies since 2017) available on request — most older client work is under NDA or no longer maintained._

---

## 🤖 How I Actually Work With AI

- **Claude Code as a daily driver** — not just chat, but a properly configured agent: custom hooks, slash commands, MCP servers, marketplace plugins, OpenGrep for codebase search, project-aware context, and custom skills (e.g. a LocalWP wp-cli fixer, an auto doc-update commit hook, an 18-hook security system that auto-rejects predictable AI-agent mistakes like secrets in client bundles or `AsyncStorage` for tokens).
- **CLI-first, MCP when it earns its place.** My default is to expose actions as small, well-scoped CLIs the agent can call — they're easier to test, version, and reason about. I reach for MCP servers when the integration genuinely needs richer context or a long-lived connection (e.g. **fal.ai's MCP** for generating on-brand images inside Claude with full project context, dramatically faster than copy-pasting prompts into a separate UI).
- **Multi-model thinking** — Claude, Grok, GPT each have a personality and a price point; I pick per task and design fallbacks, not lock-in.
- **Prompt engineering with structure** — system prompts, structured outputs, tool use / function calling, prompt caching to keep cost predictable.
- **API-fluent integration glue** — REST, webhooks, JSON, OAuth basics, and the un-glamorous reality that "integration" usually means _making one badly-documented system talk to another badly-documented system_.
- **Build for repeatability.** When a problem will happen again, I solve it once — properly — with a small tool that can be reused, scripted, and handed to someone else without ceremony. UIs go on top _if_ the audience needs one, not by default.

---

## 🛠 Toolbox

**Core (10+ years):** WordPress (custom themes, plugins, Gutenberg blocks, WP-CLI), WooCommerce (custom builders, REST API), PHP 8.x, MySQL, semantic HTML, modern CSS, vanilla JavaScript, jQuery.

**Backend & data (3+ years):** Laravel (10+, Octane / FrankenPHP, Filament v5, Inertia, Breeze / Socialite, queues, schedulers), Statamic, Node.js + Hono, PostgreSQL, Redis, REST APIs, webhooks, OAuth.

**Modern frontend (1-3 years, AI-assisted workflow):** Vue.js (2+ years, native), React + Next.js + TypeScript (production work on Voolu, getthedomain, EchoBedtime — Claude Code-led), Svelte / SvelteKit, React Native + Expo, Tailwind CSS, Shadcn/ui, Framer Motion, GSAP.

**LLMs & AI:** Claude (Sonnet / Opus / Haiku), Grok, Cerebras, ChatGPT, ElevenLabs, Anthropic SDK, OpenAI SDK, Claude Code, MCP, custom hooks, marketplace plugins, OpenGrep, fal.ai (image gen via MCP), tool use / function calling, prompt caching, RAG basics.

**Automation:** Custom CLIs (Go / Node / Python), cron jobs, webhooks, GitHub Actions, scheduled Laravel commands.

**Infra & deploy:** Git, Vite, Webpack, npm / yarn, Composer; Railway, Hetzner / Coolify, Vercel, Cloudflare; basic Go (built a production internal CLI); Plesk / cPanel.

**Design:** Adobe Photoshop, XD, Illustrator, Premiere.

---

## 💼 Experience

### **Web Developer — Northern Media** _(Remote)_

**September 2024 – Present**

- Build and ship custom WordPress themes, plugins, and bespoke product UI across a portfolio of client sites.
- Built an **internal WordPress sync CLI** in **Go** (paired with Claude Code) for pushing local builds to staging / live, replacing paid CI/CD and automation subscriptions.
- Daily **Claude Code** workflow (MCP servers, custom hooks, slash commands, OpenGrep, marketplace plugins) for dev, debugging, and content tasks.
- Built a **bespoke WooCommerce product configurator** for a client using the same agent-driven workflow.
- Wired together internal services and 3rd-party APIs via REST, webhooks, JSON.

### **Web Developer — Kaweb** _(Remote)_

**August 2023 – Present**

- Delivered responsive WordPress and **Statamic** builds with interactive **Vue.js** components.
- Worked directly with non-technical stakeholders to translate vague briefs into shipped, pixel-perfect product.

### **Web Developer — Dash Media** _(Darlington)_

**September 2021 – August 2023**

- Built cross-browser sites with custom plugins and bespoke functionality fitted to each client's actual workflow.
- Owned Google Workspace, Microsoft Exchange, and cPanel/Plesk admin — the unglamorous integration plumbing real businesses run on.
- Collaborated with project managers to scope, ship, and iterate on eCommerce and brochure projects.

### **Earlier roles — Zeek · Purehosting** _(UK)_

**April 2017 – September 2021**

- End-to-end WordPress site builds in PHP, JavaScript, jQuery, CSS — design (Photoshop) through implementation and ongoing maintenance.
- Delivered user-friendly admin dashboards so non-technical clients could self-serve. The agency reflex of shipping value, not just code.

---

## 🎓 Education

**BSc Games Software Development** · _University of Sunderland_ · Sep 2014 – Jul 2017
**A Levels in Information Technology** · _Queen Elizabeth Sixth Form College, Darlington_ · Sep 2012 – Aug 2014

---

## 🌍 Languages

| Language  | Proficiency                                |
| --------- | ------------------------------------------ |
| Czech     | Native (first language)                    |
| English   | C2 (Proficient, assessed) — UK-educated    |
| Slovakian | Strong comprehension (not written)         |
| Polish    | Basic understanding                        |
| Romanian  | Partial comprehension, conversational basics |

---

## 🪪 Personal Details

- **Citizenship:** British & Czech (full EU + UK right to work, no visa or sponsorship needed)
- **Based in:** Romania — Romanian tax-resident, work invoiced through Romanian SRL for non-UK clients
- **Time zone:** EET / EEST — flexible for European and US Eastern hours
- **Driver's Licence:** AM, B, BE
- **Experience:** 10+ years across agencies and remote teams

---

## 🧩 Interests

**Tech**

- AI agents, prompt engineering, MCP, and the broader "future of work" stack
- Building side-projects (getthedomain.app, EchoBedtime, internal tooling) and small "scratch your own itch" automations
- Clean UI and front-end performance
- WordPress / WooCommerce deep work
- Backend scripting in Python and Go

**Outside of code**

- Husband and dad to two girls — the real reason I care about workflows that don't waste time
- '90s and early-2000s cars — Honda Civic & CRX, Toyota Supra, Mazda RX-7 and MX-5 / Miata, Nissan Skyline. The era when cars still felt mechanical.
- Still play games from time to time — Metal Gear Solid and Need for Speed will always be my favourites.

---

## 🛠 Built with Claude Code

This README was authored end-to-end using **Claude Code (Opus 4.7)** — same Claude Code workflow I use professionally: MCP servers for context, custom hooks, slash commands, marketplace plugins, OpenGrep for in-repo search. Felt only fair to dogfood the toolset I'm pitching.

<details>
<summary><em>The (lightly polished) prompt that produced this version</em></summary>

> Rewrite my GitHub profile README from scratch with the projects I've actually shipped — getthedomain.app (live, AI-driven Laravel + React product), EchoBedtime (pre-launch consumer voice-AI app), Voolu (UKRI / RICS / Google Cloud / NatWest-backed property platform where I was main frontend dev), the bespoke WooCommerce product configurator, the internal Go-based WordPress sync CLI, and eternalbeautybyb.co.uk.
>
> Reflect how I actually work with AI: Claude Code as a daily driver, MCP servers, custom hooks, slash commands, OpenGrep, marketplace plugins, multi-model orchestration (Claude / Grok / GPT), fal.ai's MCP for image gen with full project context, and custom skills like the LocalWP wp-cli fixer and the 18-hook security system.
>
> Be honest about my background: PHP / WordPress / Laravel / Statamic is the 10+ year foundation, with React / Next / Svelte work being AI-assisted ramp-ups via Claude Code rather than long-standing primary stacks. Don't oversell modern frontend depth.
>
> Keep my voice — dry, direct, mildly funny — and the joke. Add a note at the bottom that this README was built with Claude Code, and include a polished version of this prompt as a sneak peek.

</details>

---

> © 2026 David Joni
> _This is the markdown version of my résumé / portfolio for GitHub use._
