# A22 Contribution Guide (v0.1)

Thanks for wanting to contribute to A22 — the open standard for agentic systems.
This document explains how to propose changes, contribute code, report issues, and participate in shaping the language.

---

## 1. How to Contribute

You can contribute in four main ways:

**✅ 1. Propose improvements to the language**

Use the AIP (A22 Improvement Proposal) process for any change to the spec, syntax, semantics, or AST.

**✅ 2. Contribute to tooling**
*   Reference parser
*   Validator
*   VSCode extension
*   Documentation
*   Examples

**✅ 3. Report bugs or inconsistencies**
*   Spec issues
*   Runtime inconsistencies
*   Ambiguous grammar
*   Missing edge cases

**✅ 4. Join discussions**

Help clarify design decisions, argue trade-offs, or advocate for features.

---

## 2. Before You Start
*   Read the A22 Spec (latest version)
*   Browse open AIPs to avoid duplication
*   Search issues to see if your problem already exists
*   Join the community discussion channels (Discord/GitHub)

If you’re unsure whether your idea needs an AIP, open a small discussion issue first.

---

## 3. AIP Process

Changes to the A22 language follow the AIP process:
1.  Draft your proposal using the AIP template
2.  Submit it as a pull request under `/AIPs/AIP-XXX-title.md`
3.  Community reviews
4.  Steering Group evaluates
5.  Approval or revisions requested

Breaking changes require stricter review.

---

## 4. What Needs an AIP vs. What Doesn’t

**Use AIP for:**
*   New keywords or blocks (agent, tool, event, data, etc.)
*   Syntax or grammar changes
*   Semantic changes
*   New capability models
*   Language-level behaviors
*   Standard library additions
*   Anything affecting runtimes

**No AIP needed for:**
*   Typos
*   Documentation fixes
*   Example projects
*   VSCode extension updates
*   Reference runtime bug fixes
*   Minor clarification PRs

If unsure: ask. We will guide you.

---

## 5. Writing a Good AIP

A great AIP is:
*   Clear
*   Minimal
*   Backward-compatible where possible
*   Backed by real use cases
*   Consistent with A22 principles
*   Includes examples
*   Identifies alternatives

Follow the official AIP Template.

---

## 6. Code Contributions

**Branches**
*   `main`: stable, released content
*   `next`: upcoming changes
*   `drafts`: experimental, community draft work

**Steps**
1.  Fork the repo
2.  Create a feature branch
3.  Add tests if applicable
4.  Run formatting + linting
5.  Submit a PR with a clear description

**Coding Standards**
*   Keep code small and readable
*   Align with spec terminology
*   Avoid runtime-specific assumptions
*   Document new behavior
*   Add examples when modifying language-related code

---

## 7. Spec Changes Workflow

When modifying the spec:
1.  Update the relevant `.md` spec sections
2.  Update grammar definitions
3.  Update AST or IR schemas
4.  Provide migration notes if necessary
5.  Run consistency checks against reference parser
6.  Update changelog

---

## 8. Discussion & Decision-Making

Most design work happens in:
*   GitHub discussions
*   AIP PR threads
*   Community calls (optional)
*   Spec comment threads

Consensus is preferred.
If consensus can’t be reached, the Steering Group votes.

---

## 9. Code of Conduct

We follow a simple, universal rule:

**Be respectful, assume good intent, keep discussions technical.**

Harassment, personal attacks, or toxic behavior will lead to removal from the community.

---

## 10. Getting Started

Good first contribution ideas:
*   Fix typos in the spec
*   Add a simple example agent
*   Propose improvements to readability
*   Add grammar tests
*   Improve VSCode syntax highlighting
*   Document ambiguous parts of the language
*   Suggest better error messages for the validator

You don’t need deep agentic experience to contribute.

---

## 11. Contact

For help:
*   GitHub Issues
*   `#a22-spec` channel on Discord
*   Email (optional)
*   Office hours (monthly)

---

## 12. Final Notes

A22’s goal is to be the simplest, most composable declarative language for agents.
Your contributions help shape the future of agentic development.

Welcome to the community.
