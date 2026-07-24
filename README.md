# Harry Levis

Making COBOL → Java modernization measurable. Built and documented in public.

> LLMs made the translation cheap. Proving the translation is correct is the expensive part —
> and that proof is the actual deliverable.

## Home Lab

| | |
|---|---|
| **Agent** | Claude Agent SDK (Python) · MCP · OpenTelemetry |
| **Legacy side** | GnuCOBOL · JCL · copybooks · fixed-length records |
| **Target side** | JDK 17 · Spring Boot 3 / Spring Batch 5 · BigDecimal |
| **Infra** | Ubuntu 22.04 · Docker · SQLite task queue · GitHub Actions |

## Roadmap

- [ ] **P0** Async agent runway — task queue, budget circuit breaker, unattended batch runs
- [ ] **P1** COBOL internals — COMP-3, REDEFINES, rounding semantics: where translation breaks
- [ ] **P2** **Equivalence harness** — GnuCOBOL as oracle, schema-driven data generation, field-level diff, exposed as an MCP server ★
- [ ] **P3** **AWS CardDemo batch migration** — end-to-end, with proven equivalence ★
- [ ] **P4** **Migration playbook** — Skill suite + quantitative evaluation on 100–200 public COBOL programs ★
- [ ] **P5** Open source — contributing corpora and evals to Zorse (Linux Foundation / Open Mainframe Project)
- [ ] **P6** Commercial tooling landscape — IBM Bob, AWS Transform, Fujitsu PROGRESSION vs. a self-built pipeline

**Two engines, on purpose:** a deterministic Python loop for measurement (single variable, no filesystem access), and the Claude Agent SDK for the engineering work. A measuring instrument has to be simpler than the thing it measures.

*Everything runs on public open-source assets only.*

## Links

📝 Build log: [[Levis's COBOL-to-Java Modernization Blog]  ](https://harry-levis-ai-agent.hatenablog.com/)
