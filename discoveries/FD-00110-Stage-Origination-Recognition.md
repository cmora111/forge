# FD-0011 — Stage Origination Authority

**Status:** Accepted
**Version:** 1.0.0

---

# Context

FD-0010 established that Stage creation has two distinct forms:

- Origination
- Succession

Origination establishes the first Stage of a Stage lineage and therefore
requires no predecessor.

Subsequent inspection of the Stage creation implementation exposed a further
governance question.

The Stage lifecycle requires that the procedural requirements governing
legitimate Stage origination be satisfied before an originating Stage is
recognized as `ACTIVE`.

This creates a boundary problem.

The evidence required to justify Origination must exist before the Stage is
recognized as `ACTIVE`, yet the existence of Stage directories, files, or
metadata cannot itself confer Stage lifecycle authority.

Therefore the authority by which a proposed Stage becomes an `ACTIVE` Stage
must be distinguished from the mechanical construction of its artifacts.

---

# Discovery

A proposed Stage and the artifacts necessary to establish its Origination MAY
exist before the Stage is lifecycle-recognized as `ACTIVE`.

Their physical existence SHALL NOT itself constitute Stage Origination.

Before Origination, those artifacts constitute evidence associated with a
proposed Stage. They do not possess Stage lifecycle authority merely because
they have been created.

Stage Origination is the authorized recognition event by which a proposed
Stage is admitted into Stage Method governance as the first `ACTIVE` Stage of
a new Stage lineage.

Preparation of proposed Stage artifacts, recording of Engineering Authority
determinations, and procedural verification of Origination requirements SHALL
precede Origination but SHALL NOT themselves constitute Origination.

The condition preceding Origination is not a Stage lifecycle state.

A proposed Stage is therefore neither `ACTIVE` nor `FROZEN`.

Only successful Origination admits the proposed Stage into the Stage lifecycle
and establishes its initial lifecycle state as `ACTIVE`.

---

# Engineering Authority

Legitimate Origination requires Engineering Authority to explicitly define and
assume the proposed Stage's engineering responsibility.

Before Origination, Engineering Authority SHALL establish:

1. the Engineering Responsibility,
2. the bounded Scope of that responsibility,
3. the Discharge Criteria by which that responsibility may eventually be
   determined to have been legitimately discharged, and
4. whether the proposed responsibility constitutes engineering continuation
   of an existing applicable Stage lineage.

Lineage applicability is an Engineering Authority determination because it
depends upon the engineering relationship between the proposed responsibility
and the responsibilities preserved by existing Stage lineages.

If the proposed responsibility constitutes continuation of an existing
applicable Stage lineage, Origination SHALL NOT be authorized.

If an applicable predecessor Stage is `FROZEN`, continuation SHALL occur
through Succession.

Origination SHALL NOT be used to escape an existing undischarged Stage
responsibility.

---

# Procedural Authority

Procedural Authority SHALL NOT independently determine the engineering
correctness of the Engineering Authority determinations required for
Origination.

Procedural Authority SHALL instead verify that the required determinations:

- exist,
- are persistently recorded,
- contain substantive content rather than generated placeholder content,
- are attributable to Engineering Authority, and
- are procedurally consistent with the proposed Origination.

Procedural Authority SHALL also verify that the proposed Stage declares no
predecessor.

The absence of a predecessor is a procedural property of Origination.

The determination that the proposed responsibility does not constitute
continuation of an existing applicable Stage lineage remains an Engineering
Authority determination.

Procedural Authority MAY verify that preserved Stage records and proposed
Stage metadata do not procedurally contradict that determination.

Procedural Authority SHALL NOT substitute its own engineering interpretation
for the determination of Engineering Authority.

---

# Minimum Origination Evidence

Before Stage Origination may be authorized, Procedural Authority SHALL verify
persistent evidence of:

1. **Proposed Stage Identity**

   The proposed Stage is unambiguously identified so that the Origination
   evidence can be associated with the Stage being considered for recognition.

2. **Engineering Responsibility**

   Engineering Authority has recorded and assumed a substantive engineering
   responsibility.

3. **Bounded Scope**

   Engineering Authority has recorded what the proposed Stage SHALL
   investigate and what it SHALL NOT investigate.

4. **Discharge Criteria**

   Engineering Authority has established an initial substantive basis for
   determining when the Stage responsibility has been legitimately discharged.

5. **Lineage Applicability Determination**

   Engineering Authority has explicitly determined that the proposed
   responsibility does not constitute continuation of an existing applicable
   Stage lineage.

6. **Absence of a Predecessor**

   The proposed Stage procedurally declares no predecessor.

7. **Engineering Authority Attribution**

   The required engineering determinations are unambiguously attributable to
   Engineering Authority and SHALL NOT be manufactured by automation.

8. **Procedural Completeness**

   Required Origination determinations are present and SHALL NOT remain in
   their generated placeholder condition.

9. **Internal Procedural Consistency**

   Proposed Stage metadata and preserved procedural records do not contradict
   the claimed Origination.

Procedural Authority verifies the existence, attribution, completeness, and
procedural consistency of this evidence.

Procedural Authority does not determine whether the engineering judgments
contained within that evidence are technically correct.

---

# Artifact Authority

Artifacts required to establish Origination MAY be constructed before the
proposed Stage enters the Stage lifecycle.

Before Origination, those artifacts serve as Origination evidence.

Their creation SHALL NOT:

- establish an `ACTIVE` Stage,
- establish a Stage lineage,
- constitute Origination, or
- independently confer Stage Method authority.

The authority of engineering determinations recorded before Origination
derives from the Engineering Authority making those determinations, not from
the existence of the proposed Stage.

Upon successful Origination, the accepted Origination artifacts become
authoritative artifacts of the newly recognized `ACTIVE` Stage.

Origination therefore changes the constitutional standing of the proposed
Stage and its accepted artifacts without requiring their physical creation to
occur at the moment of recognition.

---

# Origination Boundary

Origination SHALL be understood as the boundary between:

**Before Origination**

- a proposed Stage may physically exist,
- proposed Stage artifacts may exist,
- required Engineering Authority determinations may be recorded,
- Procedural Authority may inspect Origination evidence,
- no Stage lifecycle state exists, and
- no Stage lineage has yet been established by the proposed Stage.

**After Origination**

- the Stage is recognized by the Stage Method,
- the Stage lineage exists,
- the originating Stage is `ACTIVE`, and
- accepted Origination artifacts possess Stage authority.

Therefore:

> Preparation is not Origination.
>
> Artifact construction is not Origination.
>
> Engineering determination is not Origination.
>
> Procedural verification is not Origination.
>
> Origination is the authorized recognition event that admits the proposed
> Stage into Stage Method governance as `ACTIVE`.

---

# Dual Authority

Stage Origination requires both Engineering Authority and Procedural Authority.

Engineering Authority supplies the engineering judgments necessary to define
and assume the proposed responsibility.

Procedural Authority verifies that the required Origination evidence exists
and satisfies the governing procedural requirements.

Neither authority acting independently is sufficient to originate a Stage.

Origination occurs only after both authorities have discharged their respective
responsibilities.

This preserves the same separation of engineering judgment and procedural
enforcement that governs other Stage Method lifecycle boundaries.

---

# Automation Boundary

Automation MAY:

- construct proposed Stage directories,
- generate proposed Stage artifact structures,
- generate placeholders for required Engineering Authority determinations,
- inspect required Origination evidence,
- verify the absence of unresolved required placeholders,
- verify procedural consistency,
- verify the declared absence of a predecessor, and
- participate in execution of an authorized Origination operation only as 
  permitted by the governing Origination specification.

Automation SHALL NOT:

- define the Engineering Responsibility,
- determine engineering Scope,
- establish Discharge Criteria,
- determine engineering lineage applicability,
- assume Engineering Authority,
- manufacture evidence that Engineering Authority has made a determination, or
- recognize a proposed Stage as `ACTIVE` before the required Origination
  conditions have been satisfied.

Mechanical construction SHALL NOT be treated as lifecycle authority.

---

# Implications

Construction of proposed Stage artifacts is distinct from Stage Origination.

A tool MAY construct the artifacts necessary to propose an originating Stage
without thereby creating an `ACTIVE` Stage.

The Stage Method therefore does not require a third lifecycle state to
represent a Stage awaiting Origination.

Before Origination, there is no lifecycle-recognized Stage requiring such a
state.

The normative Stage lifecycle remains:

    ACTIVE -> FROZEN

Origination establishes the entry boundary into that lifecycle.

Succession provides the corresponding entry mechanism for a Stage continuing
an existing lineage.

The exact implementation mechanism used to represent:

- proposed Stage identity,
- Engineering Authority attribution,
- Origination authorization,
- machine-readable creation form, and
- the command or verb that performs Origination

remains subject to specification.

This discovery does not establish that an originating Stage must be numbered
Stage 0.

---

# Bedrock

> **Artifact construction does not create Stage authority.**
>
> **A proposed Stage becomes a Stage only through authorized Origination.**
>
> **Origination is the recognition event that admits the first Stage of a new
> lineage into Stage Method governance as `ACTIVE`.**

---

# Depends On

- FD-0005 — Dual Authority
- FD-0006 — Lifecycle Determinism
- FD-0009 — Lifecycle Transition Governance
- FD-0010 — Stage Origination

---

# Open Questions

This discovery does not define:

- the concrete representation of Engineering Authority attribution,
- the machine-readable metadata used to distinguish Origination from
  Succession,
- the command or Stage Method verb that performs Origination,
- whether originating Stage numbering is constrained to Stage 0,
- the implementation workflow used to prepare proposed Stage artifacts, or
- whether additional evidence beyond the minimum Origination evidence is
  required by a particular engineering domain.

These remain matters for subsequent specification or investigation.

---

## History

| Version | Status | Description |
|---|---|---|
| 0.1.0 | Draft | Stage Origination Authority |
| 1.0.0 | Accepted | Accepted following Anvil inspection |


