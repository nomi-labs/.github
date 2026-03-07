<div align="center">

<br>

# · nomi ·

### Personal intelligence that truly knows you.

*An open ecosystem building AI infrastructure that remembers,*
*learns, and grows more valuable with every conversation.*

<br>

</div>

---

## 💡 Why Nomi

Every AI assistant today starts from zero.
New conversation. No memory. No context. No continuity.

We believe this is the wrong model.

A personal AI should work the way a trusted collaborator does —
accumulating context over time, understanding your goals, and becoming
genuinely more useful the longer you work together.

> **Nomi is the infrastructure for that future.**

<br>

---

## 🏗️ The Ecosystem

Nomi follows a layered architecture. Each layer has one responsibility.

```
╔══════════════════════════════════════════╗
║           nomi-company  (future)         ║
║      Organizational AI  ·  Multi-Agent   ║
╠══════════════════════════════════════════╣
║               nomi-biseo                 ║
║          Personal AI Assistant           ║
║    Memory  ·  Goals  ·  Context          ║
╠══════════════════════════════════════════╣
║               nomi-core                  ║
║           AI Execution Engine            ║
║   LLM Adapters  ·  Retry  ·  Costs       ║
╚══════════════════════════════════════════╝
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

### 🧠 `nomi-biseo` — Personal AI Assistant

The product layer that understands the user.

| | Capability | Detail |
| --- | --- | --- |
| 💾 | Persistent Memory | Retains context across all conversations |
| 🎯 | Personal Context | Goals, habits, preferences, ongoing projects |
| 🔍 | Semantic Retrieval | Surfaces the right memory at the right moment |
| ✨ | Proactive Intelligence | Connects dots, spots patterns, follows up |

**`nomi-biseo`** decides *what* needs to happen.
**`nomi-core`** handles *how* the AI executes it.

<br>

### 🤖 `nomi-company` — Multi-Agent Intelligence *(future)*

An organizational AI layer where specialized agents collaborate
to perform complex reasoning, planning, and decision-making at scale.

<br>

---

## 📦 Repositories

| Repository | Purpose | Status |
| --- | --- | --- |
| [`nomi`](https://github.com/nomi-labs/nomi) | Ecosystem docs and local development | 🔨 Active |
| `nomi-shared` | Shared types, schemas, and contracts | 🔨 Building |
| `nomi-core` | AI execution engine — NestJS microservice | 🔨 Building |
| `nomi-biseo` | Personal AI assistant | 📋 Planned |
| `nomi-company` | Multi-agent AI layer | 🔮 Future |

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

🧠 **Memory First** — Context and personalization are first-class architectural concerns.

⚙️ **Single AI Engine** — One execution layer powers the entire ecosystem.

🔭 **Full Observability** — Every AI request is traceable by user, feature, and cost.

🔄 **Provider Independence** — LLM providers can be swapped without touching product logic.

✨ **Simplicity for Users** — Complex infrastructure. Simple, personal experience.

<br>

---

<br>

<div align="center">

Built with intention by **nomi-labs**

</div>
