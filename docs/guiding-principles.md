# A22 Guiding Principles

A22 is built on a small set of principles that ensure the language remains clear, composable, and durable. These principles guide both the design of the specification and the evolution of the ecosystem around it.

---

## 1. Clarity Over Abstraction

Every construct in A22 must be immediately interpretable.

The language favors explicitness and readability over abstraction layers or clever patterns.

**If something is unclear, it is redesigned.**

---

## 2. Intent Before Mechanics

A22 models **what** the system is meant to accomplish, not **how** it will be executed.

Execution details belong to runtimes; intent belongs to the language.

---

## 3. Minimalism as Power

The language includes only the primitives required for agentic systems—nothing more.

Features are added only when they reduce complexity at scale.

**A22 grows by subtraction, not accumulation.**

---

## 4. Uniformity Across Constructs

Every block in A22 follows the same structural rules: named, scoped, explicit, and declarative.

When two constructs look similar, they behave similarly.

When they differ, the difference is intentional.

---

## 5. Predictability Without Exceptions

There should be no "special cases" in the language.

The meaning of a construct must not change based on hidden rules or context-specific magic.

**Predictability ensures trust.**

---

## 6. Data Is Immutable Context

All data flows in one direction—forward.

State transitions create new context snapshots rather than modify existing ones.

This makes reasoning deterministic and debugging transparent.

---

## 7. Composition Over Control Flow

A22 models systems as composable relationships, not as procedural instructions.

A system is built by composing agents, contexts, tools, and flows—not by scripting control logic.

Composition reduces cognitive load and improves maintainability.

---

## 8. Human-Readable, Machine-Rigid

A22 must be pleasant to read and strict to parse.

Whitespace, block structure, and naming conventions exist to serve both humans and machines.

**Readable by anyone, reliable for everyone.**

---

## 9. Runtime Agnostic by Design

A22 programs must execute identically across runtimes.

The language specification defines behavior; runtimes implement it faithfully.

Portability ensures longevity.

---

## 10. Stability With Space to Evolve

The core primitives of A22 should remain stable over time.

Evolution happens through extensions, proposals, and optional capabilities—not breaking changes.

**Stability enables a healthy ecosystem.**

---

## 11. Transparent Intentionality

A22 avoids implicit behavior.

Every dependency, transformation, and flow relationship should be declared.

**If the reader must guess, the language has failed.**

---

## 12. Systems as First-Class Concepts

A22 treats agentic systems as structured, long-lived artifacts.

The language emphasizes:
- Declarative architecture
- Explicit capabilities
- Predictable data evolution
- Repeatable behavior

**Systems should feel designed, not improvised.**

---

## In Practice

These principles manifest in concrete design decisions:

- **Clarity**: Keywords like `can`, `use`, `when` make intent explicit
- **Intent**: Workflows describe dataflow, not execution order
- **Minimalism**: Only five primitives (Event, Context, Agent, Workflow, Tool)
- **Uniformity**: All blocks use the same indentation-based structure
- **Predictability**: Same context + same input = same output, always
- **Immutability**: Append-only events, never mutate
- **Composition**: Agents compose into workflows, workflows compose into systems
- **Human-Readable**: Natural language syntax (`agent "name" can chat, search`)
- **Runtime Agnostic**: Specification defines behavior, not implementation
- **Stability**: v1.0 specification is stable, extensions are opt-in
- **Transparent**: All dependencies, capabilities, and flows are declared
- **Systems-First**: Define the architecture, not just the code

---

## Evolution of Principles

These principles may be refined over time through the **A22 Improvement Proposal (AIP)** process, but they serve as the foundation for all design decisions in A22.

Any proposed change to the language must align with these principles, or demonstrate why a principle itself needs refinement.
