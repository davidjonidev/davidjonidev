# 👨‍💻 David Joni

**AI-Driven Developer**  
Full-Stack across WordPress · WooCommerce · React · Next.js · Vue · Laravel · Statamic · Go · and whatever the job needs  
UK / EU · 100% Remote  
📧 [davidjoni.dev@gmail.com](mailto:davidjoni.dev@gmail.com)  
📞 +44 7477 363376

---

## 🧭 About Me

I'm a **full-stack WordPress developer** at heart — 10+ years inside agencies shipping custom themes, plugins, WooCommerce work, and front-end builds in React, Next.js, Vue, Laravel, and Statamic. The last stretch I've turned that same craft toward two new customers: **internal teams** and **AI as a serious tool, not a buzzword**.

When I see repetitive work moving through Operations, Sales, Marketing, or Customer Success, my first instinct is to map it properly: what's the workflow, where's the friction, what could be a clean automation, what genuinely still needs a human. Then I build the agent, integration, or internal tool that fits — designed to last, not to demo well. Same instinct in my own work: when my team needed to push WordPress sites from local → staging → live and the only "real" options were paid CI/CD platforms, I built our own internal sync CLI in Go so we'd own the workflow end-to-end instead of paying a monthly subscription.

I work natively with **LLMs** (Claude, Grok, GPT, Cerebras) via their APIs, and I run a heavy **Claude Code** workflow day to day — **MCP servers, custom hooks, slash commands, OpenGrep, marketplace plugins, fal.ai for image generation in-context**. I glue systems together with **REST, webhooks, JSON**, and reach for **Go, Python, or Node** to build the right tool rather than renting one.

I'm a by-the-book builder, not a corner-cutter. I plan in depth before I write a line of code — the stack, the workflow, the data shape, the backend, the frontend, the failure modes — because I want what I build to still be standing six months later, not held together by a stack of "we'll fix that next sprint" notes. I've developed a strong gut for system architecture from years of agency work, and I lean on it heavily when scoping projects. When I reach for a tool, I want to use the _full_ power of it, not a fashionable subset of it.

I came up in client-services agencies, which means I'm already wired for what this role actually needs: **listening to non-technical stakeholders**, translating fuzzy frustrations into a working tool, shipping fast, gathering feedback, and iterating.

> 🛠 _Joke compiled with this build of the CV:_
> Why do programmers prefer dark mode?
> Because **light attracts bugs.** 🐛

---

## 🚀 Things I've Actually Built

### **[getthedomain.app](https://getthedomain.app)** — AI domain-name finder _(personal product, live)_

- Full product designed and built solo: idea → UI → AI pipeline → live.
- Generates domain suggestions by orchestrating **Grok (xAI)** and **Cerebras** together, so the output isn't tied to a single model's quirks and stays fast / cost-efficient on Cerebras' free tier.
- Real production concerns: prompt design, structured outputs, latency, cost, fallback when an upstream model misbehaves.

### **EchoBedtime** — AI bedtime-story app _(in active development)_

- Personal app that turns a few inputs from a parent into a tailored bedtime story (and the kind of audio + imagery that makes a kid actually want to listen).
- Built with the same multi-model + media pipeline mindset I use professionally — LLMs for narrative, image gen for scene art, all stitched together as one product, not a demo.

### **WordPress Sync CLI** — internal dev-ops tool at current role _(production, in daily use)_

- Built to replace paid CI/CD subscriptions with something fitted to how our team actually works.
- Written in **Go**, paired with **Claude Code** — single binary, no runtime dependencies, fast enough to feel instant.
- Syncs local WordPress builds to staging / live servers without monthly platform fees, custom YAML pipelines, or "computer says no" tickets.
- A clean _"build the right tool properly instead of renting a generic one"_ outcome — fitted to the team's workflow, owned end-to-end, no recurring fees.

### **Bespoke WooCommerce Product Builder** — client work, built with Claude Code

- Fully custom configurable-product builder inside WooCommerce (well past what off-the-shelf plugins can do).
- Built using a heavy **Claude Code** workflow: MCP servers for project context, custom hooks, OpenGrep-powered codebase search, and marketplace plugins to keep the agent inside guard-rails.
- Demonstrates I don't just _use_ AI — I treat my agent like a junior engineer I've onboarded properly: with tools, context, and rules.

### **Competitor / market-gap app** — next personal project _(planning)_

- Picked because the existing options in the space are slow, expensive, or just badly built.
- Same playbook: identify a real friction, plan the architecture properly, AI-assist where it adds value, ship something built to last.

---

## 🤖 How I Actually Work With AI

- **Claude Code as a daily driver** — not just chat, but a properly configured agent: custom hooks, slash commands, MCP servers, marketplace plugins, OpenGrep for codebase search, and project-aware context.
- **CLI-first, MCP when it earns its place.** My default is to expose actions as small, well-scoped CLIs the agent can call — they're easier to test, version, and reason about. I reach for MCP servers when the integration genuinely needs richer context or a long-lived connection (e.g. **fal.ai's MCP** for generating images inside Claude with full project context, which is dramatically faster than copy-pasting prompts into a separate UI).
- **Multi-model thinking** — Claude, Grok, GPT each have a personality and a price point; I pick per task and design fallbacks, not lock-in.
- **Prompt engineering with structure** — system prompts, structured outputs, tool use / function calling, prompt caching to keep cost predictable.
- **API-fluent integration glue** — REST, webhooks, JSON, OAuth basics, and the un-glamorous reality that "integration" usually means _making one badly-documented system talk to another badly-documented system_.
- **Build for repeatability.** When a problem will happen again, I solve it once — properly — with a small tool that can be reused, scripted, and handed to someone else without ceremony. UIs go on top _if_ the audience needs one, not by default.

---

## 🛠 Toolbox

**LLMs & AI:** Claude (Sonnet / Opus / Haiku), Grok, Cerebras, ChatGPT, Anthropic SDK, OpenAI SDK, Claude Code, MCP, custom hooks, marketplace plugins, OpenGrep, fal.ai (image gen via MCP), tool use / function calling, prompt caching, RAG basics
**Automation:** custom CLIs (Go / Node / Python), cron jobs, webhooks, GitHub Actions
**Languages:** JavaScript / TypeScript, Python, PHP, Go (built a production sync CLI in it)
**Web:** Next.js, React, Vue.js, Node.js, Laravel, WordPress (custom themes + plugins, WooCommerce deep-end)
**Integrations:** REST, Webhooks, JSON, OAuth basics, CRM ↔ AI tool sync
**Front-end:** HTML5, CSS3, SASS, Tailwind, Bootstrap, Framer Motion
**Tooling:** Git, Composer, Vite, Webpack, npm / yarn, Plesk / cPanel
**Design:** Adobe Photoshop, XD, Illustrator, Premiere

---

## 💼 Experience

### **Web Developer — Northern Media** _(Remote)_

**September 2024 – Present**

- Build and ship custom WordPress themes and tooling across a portfolio of client sites.
- Built an **internal WordPress sync CLI** in **Go** (paired with Claude Code) for pushing local builds to staging / live, replacing paid CI/CD and automation subscriptions — saves recurring spend and fits how the team actually works.
- Use **Claude Code** as a daily-driver agent (MCP servers, custom hooks, slash commands, OpenGrep, marketplace plugins) to compress turnaround time on dev, debugging, and content tasks.
- Built a **bespoke WooCommerce product builder** for a client using the same agent-driven workflow.
- Wired together internal services and 3rd-party APIs via **REST, webhooks, JSON** so systems stay in sync without manual exports.

### **Web Developer — Kaweb** _(Remote)_

**August 2023 – Present**

- Delivered responsive WordPress and **Statamic** builds with interactive **Vue.js** components.
- Worked directly with non-technical stakeholders to translate vague briefs into shipped, pixel-perfect product.
- Picked up new platforms on the job — same "Google, read the docs, fix it" mindset I bring to every new API or AI tool.

### **Web Developer — Dash Media** _(Darlington)_

**September 2021 – August 2023**

- Built cross-browser sites with custom plugins and bespoke functionality fitted to each client's actual workflow.
- Owned **Google Workspace, Microsoft Exchange, and cPanel/Plesk** admin — the unglamorous integration plumbing real businesses run on.
- Collaborated with project managers to scope, ship, and iterate on eCommerce and brochure projects under real deadlines and real budgets.

### **Web Developer — Zeek** _(Newton Aycliffe)_

**September 2020 – September 2021**

- Built and maintained custom WordPress sites in PHP, JS, jQuery, and CSS.
- Ran weekly maintenance, diagnosed faults, and minimised downtime — the operational rigour an internal-tools role lives or dies by.
- Delivered user-friendly admin dashboards so non-technical clients could self-serve.

### **Web Developer — Purehosting** _(Coventry)_

**April 2017 – September 2020**

- Built fully custom WordPress sites end-to-end — design in Photoshop, implementation in PHP / HTML / CSS / JS, ongoing health checks.
- Worked closely with management against revenue targets and a real backlog — early lessons in shipping value, not just code.
- Where I learned the agency reflex this role rewards: _understand the business first, then build the thing._

---

## 🧠 Why I'm a Strong Fit for Internal AI Tools at Hostaway

- **Business-focused builder.** A decade of agency work has trained me to start from "what does this team actually need?" not "what's cool to build?" I measure success in hours saved, handoffs removed, and deals / campaigns unblocked.
- **Genuine tinkerer.** I ship side-projects (getthedomain.app, EchoBedtime, an internal sync tool, more in the pipeline). The Hostaway listing called out Discord bots, automating personal tasks, and serious LLM experimentation as a positive signal — that's literally how I spend my evenings.
- **By-the-book, not corner-cutting.** I plan in depth — stack, workflow, data shape, backend, frontend, failure modes — and I want every tool I use working at its full potential, not half-configured. When the right answer is a custom CLI in Go instead of a paid SaaS subscription, I build it properly so it still works in six months. The internal WordPress sync CLI is the cleanest example.
- **Strong architectural instinct.** Years of agency work have given me a reliable gut for system design — picking the right stack, sequencing the build, and spotting where things will break before they do.
- **API-fluent.** Comfortable reading docs, wiring up REST endpoints, handling auth, parsing JSON, and debugging webhooks across systems that "should" talk to each other but don't.
- **Empathetic communicator.** I can sit with a CS rep, a marketer, or an ops lead, listen to what's _actually_ slowing them down, and explain the fix in language they trust. Fluent in **English** and **Czech**, strong **Slovakian** comprehension, basic **Polish** — useful in a 40+ country team.
- **Remote-native.** Fully remote since 2020 across UK and EU teams, no drop in throughput or communication.

---

## 🎓 Education

**BSc Games Software Development** · _University of Sunderland_ · Sep 2014 – Jul 2017  
**A Levels in Information Technology** · _Queen Elizabeth Sixth Form College, Darlington_ · Sep 2012 – Aug 2014

---

## 🌍 Languages

| Language  | Proficiency                             |
| --------- | --------------------------------------- |
| English   | Fluent                                  |
| Czech     | Fluent                                  |
| Slovakian | Strong comprehension (not written)      |
| Polish    | Basic understanding                     |
| Romanian  | Partial comprehension, few spoken words |

---

## 🪪 Personal Details

- **British Citizen:** ✅ Full right to work in the UK
- **Based in:** UK / EU — fully remote-ready
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
- Sharing dev tips and tech humour

**Outside of code**
- Husband and dad to two girls — the real reason I care about workflows that don't waste time
- '90s and early-2000s cars — Honda Civic & CRX, Toyota Supra, Mazda RX-7 and MX-5 / Miata, Nissan Skyline. The era when cars still felt mechanical
- Still play games from time to time — Metal Gear Solid and Need for Speed will always be my favourites

---

## 🛠 Built with Claude Code

This CV was authored end-to-end using **Claude Code (Opus 4.7)** — same Claude Code workflow I use professionally: MCP servers for context, custom hooks, slash commands, marketplace plugins, OpenGrep for in-repo search. Felt only fair to dogfood the toolset I'm pitching.

<details>
<summary><em>The (lightly polished) prompt that produced this version</em></summary>

> Rewrite my CV from scratch to genuinely target the **[role redacted]** position — without inventing anything.
>
> Real projects to feature: **getthedomain.app** (live, AI domain finder using Grok + Cerebras); **EchoBedtime** (in active development); the **internal WordPress sync CLI** I built in Go with Claude Code to replace paid CI/CD subscriptions with something fitted to our actual workflow; a **bespoke WooCommerce product builder** built with Claude Code; and a competitor / market-gap app I'm about to start.
>
> Reflect how I actually work with AI: Claude Code as a daily driver, MCP servers, custom hooks, slash commands, OpenGrep, marketplace plugins, multi-model orchestration (Claude / Grok / GPT), and using fal.ai's MCP to generate images inside Claude with full project context.
>
> Keep my voice — dry, direct, mildly funny — and replace the joke with a fresh one, framed as something a bit more clever than "joke of the day". Add a note at the bottom that this CV was built with Claude Code, and include a polished version of this prompt as a sneak peek.
>
> Be honest about what I've shipped. I want to land this role because I genuinely love building tools with AI — make that read as authentic, not as buzzwords.

</details>

---

> © 2026 David Joni
> _This README CV is a markdown version of my résumé for GitHub / portfolio use._
