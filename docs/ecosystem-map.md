# A22 Ecosystem Map

A strategic view of the A22 landscape — Wardley-style.

---

## Value Chain (Top to Bottom)

```
User Needs (Visible)
    ↓
Agentic Systems
    ↓
A22 Specification
    ↓
Runtime Implementations
    ↓
Infrastructure (Invisible)
```

---

## Evolution Axis (Left to Right)

```
Genesis → Custom → Product → Commodity
```

---

## The Map

```
                    Genesis         Custom          Product         Commodity
                    (Novel)       (Emerging)      (Mature)        (Ubiquitous)

User Needs
                                                    [Agentic AI Apps]
                                                          ↓

Application Layer                        [Multi-Agent Systems]
                                                ↓
                                      [RAG Systems]
                                                ↓
                                    [Conversational Agents]

Language/Spec                  [A22 Specification v3.0] ←──────────────┐
                                          ↓                             │
                                    [Grammar EBNF]                      │
                                          ↓                             │
                                  [Runtime Model]                       │
                                          ↓                             │

Runtime Layer              [Reference Runtime]                          │
                                    ↓                                   │
                          [Community Runtimes] ─────────────────────────┘
                                    ↓

Tooling                         [CLI Tools]
                                    ↓
                              [IDE Extensions]
                                    ↓
                            [Testing Frameworks]

Infrastructure                                         [Event Stores]
                                                            ↓
                                                    [LLM APIs]
                                                            ↓
                                                  [Cloud Platforms]
```

---

## Component Analysis

### User Needs → Agentic AI Applications (Product)

**Position:** Product
**Evolution:** Mature and growing
**Characteristics:**
- Customer support bots
- Research assistants
- Multi-agent workflows
- RAG systems

**Movement:** Rapidly commoditizing
**Inertia:** High (legacy code, established patterns)

---

### A22 Specification (Custom → Product)

**Position:** Custom moving toward Product
**Evolution:** Emerging standard
**Characteristics:**
- v3.0: Pure event ontology
- Natural language syntax
- Vendor-neutral
- Open specification

**Movement:** Moving right (toward product)
**Inertia:** Low (greenfield, clean design)

**Strategic Importance:** **Anchor**
- Defines how agentic systems are described
- Enables portability across runtimes
- Reduces vendor lock-in

---

### Runtime Implementations (Custom)

**Position:** Custom
**Evolution:** Early stage
**Characteristics:**
- Reference implementation (TypeScript)
- Community runtimes (multiple languages)
- Event-driven architectures
- Interpretation-based

**Movement:** Evolving rapidly
**Inertia:** Low (no legacy, clean interfaces)

**Strategic Opportunity:**
- Multiple implementations compete on performance
- No single runtime dominates
- Specification ensures compatibility

---

### Event Stores (Product → Commodity)

**Position:** Product moving to Commodity
**Evolution:** Mature technology
**Examples:**
- Kafka, Pulsar
- EventStoreDB
- Postgres with event sourcing
- DynamoDB streams

**Movement:** Commoditizing
**Strategic Note:** A22 is infrastructure-agnostic

---

### LLM APIs (Product)

**Position:** Product
**Evolution:** Rapidly maturing
**Examples:**
- OpenAI API
- Anthropic Claude
- Open-source models (Ollama)

**Movement:** Moving right (commoditizing)
**Strategic Note:** A22 abstracts over provider choice

---

### Cloud Platforms (Commodity)

**Position:** Commodity
**Examples:**
- AWS Lambda
- Cloudflare Workers
- Kubernetes
- Vercel/Netlify

**Movement:** Stable commodity
**Strategic Note:** A22 runtimes deploy anywhere

---

## Strategic Plays

### 1. Anchor on the Specification

**Why:**
The specification is the **durable asset**.

Runtimes will come and go.
LLMs will evolve.
Infrastructure will change.

The specification defines **what** agentic systems are.

**Move:**
- Keep specification minimal and stable
- Version carefully (semantic versioning)
- Evolve through community proposals (AIPs)

---

### 2. Enable Ecosystem through Simplicity

**Why:**
The simpler the specification, the more runtimes can be built.

**Move:**
- v3.0 reduces to 2 constructs (`system`, `agent`)
- Natural language syntax lowers barriers
- Runtime model is interpretation, not execution

**Result:**
- Many runtimes across languages
- Interoperability by design
- No vendor lock-in

---

### 3. Don't Compete on Infrastructure

**Why:**
Cloud platforms and event stores are commodities.

**Move:**
- A22 is infrastructure-agnostic
- Runtimes can use any event store
- Deploy to any cloud platform

**Result:**
- Users choose their own infrastructure
- A22 stays focused on specification
- No infrastructure lock-in

---

### 4. Abstract Over LLM Providers

**Why:**
LLMs are a fast-moving product category.

New models emerge constantly.
APIs change.
Pricing shifts.

**Move:**
- A22 doesn't prescribe LLM choice
- Agents declare capabilities, not models
- Runtimes handle provider integration

**Result:**
- Switch providers without rewriting specs
- Competition drives down costs
- Future-proof against model changes

---

### 5. Build Tooling Early

**Why:**
Developer experience drives adoption.

**Move:**
- CLI tools for running A22 programs
- IDE extensions for syntax highlighting
- Testing frameworks for validation
- Debugging tools for event tracing

**Result:**
- Fast feedback loops
- Easy onboarding
- Professional tooling from day one

---

## Evolutionary Pressure

### Forces Driving Commoditization

1. **LLMs** → More providers, lower costs, open-source alternatives
2. **Event Stores** → Mature, standardized, cloud-managed
3. **Infrastructure** → Serverless, edge computing, commodity platforms

### Forces Driving Differentiation

1. **Specification Design** → Simplicity, natural language, minimalism
2. **Runtime Innovation** → Performance, observability, debugging
3. **Ecosystem Growth** → Libraries, patterns, best practices

---

## Where A22 Wins

### 1. Portability

Write once, run on any runtime.
Switch infrastructure without rewriting.

### 2. Simplicity

Natural language syntax.
Two constructs: `system` and `agent`.
No boilerplate.

### 3. Clarity

Non-technical stakeholders can read specs.
No hidden behavior.
Transparent relationships.

### 4. Composability

Agents compose through events.
Systems emerge from relationships.
No orchestration code.

### 5. Durability

Specification is stable.
Runtimes evolve independently.
Future-proof against infrastructure changes.

---

## Wardley Doctrine Applied

### Pioneers, Settlers, Town Planners

**Pioneers (Genesis/Custom):**
- Runtime implementations
- Novel agent patterns
- Experimental tooling

**Settlers (Product):**
- Reference runtime (stabilize)
- CLI tools (productize)
- IDE extensions (scale)

**Town Planners (Commodity):**
- Documentation (standardize)
- Testing frameworks (commoditize)
- Best practices (codify)

### Movement Strategy

**For Specification:**
- Keep it minimal
- Resist feature creep
- Evolve through community proposals

**For Runtimes:**
- Let many bloom
- Compete on performance
- Converge on semantics

**For Ecosystem:**
- Encourage libraries
- Share patterns
- Build community

---

## Competitive Landscape

### A22 vs. Traditional Approaches

| Dimension | Traditional | A22 |
|-----------|------------|-----|
| Specification | Code (Python, JS) | Natural language DSL |
| Execution | Procedural | Event-driven |
| Portability | Language-locked | Runtime-agnostic |
| Readability | Technical only | Non-technical friendly |
| Evolution | Breaking changes | Stable primitives |
| Vendor Lock-in | High | None |

### A22 vs. Other DSLs

| DSL | Focus | Complexity | Portability |
|-----|-------|-----------|------------|
| LangChain | Python orchestration | High | Low |
| Semantic Kernel | .NET orchestration | Medium | Low |
| **A22** | **Natural language spec** | **Minimal** | **High** |

---

## Future Movements

### Short Term (6 months)

- Specification stabilizes (v3.0)
- Reference runtime matures
- CLI tools ship
- Community grows

### Medium Term (1-2 years)

- Multiple production runtimes
- IDE extensions for major editors
- Library ecosystem emerges
- Enterprise adoption begins

### Long Term (3-5 years)

- A22 becomes standard for agentic systems
- Specification evolves slowly (stability)
- Runtimes commoditize (compete on performance)
- Ecosystem thrives (tools, libraries, patterns)

---

## Summary

**A22's Position:**
- Anchor on specification (Custom → Product)
- Enable ecosystem through simplicity
- Abstract over infrastructure and LLMs
- Compete on clarity, portability, durability

**Strategic Advantage:**
- Natural language syntax lowers barriers
- Event-driven model enables composition
- Vendor neutrality prevents lock-in
- Minimal design ensures longevity

**Winning Move:**
- Keep specification simple and stable
- Let many runtimes compete
- Build tooling for developer joy
- Grow community through clarity

---

**A22** — Orchestrate agentic systems from natural language

The specification is the moat.
Simplicity is the strategy.
Community is the multiplier.
