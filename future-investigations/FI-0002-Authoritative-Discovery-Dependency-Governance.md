# FI-0002 — Authoritative Discovery Dependency Governance

**Status:** Deferred  
**Origin:** FD-0023 — Authoritative Discovery Dependency Standing  
**Deferred:** 2026-08-30

---

## Question

How should authoritative dependencies upon Accepted Forge Discoveries be
represented, verified, maintained, and governed when those dependencies
conflict or when the standing of a depended-upon finding is later challenged?

---

## Why Deferred

The investigation of FD-0023 required determining when a Forge Discovery
finding may serve as an authoritative dependency in Stage engineering.

That investigation established that authoritative dependency standing arises
only after a Discovery has acquired the canonical standing conferred by valid
Canonical Discovery Acceptance.

Once that boundary was established, additional governance questions became
visible concerning:

- how Stage engineering represents reliance upon an Accepted Discovery;
- how authoritative dependency standing is verified;
- what happens when Accepted Discoveries materially conflict; and
- what governance applies when new evidence later undermines an Accepted
  finding upon which engineering work depends.

Resolution of those questions was not demonstrated to be necessary to establish
the authority condition required for a Discovery finding to serve as an
authoritative dependency.

They were therefore deferred rather than extending FD-0023 into a complete
dependency-governance system.

This investigation is preserved for future work and is not presently blocking
the engineering work that exposed it.

---

## Preserved Findings

### Authoritative Dependency Standing

A Forge Discovery finding may serve as an authoritative dependency in Stage
engineering only after the Discovery has acquired the canonical standing
conferred by valid Canonical Discovery Acceptance.

That standing permits Stage engineering to rely upon the Accepted finding as an
established Discovery premise within the finding's established scope and
limitations without independently re-establishing the finding each time it is
used.

---

### Artifact Existence

The existence of a Discovery artifact does not establish authoritative
dependency standing.

Therefore:

    Artifact Existence ≠ Authoritative Dependency Standing

---

### Hold Standing

A Discovery in Hold does not possess authoritative dependency standing merely
because it is a governed Discovery candidate.

Therefore:

    Hold ≠ Authoritative Dependency Standing

---

### Forge Survival

Survival of Forge investigation does not itself establish authoritative
dependency standing.

Therefore:

    Forge Survival ≠ Authoritative Dependency Standing

---

### Anvil Survival

Survival of Anvil inspection does not itself establish authoritative dependency
standing.

Therefore:

    Anvil Survival ≠ Authoritative Dependency Standing

---

### Epistemic Eligibility

Epistemic eligibility is necessary to the Canonical Discovery Acceptance
process but does not itself establish authoritative dependency standing.

Therefore:

    Epistemic Eligibility ≠ Authoritative Dependency Standing

---

### Scope of Reliance

Authoritative dependency standing does not make an Accepted finding universally
applicable.

Reliance remains bounded by the established scope and limitations of the
Accepted finding.

Stage engineering may rely upon the finding as an established Discovery premise
only where that reliance remains within those bounds.

---

### Re-establishment

Valid authoritative dependency standing permits Stage engineering to rely upon
an Accepted finding without independently re-establishing that finding every
time it is used.

This does not eliminate the need to determine whether the finding actually
applies to the engineering dependency in which it is being invoked.

Therefore:

    Authoritative Standing ≠ Universal Applicability

---

## Unresolved Questions

This Future Investigation preserves the following unresolved questions:

1. How should Stage engineering represent an authoritative dependency upon an
   Accepted Forge Discovery?

2. How should the authoritative standing of a depended-upon Discovery be
   verified?

3. What information must be preserved with an authoritative dependency to
   identify the exact Accepted finding, its scope, limitations, and applicable
   canonical state?

4. What governance applies when two or more Accepted Discoveries materially
   conflict?

5. How should existing engineering dependencies be treated when new evidence
   materially undermines an Accepted finding?

6. How should changes to the canonical standing of a depended-upon Discovery
   propagate, if at all, to Stage specifications or implementations that relied
   upon it?

These questions are preserved without assuming that every one requires a
separate Forge Discovery, Stage specification, or governance mechanism.

---

## Re-entry Condition

Reopen this investigation only when a concrete Forge–Stage engineering
operation requires representation or verification of an authoritative
Discovery dependency, encounters a material conflict between Accepted
Discoveries, or requires governance of an existing dependency after the
standing or support of an Accepted finding has materially changed.

The existence of possible future conflicts or changes is not, by itself,
sufficient reason to reopen this investigation.

---

## Related Artifacts

- FD-0023 — Authoritative Discovery Dependency Standing
- FD-0022 — Authority Condition of a Discovery in Hold
- FD-0017 — Canonical Discovery Acceptance

---

## Version History

### 0.1.0 — 2026-08-30

Initial preservation of the deferred investigation concerning representation,
verification, conflict, and post-Acceptance governance of authoritative
Discovery dependencies.

---
