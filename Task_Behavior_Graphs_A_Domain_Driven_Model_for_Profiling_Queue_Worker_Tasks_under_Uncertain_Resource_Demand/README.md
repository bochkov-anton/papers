# Task Behavior Graphs

Working paper:

**Task Behavior Graphs: A Domain-Driven Model for Profiling Queue Worker Tasks under Uncertain Resource Demand**

This repository contains the paper source, models, algorithms, manifests, schemas, case studies, and evaluation scaffolding.

## Core idea

Task profiling is not raw metrics collection. Queue worker tasks should be modeled through task-class-specific behavior graphs that connect intrinsic features, execution context, resource demand, worker occupancy, entropy, and operational risk.

## Structure

- `sections/` — main paper sections.
- `models/` — formal model fragments.
- `algorithms/` — pseudocode used by the paper.
- `manifests/` — example task behavior manifests and domain packs.
- `schemas/` — JSON/YAML schema drafts for manifests.
- `case-studies/` — detailed workload examples.
- `evaluation/` — reproducibility and evaluation scaffolding.
- `figures/` — figure sources and generated/final outputs.
- `tables/` — LaTeX tables.
- `appendices/` — supplementary material.
- `bibliography/` — references and related-work notes.
- `reviews/` — internal review material.
