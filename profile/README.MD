# 守護 SHUGO

### Cryptographic security infrastructure for autonomous agents on Solana.

**Shugo Protocol** is an open-source security infrastructure project building standards, protocols, and developer tools for autonomous agents operating with digital assets.

We believe autonomous agents should be able to **act on behalf of users without taking custody of their assets**.

Shugo separates **asset ownership** from **execution authority**, giving agents constrained, measurable, and revocable permissions instead of unrestricted access to private keys.

<p align="center">
  <a href="#">🌐 Website</a>
  ·
  <a href="#">📚 Documentation</a>
  ·
  <a href="#">📜 Specification</a>
  ·
  <a href="#">🛡️ Security</a>
</p>

---

## Why Shugo?

Autonomous agents are moving from generating information to **executing real transactions**.

That creates a fundamental security problem.

Giving an agent unrestricted access to a wallet means that a compromised prompt, malicious instruction, model error, or poisoned transaction can potentially become a direct loss of funds.

Traditional wallet delegation assumes the signer can be trusted.

**Autonomous agents require a different security model.**

Shugo introduces a policy-controlled execution layer between autonomous agents and the assets they operate.

```text
         ┌───────────────────┐
         │      USER / DAO   │
         │                   │
         │    Owns Assets    │
         └─────────┬─────────┘
                   │
                   │ Delegated Authority
                   ▼
         ┌───────────────────┐
         │   SHUGO PROTOCOL  │
         │                   │
         │  Policy Guardrails│
         │  • Allowlists     │
         │  • Velocity Caps  │
         │  • Spending Limits│
         │  • Revocation     │
         └─────────┬─────────┘
                   │
                   │ Permitted Execution
                   ▼
         ┌───────────────────┐
         │  AUTONOMOUS AGENT │
         │                   │
         │   Executes Tasks  │
         └───────────────────┘
```

### The principle is simple:

> **Agents get permission to act. They don't get ownership of what they control.**

---

# What We're Building

Shugo is an ecosystem of open-source infrastructure for secure agent execution.

### 🔐 Protocols

On-chain primitives that enforce execution policies and delegation boundaries.

### 🧩 SDKs & Developer Tools

Libraries and CLI tooling that allow developers to integrate guarded execution into existing agent architectures.

### 🤖 Agent Integrations

Infrastructure for connecting Shugo with autonomous agent frameworks, runtimes, and applications.

### 🔬 Formal Verification

Security-critical protocol logic designed with formal verification and mathematically defined invariants.

### 📚 Open Standards

Public specifications for secure delegation and autonomous-agent economies.

---

# Shugo Architecture

```text
┌──────────────────────────────────────────────────────────────┐
│                       AGENT ECONOMY                           │
│                                                              │
│   Autonomous Agents • Bots • AI Runtimes • Applications      │
└──────────────────────────────┬───────────────────────────────┘
                               │
                               ▼
┌──────────────────────────────────────────────────────────────┐
│                    SHUGO DEVELOPER LAYER                     │
│                                                              │
│        SDK • CLI • Plugins • Agent Integrations              │
└──────────────────────────────┬───────────────────────────────┘
                               │
                               ▼
┌──────────────────────────────────────────────────────────────┐
│                     SHUGO PROTOCOL                            │
│                                                              │
│   Delegation • Policy Enforcement • Allowlisting             │
│   Velocity Controls • Spending Limits • Revocation            │
└──────────────────────────────┬───────────────────────────────┘
                               │
                               ▼
┌──────────────────────────────────────────────────────────────┐
│                         SOLANA                                │
│                                                              │
│       Native Accounts • Programs • Transactions • CPI         │
└──────────────────────────────────────────────────────────────┘
```

---

# Core Principles

| Principle | What it means |
|---|---|
| **Zero Custody** | Shugo does not require users to deposit assets into custodial intermediary contracts. |
| **Least Authority** | Agents receive only the permissions required to perform their tasks. |
| **Deterministic Enforcement** | Security policies are enforced on-chain rather than relying on the agent's judgment. |
| **Revocable Execution** | Delegated authority can be restricted or revoked. |
| **Verifiable Invariants** | Security-critical state transitions and limits can be formally analyzed. |
| **Open Infrastructure** | Protocol specifications and developer tooling are built in the open. |

---

# The Shugo Ecosystem

Our repositories cover different layers of the stack:

```text
                     SHUGO PROTOCOL
                           │
          ┌────────────────┼────────────────┐
          │                │                │
          ▼                ▼                ▼
       Protocol          SDK / CLI       Integrations
          │                │                │
          ▼                ▼                ▼
     On-chain Guard    Developer APIs    Agent Runtimes
          │                │                │
          └────────────────┼────────────────┘
                           │
                           ▼
                     Documentation
                           │
                           ▼
                     Specifications
```

Explore the repositories below to see how each component fits into the broader Shugo ecosystem.

---

# Built for the Agentic Economy

The next generation of software will not only **read, reason, and recommend**.

It will:

- Move assets
- Execute trades
- Manage liquidity
- Interact with protocols
- Operate infrastructure
- Coordinate with other agents
- Make autonomous decisions

This requires a security layer designed specifically for machines acting with financial authority.

**Shugo is building that layer for Solana.**

---

# Open Source

Shugo Protocol is being developed in the open.

We welcome developers, security researchers, protocol engineers, and builders interested in the future of autonomous systems and cryptographic security.

```text
守護 · शुगो · SHUGO

Secure the authority.
Preserve the custody.
Enable the agent.
```

<p align="center">
  <sub>Open-source cryptographic infrastructure for autonomous agents on Solana.</sub>
</p>
