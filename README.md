# Northtek

**Agents should prove it, not claim it.** I build infrastructure for AI agents where every result carries its evidence: signed receipts for exactly what the model was shown, skills an agent has to prove before it remembers them, memory that refuses to surface a known-wrong fact, and benchmarks published even when they come out against me.

Independent research and engineering from Alaska. Systems work in Rust, tooling in TypeScript and Python. Client work at [northtek.io](https://northtek.io).

## Agent control and execution

- **[ghost](https://github.com/NORTHTEKDevs/ghost)** - verified control of the whole desktop for agents on Windows and Linux: apps with no API, windows, shell, browser. MCP server + CLI + REST API.
- **[kryos-lang](https://github.com/NORTHTEKDevs/kryos-lang)** - Kryos, a capability-safe systems language for trustworthy software and governed AI agents. Ecosystem: [kryos-mcp](https://github.com/NORTHTEKDevs/kryos-mcp) (capability-verified compile/run/audit over MCP), [kryos-mcp-pg](https://github.com/NORTHTEKDevs/kryos-mcp-pg) (Postgres MCP with per-table grants enforced before SQL hits the wire), [kryos-mcp-template](https://github.com/NORTHTEKDevs/kryos-mcp-template).

## Agent memory and verification

- **[genome](https://github.com/NORTHTEKDevs/genome)** - auditable memory layer for AI agents. Zero-LLM-call local ingest (~10ms/msg, air-gapped), bi-temporal belief state, MCP server, honest LoCoMo/LongMemEval benchmarks.
- **[praxis](https://github.com/NORTHTEKDevs/praxis)** - verified skill memory: your agent proves a skill works, then remembers it. Memory stores what you saw; Praxis stores what you proved.
- **[verified-memory](https://github.com/NORTHTEKDevs/verified-memory)** - agent memory that refuses to surface a wrong known fact: GENOME recall composed with a deterministic fact-verification gate.
- **[lossless-context-mcp](https://github.com/NORTHTEKDevs/lossless-context-mcp)** - a context ledger with cryptographically signed receipts of exactly which file versions the model was shown.
- **[overstory](https://github.com/NORTHTEKDevs/overstory)** - a knowledge tree of your codebase where every claim carries a verifiable receipt. Local-first.
- **[factgate](https://github.com/NORTHTEKDevs/factgate)** - a hallucination gate whose verdict is a comparison, not a judgement: parameter-free fact verification over a declared domain.

## Research

- **[rck](https://github.com/NORTHTEKDevs/rck)** - an auditable, hallucination-free alternative to LLMs for factual recall: 100k facts, sub-millisecond queries, one CPU thread, provenance and belief revision.
- **[rain](https://github.com/NORTHTEKDevs/rain)** - compositional generalization: exact symbolic composition plus learned selection reaches 100% SCAN / 99.75% COGS gen in seconds of CPU, with measured transformer and LLM baselines.
- **[sumerian-agent-patterns](https://github.com/NORTHTEKDevs/sumerian-agent-patterns)** - chunking signals tested against scribal ruling lines from 91,606 Sumerian tablets, then applied to git commit streams.
- **[lemmas](https://github.com/NORTHTEKDevs/lemmas)** - seven reliability primitives for any LLM API: chain-of-verification, self-consistency, best-of-N, reflexion, debate, drift detection, hedged execution.

## Developer tooling

- **[aiproof](https://github.com/NORTHTEKDevs/aiproof)** - ESLint for AI prompts: a Rust static analyzer for system prompts, templates, configs, and SDK call sites.
- **[claude-code-flywheel](https://github.com/NORTHTEKDevs/claude-code-flywheel)** - measures which Claude Code skills and agents actually earn their cost.
- **[evolve](https://github.com/NORTHTEKDevs/evolve)** - drop-in passive A/B evolution for AI coding assistants.

## How I publish

Every benchmark is reproducible from its repo, and negative results ship too. lossless-context-mcp reports its measured real-world token saving (-1.4%) next to the synthetic number. sumerian-agent-patterns withdrew two of its own claims under self-audit and lists four pre-registered refutations.

## Elsewhere

[northtek.io](https://northtek.io)
