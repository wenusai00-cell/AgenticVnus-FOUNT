<div align="center">

# Agentic Vnus — FOUNT

### *Source of All Intelligence*

**The next evolution of Agentic Vnus.**
Not a patch. Not a feature drop. A new foundation.

![Status](https://img.shields.io/badge/status-coming%20soon-FF4500?style=for-the-badge)
![Waves](https://img.shields.io/badge/waves-2-111111?style=for-the-badge)
![Features](https://img.shields.io/badge/features-9-FF4500?style=for-the-badge)
![License](https://img.shields.io/badge/local--first-always-000000?style=for-the-badge)

**⏳ Arriving in the next few days — coming directly to existing users.**

</div>

---

## ![](https://img.shields.io/badge/-COMPASS-FF4500?style=flat-square) What Is Fount?

Fount is built on one idea: **an agent should be trustworthy before it's powerful, and powerful without needing permission from a marketplace.**

Every feature below fits into one of two waves. Wave A makes the agent something you can trust completely — it explains itself, previews itself, and understands your world continuously. Wave B makes the agent something that scales — across teams, across tools, across other agents — without losing that trust.

```mermaid
flowchart LR
    A[User Command] --> B{Fount Core}
    B --> C[Wave A: Trust & Intelligence]
    B --> D[Wave B: Marketplace & Power]
    C --> E[Verified, Explainable Action]
    D --> F[Scaled, Routed Action]
    E --> G[Result]
    F --> G[Result]

    style B fill:#FF4500,stroke:#000,color:#fff
    style C fill:#111,stroke:#FF4500,color:#fff
    style D fill:#111,stroke:#FF4500,color:#fff
    style G fill:#FF4500,stroke:#000,color:#fff
```

---

## ![](https://img.shields.io/badge/WAVE_A-Trust_%26_Intelligence_Layer-FF4500?style=for-the-badge)

*Before an agent gets more power, it needs to earn more trust. Wave A is that foundation.*

### ![](https://img.shields.io/badge/01-CONSTITUTION-111111?style=flat-square&labelColor=FF4500) Agent Constitution

A fixed, persistent set of rules the agent cannot act outside of — not a prompt, not a setting, a **constitution**. Every action the agent takes is checked against it before execution, not after.

Instead of trusting the model to "remember" to be safe, the Constitution sits underneath the model as a non-negotiable boundary layer. It defines what the agent is always allowed to do, always forbidden from doing, and what always requires your explicit approval — regardless of how a command is phrased or what the AI reasons its way into.

```mermaid
flowchart TD
    A[Agent wants to act] --> B{Check against<br/>Constitution}
    B -->|Within bounds| C[Proceed]
    B -->|Requires approval| D[Ask User]
    B -->|Forbidden| E[Blocked — Always]
    D -->|Approved| C
    D -->|Denied| E

    style B fill:#FF4500,stroke:#000,color:#fff
    style E fill:#8B0000,stroke:#000,color:#fff
    style C fill:#228B22,stroke:#000,color:#fff
```

---

### ![](https://img.shields.io/badge/02-PREVIEW-111111?style=flat-square&labelColor=FF4500) Simulation / Preview Mode

Before running a risky or irreversible action, the agent shows you **what would happen** — not just what it plans to do in words, but a real preview of the outcome. See the diff before the commit. See the file list before the delete. See the changed state before it's changed.

This turns every meaningful action into a dry-run first, real-run second workflow — without slowing down the safe, everyday commands that don't need it.

```mermaid
sequenceDiagram
    participant U as User
    participant A as Agent
    participant S as Simulation Engine

    U->>A: "Delete old project files"
    A->>S: Run dry simulation
    S-->>A: Preview: 47 files, 2.3GB, list attached
    A->>U: Shows preview + Approve/Deny
    U->>A: Approve
    A->>A: Executes for real
```

---

### ![](https://img.shields.io/badge/03-WORLD_MODEL-111111?style=flat-square&labelColor=FF4500) Continuous World Model

The agent doesn't re-scan your system from scratch every time you give it a command. It keeps a **live, continuously updated model** of your files, apps, browser state, and recent activity — so it already knows the context the moment you type.

This is the difference between an agent that has to "look around" every time, and one that already knows where things are, what changed, and what you were doing five minutes ago.

```mermaid
flowchart LR
    A[File System] --> W[Continuous World Model]
    B[Open Apps] --> W
    C[Browser State] --> W
    D[Recent Actions] --> W
    W --> E[Instant Context<br/>for Every Command]

    style W fill:#FF4500,stroke:#000,color:#fff
    style E fill:#228B22,stroke:#000,color:#fff
```

---

### ![](https://img.shields.io/badge/04-PERSONALIZATION-111111?style=flat-square&labelColor=FF4500) Local Personalization

![](https://img.shields.io/badge/status-coming%20soon-FF4500?style=flat-square)

The agent adapts to **you specifically** — your phrasing, your file structures, your habits — and it does so entirely on-device. No profile sent anywhere, no personalization-as-a-service. Your patterns stay exactly where they were learned: your machine.

Built on top of the Continuous World Model, this is one of the first systems of its kind available anywhere — local, private, per-user adaptation with zero cloud involvement. It's already working, and it will keep getting sharper with every update.

---

### ![](https://img.shields.io/badge/05-INTER--AGENT_PROTOCOL-111111?style=flat-square&labelColor=FF4500) Inter-Agent Protocol

![](https://img.shields.io/badge/status-coming%20soon-FF4500?style=flat-square)

Your agents stop being isolated. With the Inter-Agent Protocol, the Agentic Vnus running on **one of your PCs can talk directly to the Agentic Vnus running on another one of your PCs** — coordinating tasks, sharing context, and working together across machines, without any cloud server sitting in the middle.

Practically, this means your agent on your desktop can hand off a task to your agent on your laptop, check on its progress, or simply have a conversation with it to sync up — all peer-to-peer, all private.

This is one of the first systems of its kind to exist — there's nothing quite like it in the market yet. It's launching in its early form now, and it will keep getting more capable with every update that follows.

```mermaid
flowchart LR
    subgraph PC1["Your PC #1"]
        A1[Agentic Vnus Agent]
    end
    subgraph PC2["Your PC #2"]
        A2[Agentic Vnus Agent]
    end

    A1 <-->|Peer-to-peer<br/>Talk & Collaborate| A2

    style A1 fill:#FF4500,stroke:#000,color:#fff
    style A2 fill:#FF4500,stroke:#000,color:#fff
```

---

## ![](https://img.shields.io/badge/WAVE_B-Marketplace_%26_Universal_Power-FF4500?style=for-the-badge)

*Once an agent can be trusted, it should be able to scale — across tools, teams, and other agents.*

### ![](https://img.shields.io/badge/06-CONFIG_SHARING-111111?style=flat-square&labelColor=FF4500) Config-Level Agent + Team Sharing

Share an entire agent setup — skills, permissions, memory scope, tool access — as a single portable config file. A teammate imports it and gets the exact same agent behavior instantly, without rebuilding it from scratch.

```mermaid
flowchart LR
    A[Your Agent Config] -->|Export| B[.vnus config file]
    B -->|Share| C[Teammate]
    C -->|Import| D[Identical Agent<br/>Same Skills & Permissions]

    style B fill:#FF4500,stroke:#000,color:#fff
    style D fill:#228B22,stroke:#000,color:#fff
```

---

### ![](https://img.shields.io/badge/07-TOOL_ROUTER-111111?style=flat-square&labelColor=FF4500) Universal Tool Router — MCP → Macro → Live Reasoning

The agent doesn't reason from scratch for every task. When a command comes in, it checks — in order — whether an MCP tool already handles it, whether a saved macro/skill already solves it, and only falls back to full live reasoning if neither exists. Fastest path first, always.

```mermaid
flowchart TD
    A[Command Received] --> B{MCP Tool<br/>Available?}
    B -->|Yes| C[Use MCP Tool<br/>Fastest]
    B -->|No| D{Saved Macro<br/>Exists?}
    D -->|Yes| E[Run Macro<br/>Fast]
    D -->|No| F[Live Reasoning<br/>Full Think]
    F --> G[New Macro Saved<br/>for Next Time]

    style C fill:#228B22,stroke:#000,color:#fff
    style E fill:#FF4500,stroke:#000,color:#fff
    style F fill:#8B0000,stroke:#000,color:#fff
    style G fill:#111,stroke:#FF4500,color:#fff
```

This is what makes the agent get **faster the more it's used** — every live-reasoning solve becomes a macro, every macro becomes near-instant next time.

---

### ![](https://img.shields.io/badge/08-MCP_ASSIGNMENT-111111?style=flat-square&labelColor=FF4500) Per-Agent Separate MCP Assignment

Not every agent instance needs every tool. Fount lets you assign a **different set of MCP servers to each agent** — a coding agent gets GitHub and terminal tools, a research agent gets browser and search tools, a personal agent gets calendar and email — each scoped to exactly what it needs, nothing more.

```mermaid
flowchart TD
    R[Fount Router] --> A1[Coding Agent]
    R --> A2[Research Agent]
    R --> A3[Personal Agent]

    A1 --> M1[GitHub MCP]
    A1 --> M2[Terminal MCP]

    A2 --> M3[Browser MCP]
    A2 --> M4[Search MCP]

    A3 --> M5[Calendar MCP]
    A3 --> M6[Email MCP]

    style R fill:#FF4500,stroke:#000,color:#fff
```

---

### ![](https://img.shields.io/badge/09-CAPABILITY_DIRECTORY-111111?style=flat-square&labelColor=FF4500) Boss Agent Data Symmetry — Capability Directory

When you're running multiple agents, one **Boss Agent** maintains a live directory of what every other agent can do — its tools, its skills, its current state. No agent is a black box to the system; the Boss always knows who can do what, so it can route tasks to the right agent instead of guessing.

```mermaid
flowchart TD
    B[Boss Agent] -->|Reads capabilities| D[(Capability Directory)]
    D --> A1[Agent 1: GitHub, Terminal]
    D --> A2[Agent 2: Browser, Search]
    D --> A3[Agent 3: Calendar, Email]

    U[Incoming Task] --> B
    B -->|Routes based on capability| A1
    B -->|or| A2
    B -->|or| A3

    style B fill:#FF4500,stroke:#000,color:#fff
    style D fill:#111,stroke:#FF4500,color:#fff
```

---

## ![](https://img.shields.io/badge/-ROADMAP-FF4500?style=flat-square) Roadmap Overview

| Wave | Feature | Focus | Status |
|---|---|---|---|
| A | Agent Constitution | Trust boundary layer | Coming Soon |
| A | Simulation / Preview Mode | Pre-action safety | Coming Soon |
| A | Continuous World Model | Live context awareness | Coming Soon |
| A | Local Personalization | On-device adaptation | Coming Soon |
| A | Inter-Agent Protocol | Cross-device agent collaboration | Coming Soon |
| B | Config-Level Sharing | Team-wide agent configs | Coming Soon |
| B | Universal Tool Router | MCP → Macro → Reasoning | Coming Soon |
| B | Per-Agent MCP Assignment | Scoped tool access | Coming Soon |
| B | Boss Agent Capability Directory | Multi-agent orchestration | Coming Soon |

<div align="center">

**All 9 features are arriving together, in the next few days.**

</div>

---

## ![](https://img.shields.io/badge/-CORE_IDEA-FF4500?style=flat-square) The Core Idea

```mermaid
flowchart LR
    T[Trust First] --> P[Then Power]
    P --> S[Then Scale]

    style T fill:#FF4500,stroke:#000,color:#fff
    style P fill:#111,stroke:#FF4500,color:#fff
    style S fill:#000,stroke:#FF4500,color:#fff
```

Every feature above exists to answer one question in order: **can you trust it, can it act, can it scale** — never the reverse.

---

<div align="center">

**Built by Prince Tanwar — Founder, Agentic Vnus**

*Your assistant. Your machine. Your rules.*

</div>