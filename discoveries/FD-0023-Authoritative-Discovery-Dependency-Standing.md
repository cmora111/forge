# FD-0023 — Authoritative Discovery Dependency Standing

**Status:** Hold
**Version:** 0.1.0

---

# Context

FD-0017 established that valid Canonical Discovery Acceptance requires both
sufficient epistemic eligibility and an authorized canonical commit.

FD-0018 established that epistemic eligibility is distinct from Canonical
Discovery Acceptance and does not itself create Procedural Authority.

FD-0019 established how epistemic eligibility is legitimately demonstrated.

FD-0022 established that a Forge Discovery in Hold is a governed proposed
Discovery whose finding has not acquired the canonical standing conferred by
Canonical Discovery Acceptance.

FD-0022 further established:

    Governed Discovery Candidate
                ≠
        Authoritative Finding

and:

    Investigative Dependency
                ≠
        Authoritative Dependency

FD-0022 deliberately did not establish the exact canonical standing conferred
upon an Accepted Discovery or the complete rules governing authoritative
dependency upon Accepted Discoveries.

This exposed the next question:

> What standing is required of a Forge Discovery before its finding may be
> used as an authoritative dependency in Stage engineering?

---

# Discovery

A Forge Discovery finding may serve as an authoritative dependency in Stage
engineering only after the Discovery has acquired the canonical standing
conferred by valid Canonical Discovery Acceptance.

That standing permits Stage engineering to rely upon the Accepted finding as
an established Discovery premise within the finding's established scope and
limitations without independently re-establishing the finding each time it is
used.

Therefore:

    Artifact Existence
            ≠
    Authoritative Dependency Standing

    Hold
            ≠
    Authoritative Dependency Standing

    Forge Survival
            ≠
    Authoritative Dependency Standing

    Anvil Survival
            ≠
    Authoritative Dependency Standing

    Epistemic Eligibility
            ≠
    Authoritative Dependency Standing

while:

    Valid Canonical Discovery Acceptance
                    │
                    ▼
              Accepted
                    │
                    ▼
        Canonical Standing
        of Discovery Finding
                    │
                    ▼
        Eligible for Authoritative
        Dependency in Stage Engineering

Canonical Discovery Acceptance therefore changes more than a lifecycle label.

It establishes the governed standing under which the Discovery finding may be
relied upon as an authoritative Discovery dependency.

---

# Authoritative Reliance Is Distinct From Investigative Use

A Discovery need not possess authoritative dependency standing merely to be
examined, challenged, refined, reforged, Anvil-tested, compared, or otherwise
used during investigation.

A Hold Discovery may therefore participate in investigation without its
finding becoming an authoritative premise.

For example:

    Discovery D raises Question Q
                │
                ▼
    Q is investigated

does not establish:

    Discovery D authoritatively
    establishes Proposition P
                │
                ▼
    Stage Requirement R
    is derived from P

Therefore:

    Investigative Use
            ≠
    Authoritative Reliance

Authoritative reliance occurs when Stage engineering is entitled to treat the
finding as an established Discovery premise rather than independently
re-establishing that premise for the engineering act being performed.

---

# Acceptance Is Required

The physical existence, memorialization, Forge examination, Anvil survival, or
epistemic eligibility of a Discovery does not independently establish the
standing required for authoritative dependency.

A Discovery may be:

- memorialized;
- governed;
- on Hold;
- extensively investigated;
- successfully Anvil-tested; and
- epistemically eligible;

while still lacking the standing conferred by Canonical Discovery Acceptance.

Therefore:

    Epistemically Eligible
            ≠
    Accepted

and:

    Anvil Survival
            ≠
    Accepted

and:

    Hold
            ≠
    Authoritative Dependency

This preserves the distinction between epistemic sufficiency and governed
canonical standing.

---

# Acceptance Does Not Confer Unlimited Authority

Authoritative dependency standing does not permit a Discovery finding to be
used beyond what the Discovery actually establishes.

Acceptance cannot enlarge:

- the finding;
- its scope;
- its stated conditions;
- its qualifications;
- its limitations; or
- its explicit non-findings.

Therefore:

    Accepted Discovery
            │
            ▼
    Authoritative Reliance
            │
            ▼
    Only Within Established
    Finding, Scope, and Limitations

and:

    Authoritative Dependency Standing
                    ≠
            Unlimited Authority

A Stage specification, adapter, implementation, or other engineering artifact
must not attribute to an Accepted Discovery a proposition that the Discovery
does not establish.

---

# Acceptance Does Not Establish Infallibility

Authoritative dependency standing does not mean that an Accepted Discovery is
eternally true, immune from challenge, incapable of later qualification, or
protected from future evidence.

Canonical Acceptance establishes governed standing for present authoritative
reliance.

It does not establish epistemic infallibility.

Therefore:

    Accepted
        ≠
    Infallibly True

and:

    Authoritative Dependency
            ≠
    Immunity From Challenge

New evidence may later expose a defect, limitation, contradiction, or other
condition requiring additional governance.

The procedure governing any resulting withdrawal, supersession, deprecation,
invalidation, or other post-Acceptance transition is not established here.

---

# Authoritative Reliance Avoids Re-Proving Every Dependency

If every use of a Discovery finding required Stage engineering to independently
repeat the complete epistemic investigation behind that finding, Canonical
Discovery Acceptance would fail to provide stable engineering dependency
standing.

Valid Acceptance permits the relationship:

    Discovery Establishes Finding X
                │
                ▼
        Valid Canonical
        Discovery Acceptance
                │
                ▼
          Accepted Finding X
                │
                ▼
    Later Stage Engineering
    May Rely Upon X Within Scope

without requiring the complete Forge and Anvil investigation establishing X to
be repeated merely because X is used as a dependency.

This does not remove the requirement to verify that the Accepted Discovery is
the applicable dependency and that the proposed reliance remains within its
established scope.

---

# Proposition Authority and Discovery Authority Are Distinct

A proposition appearing in a Hold Discovery may also be established by another
Accepted Discovery or another independently authoritative source.

In that case, Stage engineering may possess an authoritative basis for the
proposition without the Hold Discovery itself possessing authoritative
dependency standing.

For example:

    FD-X — Hold
       establishes candidate proposition P

    FD-Y — Accepted
       independently establishes P

Stage engineering may rely upon P through the authoritative standing of FD-Y.

The existence of that independent basis does not transform FD-X into an
Accepted Discovery.

Therefore:

    Authority for Proposition P
                ≠
    Authority of Every Artifact
    Containing Proposition P

and:

    Independent Authoritative Source
                ≠
    Acceptance of Hold Discovery

---

# Conflicting Accepted Discoveries

The existence of authoritative dependency standing does not itself resolve a
conflict between Accepted Discoveries.

If two Accepted Discoveries appear to establish materially incompatible
findings, the conflict exposes a separate governance or epistemic problem.

Therefore:

    Authoritative Standing
            ≠
    Conflict Resolution

This Discovery does not establish the procedure for detecting, resolving, or
governing conflicts between Accepted Discoveries.

---

# Inspectability

It must be possible to distinguish:

    Discovery used investigatively

from:

    Discovery relied upon authoritatively

and:

    Discovery possessing Accepted standing

from:

    Discovery merely present, governed,
    examined, or epistemically eligible.

The mere presence of a Discovery in a repository, directory, registry, index,
dependency list, specification, or other engineering artifact MUST NOT be
treated as sufficient evidence that the Discovery possesses authoritative
dependency standing.

Likewise, repeated citation or historical use of a Discovery MUST NOT by itself
be treated as evidence of Canonical Discovery Acceptance.

---

# Consequence

The relevant dependency relationship is:

    Governed Discovery Candidate
                │
                ▼
              Hold
                │
                │ Forge / Reforge / Anvil
                │ epistemic evaluation
                ▼
        Epistemic Eligibility
                │
                ▼
        Valid Canonical Discovery
              Acceptance
                │
                ▼
             Accepted
                │
                ▼
        Canonical Standing
        of Discovery Finding
                │
                ▼
        Authoritative Dependency
        Available to Stage Engineering
                │
                ▼
        Reliance Within Finding,
        Scope, and Limitations

This preserves a boundary between investigation and authoritative engineering
dependency.

Stage engineering must not use the finding of a non-Accepted Discovery as an
authoritative premise merely because that finding is useful, persuasive,
necessary to current engineering, or has survived Forge or Anvil examination.

---

# Does Not Establish

This Discovery does not establish:

- the complete lifecycle of a Forge Discovery;
- the mechanism by which a proposed Discovery enters Hold;
- the method by which epistemic eligibility is established;
- the complete Canonical Discovery Acceptance procedure;
- the actor or authority permitted to perform Canonical Discovery Acceptance;
- the source of the Procedural Authority required for Acceptance;
- that every Accepted Discovery is epistemically infallible;
- that Accepted standing permits reliance outside the finding's established
  scope or limitations;
- the complete method for determining whether a Discovery is applicable to a
  particular Stage engineering decision;
- the procedure for resolving conflicts between Accepted Discoveries;
- the procedure for withdrawing, superseding, deprecating, invalidating, or
  otherwise changing the standing of an Accepted Discovery;
- that an independently authoritative proposition causes every Discovery
  containing that proposition to become authoritative;
- the complete representation of authoritative dependencies in Stage
  specifications or other artifacts;
- or that this Discovery is itself Accepted.

---

# Open Dependencies

This Discovery exposes but does not resolve the following engineering
questions:

1. What independently legitimate authority may perform the first Canonical
   Discovery Acceptance before any Accepted Discovery can serve as an
   authoritative dependency for that act?

2. How must Stage engineering represent and verify authoritative Discovery
   dependencies?

3. What governance applies when Accepted Discoveries materially conflict?

4. What post-Acceptance governance applies when new evidence undermines an
   Accepted finding?

These questions become blocking only where subsequent engineering demonstrates
that their resolution is required.

---

# Depends On

- FD-0017 — Canonical Discovery Acceptance
- FD-0018 — Discovery Epistemic Eligibility
- FD-0019 — Epistemic Eligibility Establishment
- FD-0022 — Authority Condition of a Discovery in Hold

---

# Status

| Field | Value |
|---|---|
| Status | Hold |
| Version | 0.1.0 |

This Discovery memorializes the finding that valid Canonical Discovery
Acceptance establishes the canonical standing required for a Discovery finding
to serve as an authoritative dependency in Stage engineering, while preserving
the distinction between authoritative reliance, epistemic eligibility, and
investigative use.

It remains subject to governed Canonical Discovery Acceptance and does not
acquire authoritative dependency standing merely by this memorialization.

---

# Version History

## 0.1.0 — Hold

Initial memorialization.

Established the candidate finding that a Forge Discovery finding may serve as
an authoritative dependency in Stage engineering only after the Discovery has
acquired the canonical standing conferred by valid Canonical Discovery
Acceptance.

Established that authoritative reliance is bounded by the Accepted finding's
scope and limitations and does not confer infallibility or unlimited authority.

Preserved the distinction between investigative use and authoritative
dependency and established that Forge survival, Anvil survival, epistemic
eligibility, repeated citation, and artifact existence do not independently
confer authoritative dependency standing.

Recorded unresolved questions concerning first-Acceptance authority,
representation of authoritative dependencies, conflicts among Accepted
Discoveries, and post-Acceptance epistemic change.

---
