<div align="center">

# Akirama

### Thoughtful technology for better mental arithmetic learning

We are building a curriculum-aware learning platform that turns soroban
methodology into structured, reproducible, and explainable practice.

</div>

## What we are building

Akirama helps learners practise mental arithmetic step by step. Instead of
assembling random number chains, the platform follows a structured curriculum,
uses only methods the learner is ready for, and makes every generated exercise
independently verifiable.

Our current work focuses on the next generation of the Akirama learning engine:

- curriculum-aware soroban exercise generation;
- progressive paths through Simple, Little Friends, Big Friends, and Family;
- deterministic exercises that can be reproduced from the same seed;
- transparent validation with action- and digit-level explanations;
- a foundation for learner profiles, progress tracking, and accessible web
  experiences.

## Current focus

### Akirama Nextgen

Akirama Nextgen is our proprietary platform for curriculum-aware exercise
generation and mental arithmetic learning. Its source code is proprietary and
is not distributed under an open-source license.

The current implementation covers addition and subtraction across one- to
four-digit exercises. Multiplication, division, learner accounts, progress
tracking, and the production learning experience are planned.

## Our principles

- **Pedagogy first** — confirmed learning rules take priority over convenient
  technical shortcuts.
- **Correct by design** — generation and validation are separate, testable
  responsibilities.
- **Reproducible** — versioned contracts and deterministic randomness make
  exercises repeatable.
- **Explainable** — every action can be traced back to the soroban method it
  uses.
- **Built to evolve** — curriculum, applications, and infrastructure remain
  clearly separated.

## Technology

Akirama Nextgen is currently built with Python, FastAPI, TypeScript, Next.js,
and Docker.

---

We are at an early stage and actively shaping the product, curriculum, and
learning experience.
