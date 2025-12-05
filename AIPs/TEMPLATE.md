AIP-XXX: TITLE OF PROPOSAL

Author: Name + GitHub handle
Status: Draft / Review / Approved / Rejected / Deferred
Created: YYYY-MM-DD
Version: v0.1
A22 Version Target: e.g., 1.1 / 2.0 / unspecified

---

## 1. Summary

A short, 2–4 sentence description that explains what this proposal does, why it matters, and the intended outcome.

Example:
“This proposal introduces a new tool block that allows developers to define parameter schemas for agent tools declaratively.”

---

## 2. Motivation

Explain the problem:
*   What’s missing in the current A22 spec?
*   What use cases are blocked without this?
*   Why does this proposal need to exist?
*   Who benefits?

This should be user-facing and concrete.

---

## 3. Goals & Non-Goals

### Goals

List what the proposal aims to achieve.

### Non-Goals

List what it does not aim to do, to prevent scope creep.

---

## 4. Detailed Design

This is the heart of the proposal.

Include:
*   Syntax (new blocks, keywords, fields)
*   Semantics (how it behaves)
*   Grammar changes
*   AST/IR changes
*   Type or validation rules
*   Execution implications
*   Diagrams if relevant

Example Format:

```a22
tool "email_sender" {
    schema {
        to: string
        subject: string
        body: string
    }
    handler: external("send_email")
}
```

---

## 5. Examples

Provide several examples ranging from simple to complex.

Show:
*   Common usage
*   Edge-case usage
*   Integration with other A22 constructs

Examples help reviewers visualize the impact and validate correctness.

---

## 6. Rationale

Explain alternative designs you considered and why the chosen design is better.

You can mention:
*   Simplicity
*   Consistency with A22 principles
*   Backward compatibility
*   Alignment with future roadmap

---

## 7. Backward Compatibility

Address:
*   Is this a breaking change?
*   Does old A22 code continue working?
*   Do runtimes need to update?
*   Is there a migration strategy?

Breaking changes require stronger justification.

---

## 8. Security Implications

If relevant:
*   sandboxing
*   capability access
*   execution isolation
*   external tool safety

Otherwise: “No impact.”

---

## 9. Implementation Plan

Outline concrete steps:
*   Parser updates
*   LSP (VSCode) updates
*   Reference runtime updates
*   Documentation updates
*   Tests & validation rules

Who will implement what.

---

## 10. Open Questions

List unresolved issues where community input is needed.

---

## 11. Appendix (Optional)

Any extra details, diagrams, grammar expansions, or references.
