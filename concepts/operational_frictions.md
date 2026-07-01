# LDOA Operational Frictions v1.0

## Purpose

This document collects real operational frictions that motivate **Language-Driven Ontological Architecture (LDOA)**.

These examples are not implementation requirements.

They are entry points for understanding why LDOA separates operational reality from the technical handling of that reality.

The README introduces these frictions briefly. This document gives them more space without overloading the main entry point of the repository.

This is the initial public version of this conceptual note.

---

## 1. Product Not Recognized

### Situation

A customer is at checkout with a physical product.

For example, a customer brings a drink to the cashier.

The drink exists.  
The customer is present.  
The seller is ready to sell.  
The exchange can occur.

But when the cashier scans the product, the system says:

```text
Product not found.
```

This happens in small shops, retail stores, warehouses, and large enterprise systems.

The physical reality and the technical representation of that reality are no longer aligned.

### Traditional Handling

In many systems, the inventory or product catalog becomes the practical authority over the sale.

If the product is not recognized, the sale is blocked.

The cashier must stop the operation, call a supervisor, wait for a product correction, create an exception, or abandon the sale.

The system behaves as if the product not being recognized meant that the operational act cannot exist.

The technical definition becomes stronger than the operational reality.

### LDOA Reading

LDOA separates the operational act from the technical handling of the act.

The fact that the product is not recognized by the inventory system does not erase the sale.

The fact that accounting cannot process the sale does not erase the sale.

The fact that registration fails does not erase the sale.

Those failures reveal new operational conditions.

In LDOA, the sale may remain a valid operational Situation, while the inventory failure becomes another Situation.

For example:

```text
Breakdown:
The product involved in the sale could not be recognized by inventory.
```

That Breakdown may be attended by an Inventory Being, a Registration Being, a Support Being, a Recovery Being, or another Being whose promise includes attending that type of Situation.

The important point is:

```text
The failure becomes addressable.
It does not silently deny reality.
```

### Architectural Distinction

This example exposes the core distinction of LDOA:

```text
Operational act ≠ technical handling of the act
```

A schema is not the reality.

A database record is not the act.

A validation error is not the truth.

A trace is not the responsibility.

---

## 2. The Burden of Learning the System

### Situation

A business owner wants to improve operations with software.

The owner may not understand systems, databases, workflows, permissions, menus, or technical exception handling.

That should not be surprising.

The owner understands the business.

The worker understands the work.

The seller understands the sale.

The nurse understands the patient.

The warehouse operator understands the receiving of goods.

But traditional software often asks the user to learn the internal structure of the system before the system can accept the work.

The user must learn how the software thinks.

### Traditional Handling

Traditional software often shifts the burden of structuring reality onto the user.

The user must learn:

```text
screens
menus
mandatory fields
codes
validations
roles
flows
states
exceptions
```

The person is moved away from their operational domain and pushed into the system’s domain.

The user becomes a translator between reality and software.

That burden is not merely usability friction.

It first appears as mental load: the user has to remember, interpret, search, infer, and translate the work into the system’s categories.

Over time, that mental load may become emotional load.

It appears in ordinary phrases such as:

```text
This does not work for me.
I am not an IT person.
This is complicated to learn.
This is unusable.
```

At that point, the software is no longer perceived as support.

It is perceived as another problem to manage.

This changes who carries the responsibility for making reality acceptable to the system.

### LDOA Reading

LDOA does not require reality to begin as a database-ready structure.

A human may express operational reality in language.

The system may then make that expression treatable, routable, judgeable, and continuable.

For example, a person may say:

```text
I sold 3 kilograms of potatoes.
```

The system does not create the sale.

The system makes the declaration treatable and routable.

Interpretation may extract an actionable structure.

Operation / Business may make that structured Situation available for attention.

A Being may attend it if it falls within its promise.

A Speech Act may then be produced.

### Clarification About Cognition

It may be tempting to say that traditional software forces the user to mutate their Cognition in order to think like the system.

In LDOA terms, that statement should be handled carefully.

**Cognition**, in LDOA, is the internal structural anchor of a Being. It should not be treated as an arbitrary mutable attribute.

The more precise formulation is:

```text
Traditional software imposes mental load on the user by forcing the user to translate operational reality into the system’s internal categories.

When that mental load accumulates, it may become emotional load and rejection of the system.
```

That rejection is usually expressed in practical language:

```text
This does not work for me.
I am not an IT person.
This is complicated to learn.
This is unusable.
```

LDOA does not remove the need for structure.

It relocates the responsibility for producing structure.

The person should remain closer to their operational domain.

The architecture should assume more of the burden of interpreting, routing, judging, and continuing the Situation.

### Architectural Distinction

This example exposes another core distinction of LDOA:

```text
The system should support operational language.
The user should not be forced to become the system’s adapter.
```

The goal is not to eliminate structure.

The goal is to avoid forcing the human operator to carry the architecture’s structural burden.

---

## 3. Relation to the Example Flows

These frictions explain why the pattern is needed.

The example flows show how LDOA handles a concrete Situation once operational reality has been expressed.

Read next:

* [`examples/ldoa_example_flow_short_v1.0.md`](../examples/ldoa_example_flow_short_v1.0.md)
* [`examples/ldoa_example_flow_extended_v1.0.md`](../examples/ldoa_example_flow_extended_v1.0.md)

The current example flows show this movement:

```text
Human Declaration
→ System Mediation
→ Structured Situation
→ Operation / Business Contextualization
→ Being Attention
→ Declaration, Affirmation, or Breakdown
→ Operational Continuity
```

This is not:

```text
message → process → register → notify
```

It is:

```text
situation → attention → Speech Act → new attendable situation → continuity
```

The examples are intentionally simple.

Their purpose is to show the pattern, not to prescribe one runtime, one transport, or one implementation technology.

---

## 4. Summary

LDOA addresses operational frictions where software systems confuse technical handling with operational reality.

Two recurring cases are:

```text
A technical system cannot recognize what operationally occurred.

A human is forced to translate operational reality into the system’s internal categories.
```

In both cases, LDOA preserves the same architectural position:

```text
Operational reality comes first.

Technical failure becomes an addressable Situation.

The system coordinates continuity instead of denying reality.
```
