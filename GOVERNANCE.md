# A22 Governance Model (v0.1)

## 1. Governance Philosophy

The A22 standard is governed with three goals:
*   **Stability** — predictable evolution of the language
*   **Neutrality** — no single vendor controls the direction
*   **Velocity** — fast iteration without bureaucratic overhead

A22 uses a lightweight, open, and contributor-friendly process.

---

## 2. Roles

### 2.1 Steering Group (SG)

A small group of 3–7 experienced members responsible for:
*   Maintaining the A22 specification
*   Reviewing and approving A22 Improvement Proposals (AIPs)
*   Ensuring backward compatibility
*   Managing versioning and releases

The SG is not tied to any single company.

**Selection**
*   Initial members appointed by project founders
*   Future members elected by contributor vote (simple majority)
*   1-year renewable terms

**Removal**

Members may be removed by a 2/3 SG vote in cases of inactivity or conflict of interest.

---

### 2.2 Core Contributors

Contributors with sustained involvement (PRs, reviews, design input).

Responsibilities:
*   Drafting AIPs
*   Reviewing proposals
*   Discussing design decisions
*   Building reference tooling

Promotion requires majority SG approval.

---

### 2.3 General Contributors

Anyone in the community who:
*   Submits issues
*   Writes AIPs
*   Participates in discussions
*   Creates tooling or implementations

Open to all.

---

## 3. AIP Process (A22 Improvement Proposal)

AIPs govern the evolution of A22. Each follows these stages:

1.  **Draft**
    *   Contributor writes proposal in AIP format
    *   Posted publicly (GitHub)
2.  **Review**
    *   Core contributors and community comment
    *   SG assigns reviewers
3.  **Consensus**
    *   SG seeks consensus; if unclear → a vote
4.  **Approval**
    *   Requires simple majority SG vote
    *   For breaking changes: 2/3 SG approval
5.  **Release**
    *   Included in next A22 spec release
    *   Documentation updated

Transparency: all discussion, votes, and decisions are public.

---

## 4. Decision-Making

### 4.1 Consensus First

Decisions aim for broad agreement.

### 4.2 When to Vote

Voting is used when:
*   Consensus cannot be reached
*   Breaking changes are proposed
*   Governance changes are discussed

Voting rules:
*   Simple majority for regular changes
*   Two-thirds for breaking or structural changes

---

## 5. Releases & Versioning

A22 follows semantic versioning:
*   **MAJOR**: breaking changes
*   **MINOR**: new features, capabilities
*   **PATCH**: typo fixes, clarifications

Release cadence:
*   Major releases: not more than once per year
*   Minor releases: quarterly
*   Patch releases: as needed

SG is responsible for tagging and publishing.

---

## 6. Neutrality Rules

To ensure trust:
*   No single vendor may control more than 1/3 of SG seats
*   All official materials licensed under Apache 2.0
*   Runtimes may be proprietary, but must disclose non-compliance
*   A22 spec cannot depend on vendor-specific technology

---

## 7. Conflict Resolution

If disagreements persist:
1.  Attempt informal resolution
2.  Escalate to SG discussion
3.  Formal SG vote
4.  If still unresolved, an external neutral advisor may be invited (optional)

---

## 8. Amendments to Governance

Governance changes require:
*   A formal AIP
*   2/3 SG approval
*   Public documentation of changes

---

## Summary

This governance model ensures A22 is:
*   Open but not chaotic
*   Stable but not slow
*   Neutral but founder-led
*   Community-driven but not hijacked
