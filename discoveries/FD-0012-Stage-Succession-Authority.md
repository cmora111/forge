# FD-0012 — Stage Succession Authority

**Status:** Accepted
**Version:** 1.0.0

---

# Context

The Stage lifecycle establishes that further engineering work belonging to an
existing Stage lineage SHALL occur in a successor Stage created from a
`FROZEN` predecessor.

It further establishes that a successor Stage SHALL be created only from a
`FROZEN` predecessor and SHALL begin in the `ACTIVE` state.

These requirements establish when Succession is possible, but they do not by
themselves establish sufficient authority for Succession.

A `FROZEN` predecessor establishes that the predecessor's engineering
responsibility has been legitimately discharged and that its engineering
record has become immutable history.

The existence of a `FROZEN` predecessor does not determine:

- whether additional engineering work is required,
- whether proposed work belongs to the predecessor's Stage lineage,
- what responsibility a successor Stage should assume, or
- what predecessor engineering state must form the successor's starting
  foundation.

Therefore the authority by which a proposed successor becomes the recognized
`ACTIVE` continuation of an existing Stage lineage must be explicitly
established.

---

# Discovery

A `FROZEN` predecessor is necessary but not sufficient authority for
Succession.

Legitimate Succession requires both:

1. a valid `FROZEN` predecessor from which the proposed successor derives; and
2. Engineering Authority determination that the proposed successor
   responsibility constitutes continuation of the Stage lineage represented
   by that predecessor.

A successor Stage SHALL possess its own Engineering Responsibility.

Succession SHALL NOT reopen, reactivate, or transfer the discharged
responsibility of the predecessor into the successor.

Before Succession, a proposed successor and the artifacts necessary to
establish Succession MAY exist without possessing a Stage lifecycle state.

Their physical existence SHALL NOT itself constitute Succession or confer
Stage lifecycle authority.

Succession is the authorized recognition event by which a proposed successor
Stage is admitted into an existing Stage lineage as an `ACTIVE` Stage derived
from a `FROZEN` predecessor.

No separate lifecycle-recognition operation is required after Succession.

Upon successful Succession, the successor's initial and immediate lifecycle
state SHALL be `ACTIVE`.

---

# Engineering Authority

Before Succession, Engineering Authority SHALL explicitly define and assume
the proposed successor's engineering responsibility.

Engineering Authority SHALL establish:

1. the successor Engineering Responsibility,
2. the bounded Scope of that responsibility,
3. the Discharge Criteria by which that responsibility may eventually be
   determined to have been legitimately discharged,
4. that the proposed responsibility constitutes engineering continuation of
   the Stage lineage represented by the declared predecessor, and
5. the predecessor engineering state material to the successor's starting
   engineering baseline.

Lineage continuation is an Engineering Authority determination.

Shared project identity, chronology, hardware, repository, subject matter, or
Stage numbering SHALL NOT by themselves establish engineering lineage
continuation.

Engineering Authority SHALL determine whether the engineering relationship
between the predecessor and proposed successor is sufficient to constitute
continuation of the existing Stage lineage.

Engineering Authority SHALL also determine which elements of the
predecessor's frozen engineering state are material to truthful reconstruction
of the successor's starting engineering condition.

---

# Procedural Authority

Procedural Authority SHALL verify that the proposed successor explicitly
identifies the predecessor from which Succession is claimed.

Procedural Authority SHALL verify that the declared predecessor:

- exists,
- is a recognized Stage, and
- is `FROZEN`.

Procedural Authority SHALL verify that the required Engineering Authority
determinations:

- exist,
- are persistently recorded,
- contain substantive content rather than generated placeholder content,
- are attributable to Engineering Authority, and
- are procedurally consistent with the proposed Succession.

Procedural Authority SHALL verify preservation and traceability of the
declared inherited predecessor baseline.

Procedural Authority SHALL NOT independently determine:

- whether the proposed responsibility is technically appropriate,
- whether the successor Scope is technically sufficient,
- whether the Discharge Criteria are technically sufficient,
- whether the proposed responsibility constitutes engineering continuation,
  or
- which predecessor engineering state is technically material.

Those remain Engineering Authority determinations.

Procedural Authority SHALL NOT substitute its own engineering interpretation
for the determinations of Engineering Authority.

---

# Minimum Succession Evidence

Before Succession may be authorized, Procedural Authority SHALL verify
persistent evidence of:

1. **Proposed Successor Identity**

   The proposed successor is unambiguously identified so that the Succession
   evidence can be associated with the Stage being considered for recognition.

2. **Predecessor Identity**

   The proposed successor explicitly identifies the Stage from which
   Succession is claimed.

3. **Frozen Predecessor**

   The declared predecessor exists as a recognized Stage and is `FROZEN`.

4. **Engineering Responsibility**

   Engineering Authority has recorded and assumed a substantive Engineering
   Responsibility belonging to the proposed successor.

5. **Bounded Scope**

   Engineering Authority has recorded what the proposed successor SHALL
   investigate and what it SHALL NOT investigate.

6. **Discharge Criteria**

   Engineering Authority has established an initial substantive basis for
   determining when the successor responsibility has been legitimately
   discharged.

7. **Lineage Continuation Determination**

   Engineering Authority has explicitly determined that the proposed
   successor responsibility constitutes continuation of the Stage lineage
   represented by the declared predecessor.

8. **Inherited Engineering Baseline**

   Engineering Authority has identified the predecessor engineering state
   material to the proposed successor's starting engineering condition.

9. **Baseline Traceability**

   The proposed successor preserves sufficient evidence to trace the material
   inherited or referenced engineering state to the authoritative frozen
   engineering state of the declared predecessor.

10. **Known Material Divergences**

    Known material differences between the predecessor's frozen engineering
    baseline and the proposed successor's actual starting condition are
    explicitly disclosed and SHALL NOT be represented as inherited state.

11. **Engineering Authority Attribution**

    The required engineering determinations are unambiguously attributable to
    Engineering Authority and SHALL NOT be manufactured by automation.

12. **Procedural Completeness**

    Required Succession determinations are present and SHALL NOT remain in
    their generated placeholder condition.

13. **Internal Procedural Consistency**

    Proposed successor metadata, predecessor references, baseline records, and
    preserved procedural evidence do not contradict the claimed Succession.

Procedural Authority verifies the existence, attribution, completeness,
consistency, predecessor status, and traceability of the required evidence.

Procedural Authority does not determine whether the engineering judgments
contained within that evidence are technically correct.

---

# Predecessor Baseline

Succession SHALL preserve truthful and traceable engineering continuity from
the `FROZEN` predecessor to the successor.

A successor SHALL inherit the relevant frozen engineering baseline of its
declared predecessor as its traceable starting foundation.

Baseline inheritance SHALL NOT be interpreted as requiring every predecessor
artifact to become a successor artifact.

The predecessor contains both:

- engineering state relevant to future continuation, and
- historical evidence describing engineering activity performed within the
  predecessor.

Those roles SHALL remain distinguishable.

The predecessor's frozen engineering baseline provides the engineering
foundation from which the successor derives.

The predecessor's historical evidence remains attributable to the predecessor.

---

# Baseline Completeness

An inherited predecessor baseline is sufficiently complete when it preserves
or explicitly references all predecessor engineering state known by
Engineering Authority at the time of Succession to be material to truthful
reconstruction of:

- the successor's starting engineering condition, and
- the successor's derivation from the predecessor.

Baseline completeness SHALL be determined by engineering state, not merely by
filesystem completeness.

Material predecessor state MAY be:

- physically inherited,
- preserved as controlled artifacts, or
- explicitly referenced where physical inheritance is not applicable.

Engineering Authority determines engineering materiality.

Procedural Authority verifies that the declared baseline and its provenance
have been preserved as required.

The Stage Method does not require Engineering Authority to possess knowledge
that was unavailable at the time of Succession.

A material dependency discovered later SHALL be preserved as new engineering
evidence rather than silently rewritten into the historical Succession record.

---

# Baseline Divergence

Known material predecessor state that is not actually inherited SHALL be
explicitly identified as a divergence from the predecessor baseline.

A known material divergence SHALL NOT be represented as inherited state.

Undisclosed divergence SHALL NOT be used to establish truthful baseline
continuity.

This discovery does not determine whether every possible divergence is
permissible before Succession.

The governance of engineering activity occurring before Stage admission
remains subject to separate investigation.

---

# Historical Separation

Succession continues a Stage lineage.

It does not merge the engineering histories of predecessor and successor.

The successor SHALL NOT inherit the predecessor's:

- Stage identity,
- discharged Engineering Responsibility, or
- historical engineering evidence

as though those belonged to the successor.

Historical evidence produced by the predecessor SHALL remain attributable to
the predecessor.

The successor MAY reference predecessor evidence when establishing its
engineering baseline, lineage relationship, or engineering context.

Such reference SHALL NOT recharacterize predecessor evidence as evidence
produced by the successor.

The successor SHALL establish and maintain its own responsibility, evidence,
audit history, and lifecycle record.

---

# Lineage Preservation

Succession SHALL preserve an unambiguous lineage relationship between the
successor and the exact `FROZEN` predecessor from which it derives.

The predecessor relationship SHALL be explicit and persistently recorded.

The exact machine-readable representation of that relationship is not
established by this discovery.

Stage numbering alone SHALL NOT constitute sufficient evidence of lineage.

The existence of chronological adjacency alone SHALL NOT constitute sufficient
evidence of lineage.

Lineage is established through authorized Succession from the declared
`FROZEN` predecessor.

---

# Succession Boundary

Activities necessary to prepare a proposed successor SHALL NOT themselves
constitute Succession.

Before Succession:

- the proposed successor MAY physically exist,
- proposed successor artifacts MAY exist,
- Engineering Authority determinations MAY be recorded,
- predecessor baseline inheritance or reference MAY be prepared,
- Procedural Authority MAY inspect the required Succession evidence, and
- the proposed successor possesses no Stage lifecycle state.

Satisfaction of the requirements necessary to authorize Succession SHALL NOT
itself create the successor Stage.

If authorized Succession does not occur, the proposed successor remains
outside the Stage lifecycle.

Upon successful Succession:

- the proposed successor becomes a recognized Stage,
- the successor is admitted into the existing Stage lineage,
- the predecessor remains `FROZEN`,
- the successor begins in the `ACTIVE` state, and
- the accepted Succession evidence becomes authoritative Stage evidence of
  the successor's admission and inherited baseline.

Therefore:

> Preparation is not Succession.
>
> Artifact construction is not Succession.
>
> Engineering determination is not Succession.
>
> Procedural verification is not Succession.
>
> Succession is the authorized recognition event by which a proposed successor
> becomes the `ACTIVE` continuation of an existing Stage lineage.

---

# Verification Integrity

Succession SHALL operate upon the evidence for which its authorization
requirements were satisfied.

If required Succession evidence is altered after procedural verification, the
affected verification SHALL be repeated before Succession may occur.

Successful verification SHALL NOT itself constitute Succession.

A proposed successor SHALL NOT be represented as a recognized Stage unless
Succession has completed successfully.

Upon successful Succession, the successor SHALL be represented as `ACTIVE`.

The implementation mechanism used to preserve this boundary remains subject
to specification.

---

# Predecessor Immutability

Succession SHALL NOT modify the `FROZEN` predecessor.

Engineering state, artifacts, and evidence MAY flow outward from the
predecessor through inheritance or reference.

Succession SHALL NOT rewrite predecessor history in order to establish the
successor.

The predecessor remains the authoritative immutable record of its own
engineering activity and discharged responsibility.

Engineering modifications performed in pursuit of the successor's
responsibility belong to the successor and SHALL NOT be represented as
modifications of the predecessor.

---

# Dual Authority

Stage Succession requires both Engineering Authority and Procedural Authority.

Engineering Authority:

- defines and assumes the successor responsibility,
- establishes its bounded Scope,
- establishes its Discharge Criteria,
- determines engineering lineage continuation,
- determines the predecessor engineering state material to the successor
  baseline, and
- identifies known material baseline divergences.

Procedural Authority:

- verifies successor and predecessor identity,
- verifies that the predecessor exists and is `FROZEN`,
- verifies required Engineering Authority determinations,
- verifies procedural completeness and consistency,
- verifies baseline preservation and provenance, and
- verifies disclosure of required baseline divergence records.

Neither authority acting independently is sufficient to authorize legitimate
Succession.

Succession occurs only after both authorities have fulfilled their respective
Succession responsibilities.

---

# Automation Boundary

Automation MAY:

- construct proposed successor Stage structures,
- preserve predecessor identity and lineage metadata,
- generate placeholders for required Engineering Authority determinations,
- copy or reference declared predecessor baseline artifacts,
- verify that the declared predecessor exists,
- verify that the declared predecessor is `FROZEN`,
- inspect required Succession evidence,
- verify the absence of unresolved required placeholders,
- verify procedural consistency,
- verify the presence of required baseline provenance, and
- participate in execution of an authorized Succession operation only as
  permitted by the governing Succession specification.

Automation SHALL NOT:

- define the successor Engineering Responsibility,
- determine engineering Scope,
- establish Discharge Criteria,
- determine engineering lineage continuation,
- determine which predecessor engineering state is technically material,
- conceal or reinterpret known material baseline divergences,
- assume Engineering Authority,
- manufacture evidence that Engineering Authority has made a determination,
  or
- modify the `FROZEN` predecessor.

Mechanical construction SHALL NOT be treated as lifecycle authority.

---

# Implications

A `FROZEN` predecessor establishes the possibility of Succession.

It does not establish sufficient authority to succeed.

Succession requires a new bounded engineering responsibility belonging to the
existing Stage lineage.

A successor continues the lineage but does not reopen the predecessor or
inherit its discharged responsibility.

The successor's starting engineering condition must remain truthfully and
traceably related to the authoritative frozen engineering state of its
declared predecessor.

The predecessor remains immutable engineering history.

The successor becomes a Stage only through successful authorized Succession.

Succession itself confers the successor's initial `ACTIVE` lifecycle state.

No intermediate successor lifecycle state and no separate post-Succession
recognition operation are required.

---

# Bedrock

> **A frozen predecessor establishes the possibility of Succession; it does
> not establish the authority to succeed.**
>
> **Succession continues a lineage by establishing a new responsibility from
> a truthful and traceable predecessor engineering baseline.**
>
> **A proposed successor becomes the `ACTIVE` continuation of its lineage only
> through authorized Succession.**

---

# Depends On

- FD-0005 — Dual Authority
- FD-0006 — Lifecycle Determinism
- FD-0009 — Lifecycle Transition Governance
- FD-0010 — Stage Origination
- FD-0011 — Stage Origination Authority

---

# Open Questions

This discovery does not define:

- the machine-readable representation of predecessor identity,
- the machine-readable representation of baseline inheritance,
- the specific artifact types constituting an engineering baseline,
- the use of hashes, manifests, snapshots, or other mechanisms for proving
  artifact provenance,
- Stage numbering or numbering adjacency requirements,
- the command or Stage Method verb that performs Succession,
- the implementation mechanism that ensures successful Succession and
  `ACTIVE` recognition occur consistently,
- whether particular material divergences are permissible before Succession,
  or
- the broader governance status of engineering activity performed before a
  proposed Stage is admitted into the Stage lifecycle.

These remain matters for subsequent specification or investigation.

---

## History

| Version | Status | Description |
|---|---|---|
| 0.1.0 | Draft | Stage Succession Authority |
| 1.0.0 | Accepted | Accepted following Anvil inspection |


