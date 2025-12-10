<p align="center">
  <img src="https://img.shields.io/badge/v4.1.1-SKYNET--HARDENED-0a0a0a?style=flat-square&labelColor=1a1a2e" alt="version"/>
  <img src="https://img.shields.io/badge/status-production-10b981?style=flat-square" alt="status"/>
  <img src="https://img.shields.io/badge/license-MIT-6366f1?style=flat-square" alt="license"/>
</p>

<h1 align="center">
  <br>
  <code>U S F</code>
  <br>
</h1>

<p align="center">
  <strong>Unified Superintelligence Framework</strong><br>
  <sub>Recursive self-improvement for AI reasoning systems</sub>
</p>

<p align="center">
  <a href="#quick-start">Quick Start</a> •
  <a href="MASTER-SPECIFICATION.md">Specification</a> •
  <a href="#architecture">Architecture</a> •
  <a href="core/PRECISION-LEVELS.md">Precision Levels</a>
</p>

---

USF is a methodology framework that improves itself. It coordinates multiple analytical perspectives, calibrates reasoning depth to task requirements, and uses its own methodology to identify and fix its weaknesses.

The framework emerged from 5 iterative red-team cycles where USF analyzed USF—each cycle surfaced issues that were resolved before the next. What remains is a production-hardened system for structured reasoning.

## Quick Start

USF operates through four engines that run in sequence:

```
Input → Domain Detection → Expert Generation → Precision Selection → Verification → Output
```

**Precision levels** determine analytical depth:

| Level | Confidence | When to Use |
|:------|:-----------|:------------|
| PL1 | 80-85% | Exploration, brainstorming |
| PL2 | 85-92% | Standard analysis |
| PL3 | 92-97% | High-stakes decisions |
| PL4 | 97-99% | Security, critical systems |
| PL5 | 99%+ | Cryptographic, safety-critical |

Map these to reasoning commands:

```
think        → PL1-PL2
think_hard   → PL2-PL3
think_harder → PL3-PL4
ultrathink   → PL4-PL5
```

## Architecture

```
                              ┌─────────────────────────────────────┐
                              │          ORACLE-META                │
                              │    11 agents monitor + improve      │
                              │         the framework               │
                              └──────────────┬──────────────────────┘
                                             │
                    ┌────────────────────────┼────────────────────────┐
                    │                        │                        │
                    ▼                        ▼                        ▼
        ┌───────────────────┐    ┌───────────────────┐    ┌───────────────────┐
        │  DOMAIN ADAPTER   │    │ PRECISION ENGINE  │    │   VERIFICATION    │
        │                   │    │                   │    │                   │
        │  Detects domain   │    │  Selects depth    │    │  8 independent    │
        │  Generates expert │───▶│  Maps to PL1-5    │───▶│  chains validate  │
        │  perspectives     │    │  Calibrates rigor │    │  conclusions      │
        └───────────────────┘    └───────────────────┘    └───────────────────┘
```

**Oracle-Meta** is the self-evolution layer. It runs 11 specialized agents:

| Agent | Function |
|:------|:---------|
| MAL-COVERAGE | Detects blind spots in domain analysis |
| MAL-QUALITY | Assesses output against precision targets |
| MAL-EFFICIENCY | Optimizes resource usage |
| MAL-ADVERSARIAL | Red-teams conclusions |
| MAL-CONVERGENCE | Monitors consensus formation |
| MAL-CONTEXT | Manages context window budget |
| MAL-ERROR | Coordinates failure recovery |
| MAL-KNOWLEDGE | Preserves cross-session learning |
| MAL-TASK | Parallelizes independent operations |
| MAL-WORKFLOW | Orchestrates multi-phase analysis |
| MAL-NOVELTY | Tracks novel patterns for integration |

These agents operate in a 5-phase cycle: Monitor → Analyze → Propose → Validate → Integrate.

## Verification

Conclusions pass through 8 verification chains before finalization. Chains have weighted independence—if Chain F depends on Chain B's output, its agreement counts for 0.5× instead of 1.0×:

```
Chain A  Static Analysis     ████████████  1.0×
Chain B  Dynamic Testing     ████████████  1.0×
Chain C  Formal Methods      ████████████  1.0×
Chain D  Empirical Testing   ████████████  1.0×
Chain E  Expert Review       ████████████  1.0×
Chain F  TDD (depends: B)    ██████        0.5×
Chain G  Code Review         ████████████  1.0×
Chain H  Debug (depends: BF) ████          0.3×
```

Effective agreement = `Σ(independent × 1.0) + Σ(dependent × weight)`

## Expert Archetypes

Every analysis synthesizes 5 perspectives:

| Archetype | Role | Challenge Mode |
|:----------|:-----|:---------------|
| **TH** (Theorist) | Conceptual frameworks, first principles | "What assumptions are we making?" |
| **AD** (Adversarial) | Attack surface, failure modes | "How does this break?" |
| **IM** (Implementer) | Practical constraints, execution | "Can we actually build this?" |
| **QA** (Quality) | Edge cases, regression risks | "What did we miss?" |
| **ST** (Strategist) | Long-term implications, tradeoffs | "What are we optimizing for?" |

Convergence requires 4/5 archetype agreement at the target precision level.

## Limitations

USF is a reasoning methodology, not a knowledge base. It improves *how* analysis happens, not *what* is known.

Known constraints:
- Self-improvement cycles show diminishing returns after ~5 iterations
- PL5 (exhaustive) analysis is slow and rarely necessary
- The framework assumes good-faith engagement—adversarial prompt injection is out of scope
- Cross-session knowledge persistence requires external storage

## Files

| Path | Contents |
|:-----|:---------|
| [`MASTER-SPECIFICATION.md`](MASTER-SPECIFICATION.md) | Complete framework specification |
| [`core/PRECISION-LEVELS.md`](core/PRECISION-LEVELS.md) | Precision level definitions and selection criteria |
| [`core/EXPERT-ARCHETYPES.md`](core/EXPERT-ARCHETYPES.md) | Archetype behaviors and consensus rules |
| [`self-evolution/META-ANALYSIS-AGENTS.md`](self-evolution/META-ANALYSIS-AGENTS.md) | MAL agent specifications |
| [`precision/VERIFICATION-CHAINS.md`](precision/VERIFICATION-CHAINS.md) | Chain independence and weighting |
| [`integration/EXECUTION-FLOW.md`](integration/EXECUTION-FLOW.md) | Behavioral modes and execution model |

<details>
<summary><strong>All specification files</strong></summary>

**Core**
- [`core/DOMAIN-TAXONOMY.md`](core/DOMAIN-TAXONOMY.md) — Domain classification system
- [`core/PHASE-TEMPLATES.md`](core/PHASE-TEMPLATES.md) — Analysis phase templates

**Self-Evolution**
- [`self-evolution/IMPROVEMENT-PROTOCOL.md`](self-evolution/IMPROVEMENT-PROTOCOL.md) — Self-improvement process
- [`self-evolution/BOOTSTRAP-PROTOCOL.md`](self-evolution/BOOTSTRAP-PROTOCOL.md) — Framework initialization
- [`self-evolution/VERSION-LINEAGE.md`](self-evolution/VERSION-LINEAGE.md) — Version history and changes

**Precision**
- [`precision/PRECISION-CALIBRATOR.md`](precision/PRECISION-CALIBRATOR.md) — Automatic level selection
- [`precision/UNCERTAINTY-QUANTIFICATION.md`](precision/UNCERTAINTY-QUANTIFICATION.md) — Confidence calibration

**Integration**
- [`integration/CONVERGENCE-CRITERIA.md`](integration/CONVERGENCE-CRITERIA.md) — Multi-perspective consensus
- [`integration/EXAMPLE-ADAPTATIONS.md`](integration/EXAMPLE-ADAPTATIONS.md) — Domain adaptation examples

**Domain Adaptation**
- [`domain-adaptation/DOMAIN-DETECTOR.md`](domain-adaptation/DOMAIN-DETECTOR.md) — Automatic domain detection
- [`domain-adaptation/EXPERT-GENERATOR.md`](domain-adaptation/EXPERT-GENERATOR.md) — Dynamic expert generation
- [`domain-adaptation/CROSS-DOMAIN-TRANSFER.md`](domain-adaptation/CROSS-DOMAIN-TRANSFER.md) — Knowledge transfer patterns

</details>

## Development

USF 4.1.1 is the result of 5 self-analysis cycles:

| Cycle | Findings | Resolution |
|:------|:---------|:-----------|
| 1 | 18 issues (2 critical) | Core architecture fixes |
| 2 | 10 issues (0 critical) | Operational refinements |
| 3 | 5 issues | Polish |
| 4 | 14 issues (1 critical) | SKYNET integration analysis |
| 5 | 2 issues (low severity) | Final hardening |

Total: 20 improvements across 5 cycles. Remaining findings are low-severity edge cases with diminishing ROI to address.

## Contributing

See [`CONTRIBUTING.md`](CONTRIBUTING.md). Changes are validated through USF's own MAL agents before merge.

## License

MIT. See [`LICENSE`](LICENSE).

---

<sub>USF integrates patterns from the Claude ecosystem: Anthropic, SuperClaude Framework, VoltAgent, BeehiveInnovations, and community contributors.</sub>
