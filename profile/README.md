<div align="center">

# Akirama

### Curriculum-aware soroban practice, built for correctness

Akirama turns proven soroban methodology into structured, reproducible, and
explainable mental-arithmetic practice.

</div>

## What we are building

Akirama is a learning platform for step-by-step mental arithmetic practice.
Exercises are generated from a server-owned curriculum, use only methods
available at the learner's current stage, and are independently validated
before they reach the learning experience.

The platform separates the learning product from the generation engine. The
customer experience is designed around learner profiles, sessions,
assignments, and progress, while a dedicated worker builds reproducible pools
of validated exercises from an immutable generator version.

## Product foundation

- **Curriculum-aware generation** — progressive addition and subtraction
  through Simple, Little Friends, Big Friends, and Family methods.
- **Deterministic exercises** — the same versioned configuration and seed
  produce the same result.
- **Independent validation** — generated chains are checked separately, with
  action- and digit-level explanations.
- **Safe Practice state** — learner, session, assignment, attempt, and pool
  data have explicit ownership, idempotency, and transaction boundaries.
- **Reproducible releases** — exercise pools are tied to immutable profiles,
  generator fingerprints, and validated release inputs.

## Current status

The implemented addition-and-subtraction engine covers one- to four-digit
exercises across 107 approved curriculum nodes. Its current v3 contract is
deterministic, versioned, independently validated, and packaged for use by the
Practice pool worker.

The independent Practice backend now includes its PostgreSQL persistence
foundation, learner and exercise-attempt models, transactional assignment
contracts, versioned product registry, canonical exercise profiles, generator
fingerprints, and deterministic release planning. The production deployment
foundation separates the protected operator Labs from the future customer API
and keeps Practice data inside its own service boundary.

The next delivery stages are the offline pool builder and quality gate,
customer session API and authentication, and the separate learner-facing web
application. Multiplication, division, and the broader production learning
experience remain future product work.

## Our principles

- **Pedagogy first** — confirmed learning rules take priority over convenient
  technical shortcuts.
- **Correct by design** — generation, validation, Practice state, and user
  experience have separate responsibilities.
- **Reproducible** — versioned contracts and deterministic randomness make
  exercises and releases repeatable.
- **Explainable** — every action can be traced back to the soroban method it
  uses.
- **Fail closed** — unverified generator artifacts, invalid exercises, and
  incomplete releases are never treated as production-ready.

## Technology

Akirama is being built with Python, FastAPI, SQLAlchemy, PostgreSQL,
TypeScript, Next.js, Docker, and Nginx.

The product source code is private and proprietary and is not distributed
under an open-source license.

---

We are building the platform in verifiable stages: from methodology and
generation, through validated exercise pools, to a complete learner
experience.
