# GitMedic

> Portable agent for reviewing basic Git repository hygiene through observable repository metadata.

## What it does

GitMedic checks whether a repository exposes a `.gitignore` and uses that evidence to identify a basic hygiene gap. The scope is intentionally small and deterministic.

### Diagnostic fingerprint

**Repository metadata → hygiene signal → evidence → action**

## Why this agent is distinct

GitMedic is not a Git tutor and not a full repository governance platform. It focuses on the small set of repository-level signals that can be evaluated without guessing about team practices.

That makes it a useful building block for larger developer-workflow agents.

## Workflow

```text
Git repository
    ↓
Metadata scanner
    ↓
Hygiene rule
    ↓
Evidence
    ↓
Improvement plan
```

## Verification

The repository contains:
- OpenGAP-compatible identity metadata
- Git-focused fixture coverage
- explainability and duty contracts
- four framework adapters
- automated adapter verification

OpenGAP validation passed and the four generated exports were exercised successfully.

## Design principle

**Repository hygiene should be inspectable.** GitMedic bases recommendations on visible repository structure rather than assumptions about how contributors work.

## Medic family

GitMedic shares the same portable passport model as the other Medic agents, but its diagnostic fingerprint is specifically about version-control hygiene.