<div align="center">

<br>

# · nomi ·

### Personal intelligence that truly knows you.

*An AI ecosystem where your personal assistant understands your goals deeply —*
*and runs an entire company of AI workers on your behalf.*

<br>

</div>

---

## 💡 Why Nomi

Every AI assistant today starts from zero.
New conversation. No memory. No context. No continuity.

And today's AI agent tools require you to manually orchestrate every task, every time.

We believe both of these are the wrong model.

A personal AI should work the way a trusted Chief of Staff does —
accumulating context over time, understanding your goals, and taking action
on your behalf without needing to be told twice.

> **Nomi is the infrastructure for that future.**

<br>

---

## ✨ How It Works

You talk to **nomi-biseo** — your personal AI Chief of Staff.
It understands what you want, remembers your context, and dispatches work
to a team of AI workers inside **nomi-company**.

```
You: "I need a landing page for my new product by Friday"
        │
        ▼
  nomi-biseo  (Chief of Staff)
  ┌─────────────────────────────────────────┐
  │  Knows: you prefer minimal design       │
  │  Knows: your brand tone and standards   │
  │  Knows: Friday = 3 days away            │
  │  Plans: Designer → Frontend → QA        │
  └──────────────┬──────────────────────────┘
                 │  assigns tasks with full context
                 ▼
  nomi-company  (AI Worker Team)
  ├── 🎨 Designer Agent   → layout and visuals
  ├── 💻 Frontend Agent   → builds the page
  └── 🔍 QA Agent         → reviews and validates
                 │
                 ▼
  nomi-biseo reports back to you
  "Landing page is ready. I noticed you approved
   this design style quickly — I'll remember that."
```

Every completed task feeds back into nomi-biseo's memory.
The more you use Nomi, the less you need to explain.

<br>

---

## 🏗️ The Ecosystem

Nomi follows a layered architecture. Each layer has one responsibility.

```
╔══════════════════════════════════════════════════╗
║              nomi-company  (future)              ║
║       AI Worker Team  ·  Multi-Agent Execution   ║
║       Dashboard: observe workers in action       ║
╠══════════════════════════════════════════════════╣
║                  nomi-biseo                      ║
║          Personal AI  ·  Chief of Staff          ║
║     Memory  ·  Goals  ·  Context  ·  Delegation  ║
╠══════════════════════════════════════════════════╣
║                  nomi-core                       ║
║              AI Execution Engine                 ║
║      LLM Adapters  ·  Retry  ·  Costs            ║
╚══════════════════════════════════════════════════╝
```

<br>

### ⚙️ `nomi-core` — AI Execution Engine

The unified runtime that powers every AI operation in the ecosystem.

| | Responsibility | Detail |
| --- | --- | --- |
| 🔌 | LLM Abstraction | Gemini, OpenAI, Anthropic — unified interface |
| 🛡️ | Reliability | Retry logic and fault tolerance |
| ✅ | Validation | Structured output via Zod |
| 📊 | Observability | Per-user, per-feature cost tracking |

All AI providers are accessed exclusively through this layer —
ensuring consistency and full traceability across the system.

<br>

### 🧠 `nomi-biseo` — Personal AI Chief of Staff

The layer that truly knows the user — and acts on their behalf.

| | Capability | Detail |
| --- | --- | --- |
| 💾 | Persistent Memory | Retains context across all conversations |
| 🎯 | Personal Context | Goals, habits, preferences, ongoing projects |
| 🔍 | Semantic Retrieval | Surfaces the right memory at the right moment |
| 📋 | Task Delegation | Translates intent into structured work for nomi-company |
| 🔄 | Feedback Loop | Updates memory based on outcomes and approvals |

**`nomi-biseo`** is the CEO's only interface — it decides *what* needs to happen,
*how* it aligns with your goals, and *who* should do it.

**`nomi-core`** handles *how* the AI executes it.

<br>

### 🤖 `nomi-company` — AI Worker Team *(future)*

An organizational AI layer where specialized agents execute complex work —
managed entirely by nomi-biseo.

| | Capability | Detail |
| --- | --- | --- |
| 🧩 | Context Injection | Workers receive your personal context before every task |
| 🏢 | Departments | Design, Development, QA, and more |
| 📺 | Company Dashboard | Real-time visibility into worker activity (read-only) |
| 🔄 | Memory Feedback | Completed work updates biseo's understanding of you |

> The key insight: workers don't just execute tasks.
> They execute tasks knowing *who you are* — injected by nomi-biseo on every run.

<br>

---

## 📦 Repositories

| Repository | Purpose | Status |
| --- | --- | --- |
| `nomi-shared` | Shared types, schemas, and contracts | 🔨 Building |
| `nomi-core` | AI execution engine — NestJS microservice | 🔨 Building |
| `nomi-biseo` | Personal AI Chief of Staff | 📋 Planned |
| `nomi-company` | AI worker team and company dashboard | 🔮 Future |

<br>

---

## 🗺️ Roadmap

### Phase 1 — Foundation

Build the core AI infrastructure.

- [x] Ecosystem architecture
- [x] Repository structure
- [ ] `nomi-shared` — shared interfaces and schemas
- [ ] `nomi-core` MVP
  - Gemini adapter
  - Structured output validation
  - Cost tracking

### Phase 2 — Chief of Staff

Launch nomi-biseo — the personal AI that knows you.

- [ ] `nomi-biseo` MVP
- [ ] Authentication
- [ ] Conversational interface
- [ ] Memory system — persistent personal context
- [ ] Local development environment

**Deployment targets:**

| Service | Platform |
| --- | --- |
| `nomi-core` | Railway |
| `nomi-biseo` | Vercel |

### Phase 3 — The Company

Expand nomi-biseo's capabilities with a full AI worker team.

- [ ] `nomi-company` — multi-agent worker execution
- [ ] Context injection — biseo feeds personal memory into every worker
- [ ] Company dashboard — real-time visibility (read-only)
- [ ] Feedback loop — completed work updates biseo's memory
- [ ] Multi-LLM provider support
- [ ] Cost budgets and alerts

<br>

---

## 🚀 Getting Started

### Prerequisites

- [Docker](https://www.docker.com/) and Docker Compose
- A valid `GEMINI_API_KEY`

### Setup

```bash
git clone https://github.com/nomi-labs/nomi.git
cd nomi

cp .env.example .env
# Set your GEMINI_API_KEY in the .env file

docker compose up -d
```

### Services

| Service | Address |
| --- | --- |
| nomi-biseo | `http://localhost:3000` |
| nomi-core | `TCP localhost:4000` |
| PostgreSQL | `localhost:5432` |
| Redis | `localhost:6379` |

<br>

---

<br>

## 🛠️ Technology Stack

| | Layer | Technology |
| --- | --- | --- |
| 📝 | Language | TypeScript |
| 🏛️ | Framework | NestJS |
| 🤖 | AI SDK | Vercel AI SDK |
| 🌟 | LLM Provider | Google Gemini |
| 🔐 | Schema Validation | Zod |
| 🗄️ | Database | PostgreSQL + pgvector |
| ⚡ | Cache | Redis |
| 🐳 | Local Development | Docker Compose |

<br>

---

<br>

## 🧭 Design Principles

👔 **Chief of Staff Model** — The user always talks to biseo. biseo manages everything else.

🧠 **Memory First** — Context and personalization are first-class architectural concerns.

⚙️ **Single AI Engine** — One execution layer powers the entire ecosystem.

📈 **Persistent Intelligence** — The system becomes more capable the longer it is used.

🔭 **Full Observability** — Every AI request is traceable by user, feature, and cost.

🔄 **Provider Independence** — LLM providers can be swapped without touching product logic.

✨ **Simplicity for Users** — Complex infrastructure. Simple, personal experience. Just talk to Nomi.

<br>

---

<br>

<div align="center">

Built with intention by **nomi-labs**

</div>
