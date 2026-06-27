# Language-Driven Ontological Architecture (LDOA)
> **The architecture is active and evolving.**
> The current release focuses on the architectural manifest and the core conceptual structure.
 
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

An architectural pattern in which situations from reality are attended by Beings operating within the ontological domain of language, maintaining operational continuity.

LDOA starts from a simple observation:

People usually do not want to learn how software thinks in order to do their work.

A seller wants to sell.  
A warehouse operator wants to receive goods.  
A nurse wants to attend a patient.  
A business owner wants the business to keep moving.

They should not have to become inventory clerks, database operators, workflow experts, or integration specialists just to make their work acceptable to software.

LDOA exists to design systems that accept operational reality first, and then coordinate what must happen next.

## Pattern Intent

LDOA defines a way to model systems as ecosystems of **Situations**, **Beings**, **Speech Acts**, **Judgments**, **Authority**, and **Operational Continuity**.

Its intent is to prevent software infrastructure from becoming the authority over reality.

A database may fail to record.  
A message bus may fail to transport.  
A component may fail to recognize.  
A capability may be unavailable.

None of those failures, by themselves, decide that the operational reality did not occur.

Instead, those failures become new Situations that can be judged, delegated, repaired, affirmed, or declared as Breakdowns.

## Context

Many software solutions force users to adapt their work to the internal logic of the system.

The user is asked to follow the screen, satisfy the validation, understand the inventory model, wait for synchronization, or stop their work because a component failed.

In those systems, the software becomes the center of the operation.

LDOA takes the opposite position:

> The system should support operational reality.  
> Operational reality should not be reduced to what the system was able to record.

## The Problem

Traditional software solutions treat business acts — a sale, a registration, a commitment, a delivery, a correction — as records, transactions, or messages.

This is technically convenient, but architecturally it confuses operational reality with its technical definitions, schemas, errors, and traces.

A definition is not the act.  
A schema is not the reality.  
An error is not the truth.  
A trace is not the responsibility.

When the system cannot record, transport, synchronize, or process the act, the technical failure is often treated as if the operational act itself had not occurred.

LDOA separates those two things.

The act and the technical handling of the act are not the same.

If a sale occurred, the sale occurred.

If inventory cannot recognize the product, that does not erase the sale. It reveals another operational condition: inventory could not recognize the product, stock may be inconsistent, registration may have failed, or a capability may be unavailable.

That condition must be handled.

It should not deny reality.

## Forces

LDOA is useful when these forces appear together:

- users need to continue working even when infrastructure is imperfect;
- operational acts cross several domains;
- each domain has its own responsibility and authority;
- failures should become visible and addressable;
- technical consistency is important, but should not be confused with operational truth;
- the system must preserve meaning, not only move data.

The pattern exists because these forces are usually mixed together inside services, workflows, databases, queues, validations, and user interfaces.

LDOA separates them.

## Core Movement

LDOA is organized around this movement:

```text
Situation → Being(s) → Speech Act(s) → Operational Continuity
```

A **Situation** is operational reality expressed in language and context.

A **Being** listens to Situations according to its promises, domain, authority, context, cognition, and behavior.

A **Speech Act** is what a Being produces into the shared operational language of the system. It may affirm reality, declare a new reality, or expose a Breakdown.

A produced Speech Act may itself become a new Situation for other Beings.

**Operational Continuity** is the goal: to preserve, transform, restore, or make addressable the reality recognized by the system.

This is not a linear pipeline. It is a coordination model.

## Minimal Example

A seller declares:

> “I sold three kilograms of potatoes.”

If the seller has authority in the sales domain, that declaration constitutes operational reality for Sales.

From there, other Beings may listen:

- the Sales Being continues the sale;
- the Inventory Being updates or evaluates stock;
- the Accounting Being performs the accounting work;
- the Registration Being records the trace.

Each Being operates in its own domain, with its own promises and authority.

If Inventory cannot recognize the product, the sale does not disappear.

If Accounting fails, the sale does not disappear.

If Registration fails, the sale does not disappear.

Those failures become new Situations that must be judged, handled, delegated, repaired, or declared as Breakdowns.

## Pattern Structure

LDOA is composed of several internal models:

- **Behavior Model** — defines how a Being fulfills its promises when a Situation appears.
- **Faculty, Capability, and Cognition Model** — separates native modes of operation from acquired abilities and internal memory.
- **Judgment and Breakdown Model** — makes evaluation and operational friction explicit.
- **Speech Act Model** — defines how produced acts affirm, declare, or expose Breakdowns.
- **Authority Model** — defines when a produced act has transformative force.
- **Common Communication Channel Model** — defines the shared medium through which acts circulate.
- **Unified Language Model** — preserves shared meaning across domains.
- **Multi-Domain Context Model** — separates residence, operation, and situation contexts.
- **Metastructure Model** — describes how multiple Beings coordinate through Situations and Speech Acts.

These models are not separate architectures. They are dimensions of the same pattern.

## Core Distinctions

LDOA uses a specific vocabulary:

- **Situation** — operational reality expressed in language and context.
- **Being** — the core ontological-operational unit of the architecture.
- **Promise** — what a Being is committed to fulfill.
- **Faculty** — a native constitutive mode of operation shared by all Beings.
- **Capability** — an acquired, learned, granted, or declared operational ability.
- **Cognition** — the internal domain where a Being preserves memory, distinctions, judgment criteria, and learned capabilities.
- **Judgment** — the evaluation a Being makes before producing an act.
- **Speech Act** — an act produced into the shared operational language.
- **Affirmation** — observes, reports, or confirms operational reality.
- **Declaration** — transforms or constitutes operational reality when authority exists.
- **Breakdown** — exposes operational friction as a new Situation.
- **Authority** — the condition that gives a produced act transformative force within a domain.
- **Common Communication Channel** — the shared medium where produced acts circulate.
- **Operational Continuity** — the preservation, transformation, restoration, or handling of operational reality.

## Core Ontology and Environments

LDOA separates the ontology of the architecture from the environments where it may operate.

A Being’s identity, promises, cognition, authority, and behavior are environment-agnostic.

They belong to the core ontology of the architecture.

What changes across environments is not the Being itself, but the way its Faculties are expressed through infrastructure.

In an event-driven environment, Listening may be expressed through subscribers, and Speaking / Producing may be expressed through producers.

In an API-driven environment, Listening may be expressed through endpoints, and Speaking / Producing may be expressed through responses, callbacks, or client calls.

The Being remains the same.

Its Faculties do not change ontologically; they are expressed through different operational media.

## When to Use LDOA

Use LDOA when the system must preserve operational meaning across domains, responsibilities, authority boundaries, and technical failures.

It is especially useful when:

- business acts must remain visible even if infrastructure fails;
- several domains react to the same operational reality;
- authority matters;
- promises and responsibilities must be explicit;
- failures must become addressable instead of disappearing into logs;
- continuity matters more than simple request-response processing;
- the system must coordinate people, software, and operational domains.

## When Not to Use LDOA

LDOA may be unnecessary for simple CRUD applications, isolated scripts, prototypes, or small tools where operational meaning, authority, and continuity are not central concerns.

If the problem is only data storage, simple automation, or basic request-response processing, LDOA may add unnecessary conceptual overhead.

LDOA is not meant to make simple systems look sophisticated.

It is meant for systems where reality, responsibility, authority, and continuity are already complex.

## Consequences

LDOA makes responsibility explicit.

That is useful, but it has a cost.

Domains must be named.  
Promises must be declared.  
Authority must be modeled.  
Breakdowns must be handled.  
Speech Acts must be distinguished.  
Operational continuity must be designed deliberately.

The pattern does not remove complexity. It moves complexity into explicit architectural distinctions.

That is the tradeoff.

## What LDOA Is Not

LDOA is not a database pattern.

It is not a messaging framework.

It is not a workflow engine.

It is not tied to Kafka, REST, queues, microservices, actors, or any specific infrastructure.

Those technologies may be used to implement LDOA, but they are not the architecture itself.

LDOA defines the rules of operational coordination: how reality is expressed, listened to, judged, declared, affirmed, broken down, delegated, and continued.

## Repository Map

This repository contains the current public formulation of LDOA.

Current structure:

```text
LDOA/
├── README.md
├── manifest.md
└── LICENSE
```

The current release focuses on the architectural manifest and the core conceptual structure of LDOA.

Planned structure:

```text
LDOA/
├── core-ontology/
│   ├── domains/
│   │   ├── sales/
│   │   └── accounting/
│   │
│   ├── unified-language/
│   │   ├── situations/
│   │   └── speech-acts/
│   │
│   └── metastructure/
│
├── environments/
│   ├── event-driven/
│   │   ├── faculty-impl/
│   │   └── coordination.md
│   │
│   └── api-driven/
│       ├── faculty-impl/
│       └── coordination.md
│
├── examples/
├── diagrams/
├── concepts.md
├── architecture.md
└── evolution.md
```

The `core-ontology/` directory will contain the stable architectural distinctions: domains, Situations, Speech Acts, and metastructure rules.

The `environments/` directory will describe how those distinctions may be expressed through different technical media, such as event-driven or API-driven systems.

## Planned Work

The initial public release focuses on the architectural manifest and the core conceptual structure of LDOA.

The following artifacts are currently being prepared:

- [ ] `core-ontology/` — Formalization of domain models, Situation models, and Speech Act schemas.
- [ ] `environments/event-driven/` — Design patterns for asynchronous implementations.
- [ ] `examples/` — Walkthrough of the Sales-to-Accounting operational flow.

Contributions and discussions on these topics are welcome.

## Current Status

This repository contains the initial public formulation of LDOA.

The architecture is active and evolving. The manifest captures its current thesis; future examples, diagrams, and implementation notes may refine the model over time.

## License

Language-Driven Ontological Architecture (LDOA) — Manifest v1 is the original intellectual property of Andres Silva Hormazabal, Sin Límites SpA.

Licensed under the **Creative Commons Attribution 4.0 International License (CC BY 4.0)**.

You are free to share and adapt this material for any purpose, as long as appropriate credit is given. See the [LICENSE](./LICENSE) file for more details.
