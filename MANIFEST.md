# Language-Driven Ontological Architecture (LDOA) — Manifest v1

## Epistemological Disclaimer

This architecture is rooted in the epistemology of the human being and the Ontology of Language, pioneered by Fernando Flores and Rafael Echeverría. Reading the foundational texts is not required to implement this architecture, but the core premise matters: language does not merely describe reality; it generates it.

In LDOA, “reality” refers to operational reality: the set of conditions, states, commitments, transitions, and valid acts that are recognized, declared, transformed, or made addressable within the system.

LDOA translates human cognitive coordination, speech acts, authority, promises, cognition, and the management of operational friction into a software architecture.

Terms such as Being, Situation, Judgment, Affirmation, Declaration, Breakdown, Listening, Speaking, and Reflecting are used as architectural translations of ontological distinctions. They should be read operationally, not psychologically or metaphysically.

## 0. Naming Convention

* **Architecture name:** Language-Driven Ontological Architecture
* **Acronym:** LDOA
* **Central ontological unit:** Being

A Being is an ontological-operational existence within the system. It is defined declaratively and operates with bounded autonomy. It should not be reduced to an entity, a microservice, an actor, or a role.

An entity can be identified. An actor can act. A role can describe responsibility. A Being exists operationally. It carries identity, promises, behavior, native faculties, cognition, learned capabilities, judgments, authority, and the ability to produce acts into a shared operational language.

A Being has a root identity. That identity is stable during the life of the Being. Descriptions, memory, capabilities, promises, and behavior may evolve under governance, but changing the root identity means creating another Being.

## 1. The Core Premise and Ontological Shift

The base assumption of this architecture is that systems do not merely store, synchronize, or process data. In classical IT, ontology is commonly used to describe an external reality. LDOA shifts that base.

Operational reality has primacy over infrastructure.

A database does not decide what occurred. A message bus does not decide what occurred. A component does not decide what occurred. Infrastructure records, transports, stores, executes, exposes, or fails to recognize aspects of operational reality. It does not command reality.

A Situation is not merely a technical event, message, request, or wrapper.

A Situation is operational reality expressed in language and context.

A declared Situation changes operational reality when authority exists.

An affirmed Situation observes, reports, or confirms operational reality without transforming it.

This distinction matters. A system may fail to record, transport, process, or recognize a Situation, but that failure does not automatically decide that the operational reality did not occur. It reveals another Situation: a missing record, a failed transport, an unavailable capability, an inconsistency, an insufficiency, or a Breakdown.

This is the ontological shift: LDOA does not begin with infrastructure. It begins with operational reality in language.

### Primacy of Operational Reality

If a sale has occurred, the sale has occurred.

If an operator with authority declares that three kilograms of potatoes were sold, that declaration constitutes operational reality in the sales domain. The fact that the product is not recognized by the inventory system does not erase the sale, nor should it retroactively prevent it.

The missing product reveals another operational condition: an insufficiency, inconsistency, or Breakdown in inventory, catalog, stock, integration, registration, or fulfillment.

That new condition must itself become addressable as a Situation.

In LDOA, a system does not deny operational reality because one component cannot recognize it. The architecture preserves the reality of the act and exposes the friction that prevents continuity.

A database may fail to record.
A bus may fail to transport.
A component may fail to recognize.
A capability may be unavailable.
A domain may lack the authority to transform what another domain has already validly declared.

None of those failures, by themselves, decide that the operational reality did not occur.

They produce new Situations that must be judged, handled, delegated, repaired, affirmed, or declared as Breakdowns.

This does not mean that every attempted act is valid. A Being may require preconditions before producing a valid Declaration. But once a valid operational act has been produced within its authority and domain, a later inconsistency in another component or domain does not erase that reality. It introduces another Situation.

### Core Movement

LDOA is organized around a simple architectural movement:

```text
Situation → Being(s) → Speech Act(s) → Operational Continuity
```

A Situation is operational reality expressed in language and context.

A Being listens to a Situation according to its promises, domain, context, cognition, behavior, and authority.

The Being may judge the Situation, exercise native Faculties, use acquired Capabilities, and produce a Speech Act.

That Speech Act may affirm, declare, or expose a Breakdown.

A produced Speech Act may itself become a new Situation for other Beings.

Operational continuity is therefore not a linear pipeline. It is a coordinated movement where Beings listen, judge, speak, and preserve or restore continuity across domains.

The purpose of this movement is operational continuity: to preserve, transform, restore, or make addressable the reality recognized by the system.

That is the central movement of the architecture.

## 2. Architectural Composition

LDOA is one architecture, but it is composed of several internal models. These models are not separate architectures; they describe different dimensions of the same architectural form:

* Behavior Model
* Faculty, Capability, and Cognition Model
* Judgment and Breakdown Model
* Speech Act Model
* Authority Model
* Common Communication Channel Model
* Unified Language Model
* Multi-Domain Context Model
* Metastructure Model

The architecture only makes sense when these models operate together. Speech Acts without Authority lack transformative force. Authority without Context is ambiguous. Context without a Unified Language collapses into local interpretation. Behavior without Promises becomes generic execution. Communication without a shared channel cannot coordinate Beings. Capabilities without Cognition become static mechanisms detached from adaptation. LDOA is the composition of those distinctions.

## 3. The Behavior Model

The Behavior Model separates business definition from physical execution.

### The Unified Event Schema: Situations

In this architecture, an “Event” is not limited to an asynchronous message from infrastructure such as Kafka or RabbitMQ. A REST API call, a webhook, a scheduled trigger, or a database trigger may carry Situations into the operational ecosystem.

The Unified Event Schema is the technical envelope through which a Situation may circulate. It is not the Situation itself.

A Situation is operational reality expressed in language and context. The schema exposes that Situation’s context, identity, data, and authority-relevant dimensions. The schema does not make every Being capable of acting. It only makes the Situation structurally available within the shared operational language.

Whether a Being can understand, judge, or act upon a Situation depends on its own declarative definition, promises, domain, authority, behavior, and cognition.

### The Being

A Being is defined through a declarative Domain-Specific Language (DSL) governed by the business. The DSL declares the Being’s identity, promises, behavior, native faculties, cognition, learned capabilities, judgments, and authority. The DSL is not the Being itself; it is the declarative structure through which the Being becomes operational.

A Being does not simply execute logic. It carries promises. A promise defines what the Being is committed to fulfill. An operational Being is not meaningful without promises, because without promises there is no responsibility to observe, judge, fulfill, or produce an act.

Behavior is the way the Being fulfills its promises when a Situation appears. Behavior belongs to the Being: it defines which Situations the Being attends, which promise is activated, which native faculties may be exercised, which learned capabilities may be used, which judgments may be emitted, and which acts may be produced.

An Accountant within this architecture is not an entity called Accountant. It is not an actor playing accountant. **The Being is the Accountant.** It interprets accounting Situations, exercises its native faculties, uses learned accounting capabilities, emits accounting Judgments, and produces accounting acts that may become valid Declarations when authority exists.

### The Executor

The Executor provides the infrastructure. It supplies CPU, memory, network, storage, event transport, and access to technical resources. It acts as a business-agnostic interpreter of the Being’s DSL.

The Executor contains no business logic. It holds no authority. It does not own context, decide behavior, or produce meaning. It gives physical execution to the ontological decisions established by the Being.

## 4. Faculty, Capability, and Cognition Model

In LDOA, a Faculty is not a generic technical capability. A Faculty is a native constitutive mode of operation shared by all Beings. Every Being is born with Faculties.

A Capability is different. A Capability is an acquired, learned, granted, or declared operational ability that allows a Being to fulfill a specific promise within a domain.

Faculties define *how* a Being can operate. Capabilities define *what* a Being has learned, acquired, or been granted to do.

Cognition is the internal domain where the Being preserves memory, distinctions, learned capabilities, judgment criteria, promise history, and observed fulfillment. Learning belongs to Cognition. It is not part of the native Faculty set. Learning is an adaptive cognitive capability that allows some Beings to acquire, refine, or update Capabilities under governance.

In conventional software architecture, a capability may refer to an API, a function, a permission, a feature, a module, or an organizational ability. In LDOA, that word is constrained. Capabilities are not native modes of operation. They are acquired operational abilities available to a Being for fulfilling promises.

A Being can observe. A Being can listen. A Being can speak. A Being can judge. A Being can reflect. **Those are native Faculties.**

An Accountant may acquire Reconciliation. A Support Being may acquire Incident Classification. An Operator may acquire the ability to initiate a specific operational flow. A Being may acquire the ability to read a ledger, call an API, parse a format, persist data, publish an event, or query a source. **Those are Capabilities.**

A Being does not outsource its responsibility when it uses a Capability. It may use infrastructure, connectors, resources, APIs, databases, queues, or external systems through acquired capabilities, but the meaning and responsibility of the action remain owned by the Being. If the Being is an Accountant and it has acquired the Capability of Reconciliation, the Executor may provide the database connection, but ontologically, the Accountant reconciles.

### Native Faculties

A Being is born with a minimal set of native Faculties. These are constitutive modes of operation:

* **Observing / Distinguishing:** Allows a Being to distinguish operational reality, including its own state, promise fulfillment, degradation signals, and relevant conditions. Observing is not passive perception; to observe is to distinguish reality through the language and cognition available to the Being.
* **Listening:** Allows a Being to attend incoming Situations. A Being does not listen to everything; it listens to what it needs to listen to in order to fulfill its promises, according to its context, behavior, and cognition.
* **Speaking / Producing:** Allows a Being to produce acts into the shared operational language of the system. Producing is the operational form of Speaking.
* **Judging:** Allows a Being to evaluate a Situation before acting.
* **Reflecting:** Allows a Being to observe itself over time: its pending promises, emitted Judgments, fulfillment level, memory, learned capabilities, and possible Breakdowns.

### Cognition and Learning

Cognition may evolve during the life of a Being. The root identity does not change. The Being may refine its memory, distinctions, learned capabilities, judgment criteria, and ways of fulfilling promises, but it remains the same Being only while its root identity remains stable.

Learning is a cognitive capability. It allows a Being to acquire, refine, or adjust Capabilities under governance. Learning does not mean arbitrary mutation. A Being learns within the boundaries of its promises, authority, Unified Language, and declarative definition. When a Being accepts or is granted a new promise, it may need to acquire new Capabilities, refine its Observing, adjust its Judging, or extend its behavior. The promise is not merely learned as a function; it becomes part of the Being’s responsibility under authority.

## 5. Common Communication Channel Model

A Being does not coordinate in isolation. Communication requires a shared medium.

The Common Communication Channel is the shared operational medium through which produced acts circulate and become available for other Beings to listen to. In a concrete implementation, this channel may be Kafka, an API, a queue, a webhook, or another shared communication mechanism.

The channel allows Beings to speak and listen. It does not, by itself, create meaning, authority, or validity. A Being may produce an act into the channel. Another Being may listen to that act if its promises, behavior, context, and cognition make that act relevant.

The channel transports communication. The Unified Language preserves meaning. Authority determines transformative force.

A channel may carry Situations produced through Affirmations, Declarations, Breakdowns, or other valid Speech Acts. What matters architecturally is not the transport mechanism, but the fact that Beings coordinate through a common communicational space.

## 6. Judgments and Breakdowns

LDOA reframes technical validations and exceptions as part of a broader operational judgment model. Before producing an act, a Being evaluates the Situation and emits a Judgment:

* **Judgment of Ignorance:** “The DSL lacks the configuration or cognition required to interpret this situation.”
* **Judgment of Insufficiency:** “The Situation is recognized, but its structure lacks the required data, context, authority, or capability to act.”
* **Judgment of Satisfaction:** “Conditions are met to proceed with the promise.”

### The Breakdown

When operational transparency is lost—because of missing context, degraded promises, insufficient data, technical friction, systemic uncertainty, or a missing Capability—the Being produces a Breakdown.

A Breakdown is not a fatal exception. It is a valid Speech Act that enters the ecosystem as a new Situation. It makes the friction addressable. A Breakdown can be handled by the same Being during a later Reflection, routed to a specialized Support Being, processed by AI, escalated to an operator, or passed into another operational layer.

### Resilience and Ontological Continuity

In many conventional architectures, a technical failure is treated primarily as an exception, timeout, retry, or infrastructure incident.

LDOA separates physical execution from ontological responsibility. The Executor acts as the physical body; the Being holds operational identity, promises, behavior, cognition, and authority.

A network timeout, a dead connection, or an unavailable dependency is not an ontological fatal error. It is a physical obstacle that breaks the transparency of normal operation.

When such a failure becomes observable, the Executor may translate it into a new Situation presented to the Being, such as: “The acquired capability is temporarily unavailable.”

The Being evaluates that Situation. If the obstacle affects its promise fulfillment, the Being may produce a Breakdown.

The Breakdown enters the Common Communication Channel as a new Situation. A separate Affirmation may report the physical condition, but the Breakdown is the act that makes the friction operationally addressable.

Just as a human accountant does not cease to exist when their calculator loses power, a Being does not lose its identity when infrastructure fails. The Being preserves its promises and continuity while the friction is routed, delegated, or handled by another Being, operator, or operational layer.

### Impeccability

A Being tracks its own Judgments. By observing its ratio of Satisfaction, Ignorance, and Insufficiency, the Being observes its own Impeccability: its level of fulfillment against its promises.

Impeccability is not moral purity. Operationally, it is promise fulfillment observed over time. If fulfillment degrades, Reflection may lead the Being to produce a higher-level Breakdown. This allows the system to surface degradation before it becomes invisible operational debt. Trust emerges from observed Impeccability over time.

## 7. Speech Act and Authority Models

System outputs are treated as acts of language. A Being has the Faculty of Speaking / Producing. It does not have a native Faculty called Declaring or Affirming. Affirmation and Declaration belong to the Speech Act Model. They describe what a produced act becomes within the shared operational language of the system.

* **Affirmation:** Observes, reports, or confirms operational reality. It does not transform operational reality and requires no transformative authority.
* **Declaration:** Transforms or constitutes operational reality. It creates a new condition and advances system continuity.

A Declaration requires Authority to be valid. Authority is not the same as RBAC; it is not simply a permission attached to a user or process. Authority is the ontological condition that gives a produced act transformative force.

Implicit authority exists when the following are aligned:

```text
Residence Domain == Operation Domain == Situation Domain
```

Authority may also be explicitly granted through the Being’s DSL. Without authority, an attempted Declaration has no transformative effect on operational reality. Depending on the Being’s definition, it may be treated as an Affirmation, rejected as invalid, or produced as a Breakdown.

A judge issuing a ruling in a courtroom performs a Declaration. The same individual saying the same words in a public square performs, at most, an Affirmation. The words may be identical. The authority is not. The reality produced is different.

An operator declaring a sale within the sales domain may produce a valid operational reality for Sales. Inventory, Accounting, Registration, or Fulfillment may each listen to that Situation according to their own promises and authority. If one of those domains fails, the sale does not disappear. The failure becomes another Situation.

## 8. Shared Meaning: Language and Context

Integration relies on shared meaning, not only on data exchange. The Unified Language Model establishes that Situations, Judgments, Breakdowns, Speech Acts, Authority, Promises, Faculties, Capabilities, Cognition, and Beings share the same semantic distinctions across the system. Without that language, messages may still move, endpoints may still respond, and workflows may still execute, but operational coherence collapses.

Context does not live in one central place:

* The **Situation Context** arrives with the Situation.
* The **Residence Context** defines where the Being lives and where its baseline legitimacy comes from.
* The **Operation Context** identifies where the behavior is being exercised.

A Being may live in one domain, operate in another, and attend Situations from multiple domains. Operating in a domain does not automatically grant authority to declare within it. Authority must be implicit through alignment or explicit through declaration in the DSL.

## 9. Metastructure

A Being alone may exist, but it does not operate in isolation. Operation requires interaction. The minimal operational unit of LDOA is:

```text
Situation + Being + Unified Language
```

The Situation is operational reality expressed in language and context. The Being provides identity, promises, behavior, native faculties, cognition, learned capabilities, Judgments, and authority. The Unified Language makes coordination possible across Beings and domains.

From this minimal unit, the architecture scales into multiple Beings, multiple domains, multiple operational layers, and multiple forms of responsibility. LDOA is not simply a collection of autonomous components; it is a metastructure where Beings coordinate through Situations, Judgments, Speech Acts, Cognition, and shared meaning.

Some responsibilities are fulfilled by specialized Beings. Registration, for example, is not a native Faculty of every Being. A Being may produce a Situation that requires registration, but the responsibility of recording belongs to a Being whose promise is to register.

## 10. Synthesis

The Language-Driven Ontological Architecture defines a way of designing systems around the structure of action and language.

The design does not begin with databases, services, APIs, or infrastructure. It begins with operational reality expressed as Situations and with Beings carrying responsibility through declarative definitions.

A Situation is operational reality in language and context. Beings listen, distinguish, judge, and produce acts. Cognition preserves memory and learned capabilities. A common channel allows Beings to coordinate. Breakdowns make friction addressable. Declarations, backed by Authority, transform or constitute the operational world.

Infrastructure executes the operations.
Language provides shared meaning.
The channel allows coordination.
Judgments evaluate Situations.
Cognition preserves and refines operational ability.
Valid acts move reality forward.

## 11. Author, Copyright & License

**Author:** Andres Silva Hormazabal.

**Year:** 2026

**Affiliation:** Sin Límites SpA

**Copyright & Licensing**

This document, *Language-Driven Ontological Architecture (LDOA) — Manifest v1*, is the original intellectual property of Andres Nicolas Silva Hormazabal.

It is licensed under the **Creative Commons Attribution 4.0 International License (CC BY 4.0)**.

To view a copy of this license, visit: https://creativecommons.org/licenses/by/4.0/

**Permissions & Attribution**

Under this license, you are free to:

* **Share:** Copy and redistribute the material in any medium or format.
* **Adapt:** Remix, transform, and build upon the material for any purpose, even commercially.

**Under the following terms:**

* **Attribution:** You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.

**Recommended Citation Format:**

> Silva Hormazabal, A. (2026). *Language-Driven Ontological Architecture (LDOA) — Manifest v1*. Sin Límites SpA. Licensed under CC BY 4.0.

