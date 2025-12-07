# A22 Guiding Principles

A22 orchestrates agentic systems from natural language.

These principles guide everything we build.

---

## 1. Clarity Over Abstraction

Every line of A22 should be immediately understandable.

We favor explicitness over cleverness.
We favor natural language over symbols.
We favor intent over mechanics.

**If someone has to guess, we failed.**

---

## 2. Intent Before Mechanics

A22 describes **what** a system does, not **how** it runs.

```a22
agent "assistant"
    knows how to chat
    listens to message.received
    speaks message.reply
```

The runtime figures out execution.
You describe intent.

---

## 3. Minimalism as Power

A22 has exactly **two constructs**: `system` and `agent`.

Everything else emerges from event relationships.

**We grow by subtraction, not accumulation.**

---

## 4. Uniformity Across Constructs

Every block follows the same rules:
- Named
- Scoped
- Declarative
- Natural language

When two things look similar, they behave similarly.
When they differ, the difference is intentional.

---

## 5. Predictability Without Exceptions

No special cases.
No hidden rules.
No context-dependent magic.

```a22
when message.received
    the system should eventually speak support.complete
```

This means exactly what it says. Always.

---

## 6. Everything Is Temporal

The unit of truth is **an event happening in time**.

History grows forward.
Nothing mutates.
State is computed, not stored.

---

## 7. Composition Over Control Flow

Systems are built by composing relationships, not scripting procedures.

```a22
agent "assistant"
    listens to message.received
    speaks retrieval.request

agent "retriever"
    listens to retrieval.request
    speaks retrieval.done

agent "assistant"
    listens to retrieval.done
    speaks answer.generated
```

No orchestration code. The flow emerges.

---

## 8. Human-Readable, Machine-Rigid

A22 reads like structured thought.

Non-technical people can understand what a system does.
Machines can parse it without ambiguity.

**Readable by anyone. Reliable for everyone.**

---

## 9. Runtime Agnostic by Design

A22 programs execute identically across runtimes.

The specification defines behavior.
Runtimes implement it faithfully.

This ensures portability and longevity.

---

## 10. Stability With Space to Evolve

Core primitives remain stable.

Evolution happens through:
- Extensions (opt-in)
- Proposals (community-driven)
- Capabilities (runtime-specific)

**Not breaking changes.**

---

## 11. Transparent Intentionality

A22 avoids implicit behavior.

```a22
agent "assistant"
    knows how to chat
    is not allowed to execute_code
    listens to message.received
    looks at message.* history
    interprets intent from message.* history
```

Every dependency is declared.
Every capability is explicit.
Every relationship is visible.

---

## 12. Systems as First-Class Concepts

Agentic systems are structured, long-lived artifacts.

They should feel **designed, not improvised**.

```a22
system "support"
    description: "customer support system"
    ensures "all messages receive replies within 5 minutes"

agent "assistant"
    knows how to chat
    listens to message.received
    speaks message.reply

when message.received
    the system should eventually speak support.complete
```

Architecture is explicit.
Guarantees are enforced.
Behavior is predictable.

---

## In Practice

These principles manifest in concrete design:

### Clarity
Keywords like `knows how to`, `listens to`, `speaks` — reads like English.

### Intent
Describe what agents do, not how they execute.

### Minimalism
Only `system` and `agent`. Everything else emerges.

### Uniformity
All blocks use indentation-based natural language structure.

### Predictability
Same events + same histories = same outputs. Always.

### Temporal
Events flow forward in time. Append-only. Immutable.

### Composition
Agents compose through event subscriptions, not orchestration.

### Human-Readable
Natural language syntax flows like thought.

### Runtime Agnostic
Specification defines behavior. Implementations vary.

### Stability
v3.0 primitives are stable. Extensions are opt-in.

### Transparent
All relationships declared. No implicit behavior.

### Systems-First
Define architecture, guarantees, and constraints.

---

## Evolution

These principles may evolve through the **A22 Improvement Proposal (AIP)** process.

But they are the foundation.

Any proposed change must:
1. Align with these principles
2. Or demonstrate why a principle needs refinement

---

## Why These Principles Matter

**Clarity** ensures adoption.
**Intent** enables portability.
**Minimalism** reduces cognitive load.
**Uniformity** makes learning instant.
**Predictability** builds trust.
**Temporality** enables reasoning.
**Composition** scales naturally.
**Human-readability** democratizes AI.
**Runtime agnosticism** ensures longevity.
**Stability** enables ecosystems.
**Transparency** prevents surprises.
**Systems-first** thinking builds quality.

---

**A22** — Orchestrate agentic systems from natural language
