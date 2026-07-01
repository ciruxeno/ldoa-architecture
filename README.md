# Language-Driven Ontological Architecture (LDOA)

**An architectural pattern in which situations from reality are attended by Beings operating within the ontological domain of language, maintaining operational continuity.**

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

> **Read the core specification:** [The LDOA Manifest v4](./MANIFEST.md)

---

## What This Repository Is

This repository presents **Language-Driven Ontological Architecture (LDOA)** as an architectural pattern.

It does not present a framework, product, library, runtime, workflow engine, or reference implementation.

A runtime may implement LDOA, but the runtime is not the pattern.

LDOA was distilled from implementation work, but this repository describes the architectural pattern itself: its distinctions, movement, rules, and examples.

---

## The Observation

People usually do not want to learn how software thinks in order to do their work.

A seller wants to sell.  
A warehouse operator wants to receive goods.  
A nurse wants to attend a patient.  
A business owner wants the business to keep moving.

They should not have to become inventory clerks, database operators, workflow experts, or integration specialists just to make their work acceptable to software.

LDOA exists to design systems that accept operational reality first, and then coordinate what must happen next.

---

## The Core Distinction

Traditional software solutions often treat business acts — a sale, a registration, a commitment, a delivery, a correction — as records, transactions, messages, or workflow steps.

This is technically convenient, but architecturally it confuses operational reality with its technical handling.

A definition is not the act.  
A schema is not the reality.  
An error is not the truth.  
A trace is not the responsibility.

When a system cannot record, transport, synchronize, validate, or process an act, the technical failure is often treated as if the operational act itself had not occurred.

LDOA separates those two things.

**The act and the technical handling of the act are not the same.**

If a sale occurred, the sale occurred.

If inventory cannot recognize the product, that does not erase the sale.  
If accounting cannot process the sale, that does not erase the sale.  
If registration fails, that does not erase the sale.

Those failures reveal new operational conditions.

Those conditions must be handled.

They should not deny reality.

---

## Operational Frictions

LDOA is easier to understand through the operational frictions it addresses.

### Product Not Recognized

A customer is at checkout with a physical product.

The product exists.  
The customer is willing to pay.  
The seller is performing the sale.

But the system says:

```text
Product not found.
```

In many traditional systems, that technical condition blocks the sale. The inventory system is treated as if it had authority to deny the operational act.

In LDOA, the failure to recognize the product does not erase the sale. It exposes another Situation: inventory could not recognize or reconcile the product.

That Situation may become a Breakdown and be attended by another Being.

The sale remains visible.  
The failure becomes addressable.  
Operational continuity is preserved.

### The Burden of Learning the System

A business owner may want to improve operations with software, but the system often forces the owner and workers to learn the internal logic of the software first.

They must learn screens, menus, validations, codes, roles, flows, and exceptions before their own work becomes acceptable to the system.

That burden is not neutral.

It first appears as mental load: the person must stop working in their own operational domain and start thinking in the categories of the software.

Over time, that mental load often becomes emotional load.

It appears in ordinary phrases such as:

```text
This does not work for me.
I am not an IT person.
This is complicated to learn.
This is unusable.
```

LDOA takes a different position: the system should listen to operational language and make it treatable, routable, judgeable, and continuable.

This does not mean that structure disappears.

It means the burden of structuring operational reality should belong to the architecture, not to the person doing the work.

For a deeper treatment of these examples, see [`concepts/operational_frictions.md`](./concepts/operational_frictions.md).

---

## Core Movement

LDOA is organized around this movement:

```text
Situation → Being(s) → Speech Act(s) → Operational Continuity
```

A **Situation** is operational reality expressed in language and context.

A **Being** attends Situations when they fall within its promise.

A **Speech Act** is what a Being produces into the shared operational language of the system.

A produced Speech Act may itself become a new Situation for other Beings.

**Operational Continuity** is the governing principle: to preserve, transform, restore, or make addressable the reality recognized by the system.

This is not a linear pipeline.

It is a coordination model.

---

## Essential Distinctions

LDOA uses a specific vocabulary. The following distinctions are enough to enter the pattern:

* **Situation** — operational reality expressed in language and context.
* **Being** — the ontological-operational unit that attends Situations and produces Speech Acts.
* **Promise** — what a Being is committed to fulfill; it determines what the Being may attend.
* **Authority** — the condition that gives a produced act transformative force within a domain.
* **Speech Act** — an act produced into the shared operational language.
* **Declaration** — a Speech Act that transforms or constitutes operational reality when authority exists.
* **Affirmation** — a Speech Act that observes, reports, confirms, coordinates, or leaves trace.
* **Breakdown** — a Speech Act that exposes operational friction as a new Situation.
* **Operational Continuity** — the preservation, transformation, restoration, or handling of operational reality.

Domains do not attend Situations.

Beings do.

The domain provides context and authority boundaries. The promise determines what a Being may attend.

For the fuller conceptual formulation, see [`concepts/ldoa_language.md`](./concepts/ldoa_language.md).

---

## Architecture Boundary

LDOA operates above any specific transport or execution mechanism.

It is not tied to Kafka, REST, queues, microservices, actors, webhooks, files, or scheduled triggers.

Those technologies may be used to implement LDOA, but they are not the architecture itself.

The channel transports communication.  
The Unified Language preserves meaning.  
Authority determines transformative force.

LDOA defines rules of operational coordination: how reality is expressed, attended, judged, declared, affirmed, broken down, delegated, and continued.

---

## When to Use LDOA

Use LDOA when operational meaning, authority, responsibility, and continuity matter more than simply completing a technical transaction.

LDOA is useful when business acts cross domains, when failures must remain visible, when authority matters, and when the system must preserve meaning instead of only moving data.

It may be unnecessary for simple CRUD applications, isolated scripts, prototypes, or small tools where operational meaning and continuity are not central concerns.

LDOA is not meant to make simple systems look sophisticated.

It is meant for systems where reality, responsibility, authority, and continuity are already complex.

---

## Repository Map

Current structure:

```text
ldoa-architecture/
├── README.md
├── MANIFEST.md
├── LICENSE
├── concepts/
│   ├── ldoa_language.md
│   └── operational_frictions.md
└── examples/
    ├── ldoa_example_flow_short_v1.0.md
    └── ldoa_example_flow_extended_v1.0.md
```

The repository is organized as follows:

* [`MANIFEST.md`](./MANIFEST.md) — the core specification and philosophical foundation of LDOA.
* [`concepts/ldoa_language.md`](./concepts/ldoa_language.md) — operational language concepts, including Beings, Promises, Authority, and Speech Acts.
* [`concepts/operational_frictions.md`](./concepts/operational_frictions.md) — real operational frictions that motivate the pattern.
* [`examples/ldoa_example_flow_short_v1.0.md`](./examples/ldoa_example_flow_short_v1.0.md) — a short walkthrough from human declaration to operational continuity.
* [`examples/ldoa_example_flow_extended_v1.0.md`](./examples/ldoa_example_flow_extended_v1.0.md) — an extended flow with more detail and visual structure.

---

## Current Status

This repository contains the current public formulation of LDOA.

The architecture is active and evolving. The [Manifest v4](./MANIFEST.md) captures its current and stable thesis.

The current concepts and examples provide an initial path for understanding the practical application of the pattern.

---

## License

**Language-Driven Ontological Architecture (LDOA)** is the original intellectual property of Andres Silva Hormazabal, Sin Límites SpA.

Licensed under the **Creative Commons Attribution 4.0 International License (CC BY 4.0)**.

You are free to share and adapt this material for any purpose, as long as appropriate credit is given. See the [LICENSE](./LICENSE) file for more details.
