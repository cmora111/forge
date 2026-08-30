# FI-0001 — Discovery Candidate and Hold Governance

**Status:** Deferred  
**Origin:** FD-0022 — Authority Condition of a Discovery in Hold  
**Deferred:** 2026-08-30

---

## Question

What governance establishes a proposed Forge Discovery as a governed Discovery
candidate in Hold, and how is that standing represented and distinguished from
the standing of an Accepted Discovery?

---

## Why Deferred

The investigation of FD-0022 required distinguishing the governed existence of
a Discovery candidate from the authority of its finding.

That investigation established that a Discovery in Hold may possess governed
candidate standing without its finding possessing the canonical standing
conferred by Canonical Discovery Acceptance.

This exposed additional questions concerning:

- how a proposed Discovery formally enters Hold;
- what authority is required for that memorialization;
- what governance effects are created by entry into Hold; and
- how governed Discovery candidates are represented and distinguished from
  Accepted Discoveries.

Resolution of those questions was not demonstrated to be necessary to establish
the authority condition of a Discovery already in Hold.

They were therefore left unresolved rather than extending FD-0022 into the
complete governance and lifecycle of Discovery candidates.

This investigation is preserved for future work and is not presently blocking
the engineering work that exposed it.

---

## Preserved Findings

The following findings and distinctions were established or preserved during
the investigation that exposed this question:

### Governed Candidate Standing

A Forge Discovery in Hold is a governed proposed Discovery whose finding has
not acquired the canonical standing conferred by Canonical Discovery
Acceptance.

Hold establishes governed candidate standing.

Hold does not, by itself, confer epistemic authority, normative authority, or
canonical acceptance authority upon the Discovery's finding.

Therefore:

    Governed Discovery Candidate ≠ Authoritative Finding

and:

    Hold ≠ Canonical Discovery Acceptance

---

### Governance and Authority

Governance of a Discovery candidate is distinct from authority of the
Discovery's finding.

Therefore:

    Governance of Candidate ≠ Authority of Finding

The fact that a proposed Discovery is governed, recorded, tracked, inspected,
or maintained does not establish that its finding may be relied upon as an
authoritative Discovery premise.

---

### Artifact Existence

The existence of a Discovery artifact does not, by itself, establish Hold
standing.

Therefore:

    Artifact Existence ≠ Hold

The exact governed mechanism by which an artifact or proposed Discovery
acquires Hold standing remains unresolved.

---

### Investigative Dependency

A Discovery in Hold may participate in continuing Forge investigation,
Reforge, Anvil inspection, evidence gathering, epistemic-eligibility
investigation, dependency discovery, and historical preservation.

Such investigative use does not make its finding an authoritative dependency.

Therefore:

    Investigative Dependency ≠ Authoritative Dependency

---

### Epistemic Eligibility

A Discovery may coherently be both:

    Hold + Epistemically Eligible

Epistemic eligibility does not itself establish Canonical Discovery Acceptance.

Therefore:

    Epistemic Eligibility ≠ Canonical Acceptance

---

### Acceptance and Artifact Creation

Canonical Discovery Acceptance changes the standing of the finding of an
already-governed Discovery candidate.

The creation or memorialization of the Discovery artifact is not itself that
Acceptance.

Therefore:

    Artifact Creation ≠ Canonical Discovery Acceptance

---

### Storage and Authority

Governed Discovery candidates and Accepted Discoveries may potentially share
storage, representation, or other infrastructure without thereby possessing
the same authority.

Therefore:

    Common Storage ≠ Common Authority

FD-0022 deliberately did not establish whether a Discovery in Hold is a member
of, outside of, or otherwise associated with a structure called the canonical
Discovery corpus.

That question remains unresolved unless subsequent engineering demonstrates
that the distinction is necessary.

---

## Unresolved Questions

This Future Investigation preserves the following unresolved questions:

1. By what governed mechanism does a proposed Discovery acquire Hold standing?

2. What authority is required to perform or recognize that memorialization?

3. What exact governance effects are created when a proposed Discovery enters
   Hold?

4. How is governed candidate standing represented?

5. How is a governed Discovery candidate distinguished from an Accepted
   Discovery in canonical records or structures?

6. Does Hold imply membership in a canonical Discovery corpus, association with
   such a corpus, or some other governed relationship to it?

These questions are preserved without assuming that every one of them must
eventually require a separate Forge Discovery or Stage specification.

---

## Re-entry Condition

Reopen this investigation only when a concrete Forge–Stage engineering
operation requires resolution of how a proposed Discovery acquires governed
Hold standing, what authority governs that transition, or how governed
Discovery candidates must be represented or distinguished from Accepted
Discoveries.

The existence of an unresolved Discovery-candidate lifecycle question is not,
by itself, sufficient reason to reopen this investigation.

---

## Related Artifacts

- FD-0022 — Authority Condition of a Discovery in Hold
- FD-0023 — Authoritative Discovery Dependency Standing
- FD-0017 — Canonical Discovery Acceptance

---

## Version History

### 0.1.0 — 2026-08-30

Initial preservation of the deferred investigation concerning Discovery
candidate governance, acquisition of Hold standing, memorialization authority,
and representation of governed Discovery candidates relative to Accepted
Discoveries.

---
