# FD-0018 — Discovery Epistemic Eligibility

**Status:** Hold
**Version:** 0.1.0

---

# Context

FD-0017 established that valid Canonical Discovery Acceptance requires both
sufficient epistemic eligibility and an authorized canonical commit.

Neither condition alone is sufficient.

FD-0017 deliberately did not establish what constitutes sufficient epistemic
eligibility.

That omission exposed a dependency for the Canonical Discovery Acceptance
Specification.

Before that specification can govern the transition of an eligible Discovery
into the canonical Discovery corpus, the Method must be able to distinguish
a Discovery that is epistemically eligible for acceptance consideration from
one that merely claims to be eligible.

Forge investigation, memorialization, Anvil examination, evidentiary support,
dependency resolution, and artifact state may all contribute to that
determination.

None may be assumed sufficient merely because it occurred.

The remaining question is therefore:

> What constitutes sufficient epistemic eligibility for a Forge Discovery to
> become eligible for canonical acceptance?

---

# Discovery

A Forge Discovery is epistemically eligible for canonical acceptance when the
finding presented for acceptance has satisfied the applicable epistemic
examination, its material epistemic dependencies are sufficiently supported
for the use made of them, no known unresolved material epistemic defect
defeats the finding, and sufficient inspectable evidence exists to demonstrate
those conditions for the evaluated state of the finding.

Epistemic eligibility therefore requires the conjunction of:

    Applicable Epistemic Examination
                +
    Sufficient Material Dependency Support
                +
    No Known Unresolved Material Defeating Defect
                +
    Sufficient Inspectable Epistemic Evidence
                +
    Evaluated-State Identity
                ↓
        Epistemic Eligibility

No single component independently establishes eligibility.

---

# Applicable Epistemic Examination

A candidate Discovery must undergo the epistemic examination applicable to
the kind of finding being presented.

The existence of a Discovery artifact does not establish that examination has
occurred.

Therefore:

    Memorialization
            ≠
    Epistemic Eligibility

Likewise, the fact that a finding originated through Forge investigation does
not establish that all epistemic examination required for canonical
acceptance has been satisfied.

Therefore:

    Forge Origination
            ≠
    Epistemic Eligibility

The exact examination required for a particular class of Discovery remains a
governance and specification question.

This Discovery establishes only that the applicable examination must be
satisfied before epistemic eligibility can legitimately be established.

---

# Forge Examination

Forge examination may expose:

- unsupported inference,
- hidden dependency,
- contradiction,
- scope error,
- authority expansion,
- ambiguity,
- overconstraint,
- or other defects in a candidate finding.

A candidate may be reforged in response.

Successful Forge examination therefore contributes to the epistemic basis of
a Discovery.

It does not, merely by occurring, establish sufficient epistemic eligibility.

Therefore:

    Forge Examination
            ≠
    Sufficient Epistemic Eligibility

This prevents the discovery mechanism from automatically certifying its own
output.

---

# Anvil Examination

The Anvil attempts to falsify, break, contradict, or expose material weakness
in a candidate finding.

Survival of applicable Anvil examination provides material epistemic evidence
concerning the finding tested.

It does not establish infallibility.

Nor does the phrase:

    Anvil Survived

by itself establish eligibility if the wrong proposition was tested, the
tested state no longer corresponds materially to the candidate presented for
acceptance, required examination was incomplete, or a material defeating
defect remains unresolved.

Therefore:

    Anvil Survival
            ≠
    Infallibility

and:

    Anvil Survival Alone
            ≠
    Sufficient Epistemic Eligibility

The evidentiary value of Anvil survival attaches to the finding and state
actually subjected to examination.

---

# Material Dependency Support

A Discovery may depend upon findings established elsewhere in the Method.

A dependency need not necessarily possess Accepted canonical status before it
can provide epistemic support.

Therefore:

    Canonical Lifecycle Status
            ≠
    Epistemic Sufficiency

However, where a material dependency is necessary to support the finding
presented for acceptance, that dependency must possess sufficient epistemic
support for the use made of it.

An unresolved material dependency cannot be silently treated as established
merely because the dependent Discovery requires it.

Therefore:

    Required Material Dependency
            +
    Insufficient Epistemic Support
            =
    Eligibility Not Established

The degree and form of support required for particular dependency classes
remain governance questions.

---

# No Known Unresolved Material Defeating Defect

Epistemic eligibility does not require proof that no unknown defect exists.

Such a requirement would demand certainty beyond what engineering
investigation can generally establish.

It does require that no known unresolved material epistemic defect defeats the
finding being presented for acceptance.

Therefore:

    Unknown Possible Defect
            ≠
    Automatic Ineligibility

but:

    Known
    +
    Unresolved
    +
    Material
    +
    Defeats the Finding
            =
    Eligibility Not Established

A known issue that is immaterial to the finding does not automatically defeat
eligibility.

A known material issue that remains unresolved and defeats the finding does.

The determination of materiality must itself remain justified and
inspectable.

---

# Inspectable Epistemic Evidence

A claim that epistemic examination occurred is not equivalent to evidence
that it occurred.

Therefore:

    Claim of Eligibility
            ≠
    Evidence of Eligibility

Sufficient inspectable evidence must exist to demonstrate the epistemic basis
upon which eligibility is claimed.

The evidence must be sufficient to inspect, as applicable:

- what finding was examined,
- what epistemic examination was performed,
- what material dependencies were relied upon,
- what material defects were identified,
- how those defects were resolved or shown not to defeat the finding,
- and what state of the finding the evidence supports.

The exact evidence artifacts, formats, records, or metadata required remain a
specification question.

---

# Evaluated-State Identity

Epistemic evidence attaches to the finding actually examined.

A candidate presented for canonical acceptance cannot silently inherit
epistemic eligibility from a materially different state of the finding.

Therefore:

    Examined State
            ≠
    Materially Altered State

unless the applicable governance establishes that the existing examination
remains sufficient for the altered state.

This requires an inspectable relationship between:

    the finding examined

and:

    the finding presented for acceptance.

That relationship is Evaluated-State Identity.

---

# Material Change

Not every artifact change necessarily alters the epistemic state of a
Discovery.

A correction to spelling, formatting, or other non-material representation
may leave the finding and its evidentiary basis unchanged.

A change that materially alters the finding, its reasoning, its scope, its
dependencies, or the basis upon which it survived epistemic examination may
invalidate prior eligibility evidence for the altered state.

Therefore:

    Non-Material Change
            ≠
    Automatic Loss of Eligibility

but:

    Material Change
            →
    Prior Epistemic Examination
    May No Longer Be Sufficient

This Discovery does not establish the complete rule for determining
materiality or when re-examination is required.

Those determinations belong to governing procedure.

---

# Eligibility Is Not Truth

Epistemic eligibility does not establish that a Discovery is eternally or
infallibly true.

It establishes that the finding has satisfied the applicable epistemic
requirements for consideration for canonical acceptance under the knowledge
and evidence available at that time.

Therefore:

    Epistemically Eligible
            ≠
    Infallibly True

New evidence may later expose contradiction, qualification, limitation, or
falsification.

That possibility does not make epistemic eligibility meaningless.

It establishes the boundary of what eligibility claims.

---

# Eligibility Is Not Acceptance

Epistemic eligibility does not alter the canonical lifecycle state of a
Discovery.

Therefore:

    Epistemically Eligible
            ≠
    Canonically Accepted

An eligible Discovery may remain on Hold or in another applicable
non-Accepted state until a valid authorized canonical acceptance transition
occurs.

This preserves FD-0017's distinction between epistemic eligibility and
authorized canonical commit.

---

# Eligibility Does Not Create Procedural Authority

Epistemic strength does not grant authority to alter the canonical Discovery
corpus.

Therefore:

    Epistemically Eligible
            ≠
    Authorized to Commit

Even a strongly supported finding requires the independently legitimate
Procedural Authority and governed transition required by FD-0017 before valid
canonical acceptance occurs.

This preserves the boundary between Engineering Authority and Procedural
Authority.

---

# Procedural Authority Does Not Create Eligibility

The reverse is also true.

An actor, office, mechanism, or governed process possessing legitimate
Procedural Authority over the canonical corpus cannot make an epistemically
ineligible finding eligible merely by exercising that authority.

Therefore:

    Procedurally Authorized
            ≠
    Epistemically Eligible

The epistemic basis must remain independently demonstrable.

---

# Eligibility Must Be Demonstrable

Epistemic eligibility is not established merely because someone concludes
that a Discovery is ready.

The basis for that conclusion must be inspectable.

Therefore:

    Eligibility Assertion
            ≠
    Eligibility Demonstration

The Method must be capable of distinguishing between:

    examination that occurred

and:

    examination merely claimed to have occurred.

This requires preserved epistemic evidence sufficient for the applicable
eligibility determination.

---

# Consequence

Epistemic eligibility can be understood as an evidence-supported relationship
between a candidate finding and the epistemic examination applicable to it.

The relationship is:

    Candidate Discovery
            │
            ▼
    Applicable Epistemic Examination
            │
            ├───────────────┐
            │               │
            ▼               ▼
    Material Dependency   Material Defect
         Support           Examination
            │               │
            └───────┬───────┘
                    ▼
          Inspectable Evidence
                    │
                    ▼
          Evaluated-State Identity
                    │
                    ▼
          Epistemically Eligible
                    │
                    ▼
       Eligible for Consideration
       for Canonical Acceptance

Epistemic eligibility establishes that the Discovery may legitimately be
presented to the procedural acceptance question.

It does not supply the Procedural Authority required to answer that question
or perform the canonical acceptance transition.

---

# Does Not Establish

This discovery does not establish:

- that memorialization establishes epistemic eligibility,
- that Forge origination establishes epistemic eligibility,
- that Forge examination alone establishes epistemic eligibility,
- that Anvil survival alone establishes epistemic eligibility,
- that Anvil survival establishes infallibility,
- that every Discovery requires identical epistemic examination,
- the exact epistemic examination required for every Discovery class,
- that every material dependency must already be canonically Accepted,
- that canonical lifecycle status and epistemic sufficiency are equivalent,
- that no unknown defect may exist,
- that every known defect defeats eligibility,
- the complete definition of materiality,
- the complete rule for determining whether a change is material,
- the exact circumstances requiring re-examination after change,
- the exact evidence artifacts required to demonstrate eligibility,
- the actor, office, mechanism, or process that determines eligibility,
- that epistemic eligibility creates Procedural Authority,
- that Procedural Authority creates epistemic eligibility,
- that epistemic eligibility constitutes canonical acceptance,
- that an epistemically eligible Discovery is infallibly true,
- the canonical Discovery acceptance procedure,
- or that this Discovery is itself epistemically eligible or Accepted.

---

# Depends On

- FD-0005 — Dual Authority
- FD-0017 — Canonical Discovery Acceptance

---

# Status

| Field | Value |
|---|---|
| Status | Hold |
| Version | 0.1.0 |

This discovery records the currently established result of the investigation
into the conditions required for sufficient epistemic eligibility of a Forge
Discovery before canonical acceptance may legitimately be considered.

It remains subject to further Forge and Anvil inspection before acceptance.

---

# Version History

| Version | Status | Description |
|---|---|---|
| 0.1.0 | Hold | Initial memorialization of the discovery that epistemic eligibility for a |
| | | Forge Discovery requires applicable epistemic examination, sufficient |
| | | material dependency support, absence of a known unresolved material |
| | | defeating defect, sufficient inspectable epistemic evidence, and identity |
| | | between the evaluated finding and the finding presented for canonical |
| | | acceptance. |

---
