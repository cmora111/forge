# FD-0014 — Stage Admission Verification Integrity

**Status:** Hold
**Version:** 0.1.0

---

# Context

Stage Origination and Stage Succession are distinct forms by which a proposed
Stage may become a lifecycle-recognized `ACTIVE` Stage.

Each form requires Engineering Authority determinations and Procedural
Authority verification before the applicable admission event may legitimately
occur.

FD-0011 establishes the authority and minimum evidence required for
Origination.

FD-0012 establishes the authority and minimum evidence required for
Succession.

FD-0013 establishes Controlled Stage Admission and the distinction between
procedural verification and the admission commit through which authorized
Origination or Succession takes lifecycle effect.

FD-0012 further establishes that if required Succession evidence is altered
after procedural verification, the affected verification SHALL be repeated
before Succession may occur.

This exposes a broader question.

Procedural verification necessarily occurs against a particular condition of
the evidence presented for Stage admission.

If that evidence changes after verification but before the admission event,
the evidence presented for admission is no longer necessarily the evidence
that was verified.

Therefore verification integrity must be established independently of the
particular form of Stage admission.

---

# Discovery

Stage-admission verification attaches to the evidence condition actually
inspected.

It does not confer continuing admission authority upon a proposed Stage
independent of that evidence.

A Stage SHALL be admitted only upon required evidence for which the applicable
procedural verification remains valid at the time of admission.

If required Stage-admission evidence changes after procedural verification and
before the applicable admission event, the affected verification SHALL be
repeated before admission may occur.

This requirement applies equally to:

- Origination, and
- Succession.

Stage Admission is a category describing the lifecycle-recognition boundary
implemented through Origination or Succession.

Stage Admission SHALL NOT be interpreted as a separate lifecycle operation,
transition, or Stage lifecycle state.

---

# Verification Object

Procedural verification has an object.

That object is the required evidence condition inspected by Procedural
Authority.

Verification SHALL establish procedural sufficiency only for the evidence
condition actually inspected.

Verification of one evidence condition SHALL NOT be treated as verification
of a different evidence condition merely because:

- both conditions belong to the same proposed Stage,
- the proposed Stage identity has not changed,
- the admission form has not changed, or
- the altered evidence appears similar to previously verified evidence.

Therefore:

> Procedural verification attaches to evidence, not indefinitely to the
> proposal containing that evidence.

---

# Evidence Change

Required Stage-admission evidence MAY change before admission.

Such change SHALL NOT itself constitute a lifecycle violation because the
proposed Stage has not yet been admitted into the Stage lifecycle.

However, verification performed against an earlier evidence condition SHALL
NOT establish procedural sufficiency of a changed evidence condition.

If required evidence changes after verification:

1. the historical fact that the earlier verification occurred SHALL remain
   valid;

2. the earlier verification SHALL NOT be represented as verification of the
   changed evidence;

3. verification affected by the change SHALL be repeated; and

4. admission SHALL NOT occur until the required verification applicable to
   the current evidence condition has been satisfied.

Reverification SHALL establish procedural sufficiency of the evidence
condition then presented for admission.

---

# Affected Verification

A change to required Stage-admission evidence does not necessarily invalidate
every procedural fact previously verified.

Only verification affected by the changed evidence is required by this
discovery to be repeated.

For example, alteration of one required Engineering Authority determination
does not by itself establish that an independently verified predecessor
identity has changed.

This discovery therefore SHALL NOT require indiscriminate repetition of
unaffected verification.

However, verification SHALL NOT rely upon an earlier result where the evidence
upon which that result depended has changed.

---

# Engineering Materiality

Procedural Authority SHALL NOT be required to determine whether a change in
engineering evidence is technically material.

A rule requiring Procedural Authority or automation to decide whether two
different engineering statements are technically equivalent would improperly
transfer engineering judgment to Procedural Authority.

Therefore, where a required Engineering Authority determination has changed
after verification, the verification affected by that determination SHALL be
repeated.

Engineering Authority retains authority over the engineering meaning of the
evidence.

Procedural Authority retains authority over whether the evidence condition
presented for admission is the condition for which the required procedural
verification remains valid.

---

# Origination

The verification-integrity requirement applies to Origination.

Before Origination, Procedural Authority verifies the evidence required to
establish legitimate Stage Origination.

If required Origination evidence changes after that verification and before
Origination occurs, the affected verification SHALL be repeated.

Origination SHALL NOT rely upon procedural verification performed against
required evidence that has since changed.

Successful Origination therefore admits the proposed Stage on the basis of
the evidence condition for which the required Origination verification remains
valid.

This requirement supplements the Origination authority established by
FD-0011.

It does not alter the Engineering Authority determinations required for
Origination.

---

# Succession

The verification-integrity requirement applies equally to Succession.

Before Succession, Procedural Authority verifies the evidence required to
establish legitimate Stage Succession.

If required Succession evidence changes after that verification and before
Succession occurs, the affected verification SHALL be repeated.

Succession SHALL NOT rely upon procedural verification performed against
required evidence that has since changed.

Successful Succession therefore admits the proposed successor on the basis of
the evidence condition for which the required Succession verification remains
valid.

This discovery generalizes the verification-integrity requirement identified
during the investigation of Stage Succession Authority.

It does not alter the Engineering Authority determinations or predecessor
requirements established by FD-0012.

---

# Admission Boundary

Stage Admission describes the boundary at which a proposed Stage becomes a
lifecycle-recognized `ACTIVE` Stage.

The applicable admission event is:

- Origination for the first Stage of a new Stage lineage; or
- Succession for a successor Stage within an existing Stage lineage.

Stage Admission SHALL NOT introduce an additional operation between
Origination or Succession and `ACTIVE` recognition.

The relationship is:

    proposed Stage
          |
          | required evidence
          v
    procedural verification
          |
          | verified evidence condition
          v
    Origination or Succession
          |
          v
        ACTIVE

If required evidence changes between procedural verification and the admission
event, the affected verification SHALL be repeated before that boundary may be
crossed.

---

# Historical Verification Integrity

A verification record is evidence of what Procedural Authority verified at the
time that verification occurred.

Later evidence changes SHALL NOT cause the historical verification record to
be rewritten as though the changed evidence had been inspected.

The Stage Method SHALL preserve the distinction between:

- evidence that was verified,
- evidence that was later changed, and
- evidence that was subsequently reverified.

Historical verification evidence SHALL NOT be rewritten to represent
verification of evidence that was not actually inspected.

This preserves truthful procedural history without asserting that an earlier
verification was invalid when originally performed.

---

# Verification and Authorization

Successful procedural verification does not itself constitute Stage
admission.

Verification establishes that the applicable procedural requirements have
been satisfied for the evidence condition inspected.

If all other required admission conditions are satisfied, that verification
may contribute to authorization of Origination or Succession.

If admission does not occur, the proposed Stage remains outside the Stage
lifecycle.

If required evidence changes before admission, prior verification affected by
that change no longer establishes procedural sufficiency for the current
evidence condition.

Therefore:

> Verification of an admissible proposal is not itself admission.

and:

> Admission authority extends only to the evidence condition for which the
> required verification remains valid.

---

# Post-Admission Boundary

This discovery governs verification integrity between procedural verification
and Stage admission.

It does not establish that Stage artifacts SHALL remain unchanged after
admission.

Once a Stage has been admitted as `ACTIVE`, engineering activity and artifact
evolution are governed by the Stage lifecycle and applicable artifact
governance.

Changes occurring after Stage admission SHALL NOT retroactively alter the
historical evidence condition upon which admission occurred.

The authoritative admission record SHALL continue to represent the evidence
condition under which the Stage was admitted.

---

# Dual Authority

This discovery preserves Dual Authority.

Engineering Authority determines the engineering meaning and substantive
content of required engineering evidence.

Procedural Authority verifies that required evidence:

- exists,
- is attributable as required,
- satisfies applicable procedural requirements, and
- remains the evidence condition for which the required verification is valid
  at the time of admission.

Procedural Authority SHALL NOT determine technical equivalence between changed
engineering determinations.

Engineering Authority SHALL NOT independently declare procedural verification
valid for evidence that has changed since Procedural Authority inspected it.

Neither authority SHALL substitute for the other.

---

# Automation Boundary

Automation MAY:

- record the evidence condition against which procedural verification was
  performed,
- detect changes to required Stage-admission evidence,
- invalidate reliance upon affected prior verification,
- require affected verification to be repeated,
- preserve historical verification records, and
- participate in enforcement of the admission boundary as permitted by the
  governing Stage Method specification.

Automation SHALL NOT:

- determine whether changed engineering evidence is technically equivalent,
- determine whether an engineering change is substantively insignificant,
- reinterpret Engineering Authority determinations,
- rewrite historical verification evidence to represent inspection that did
  not occur, or
- treat successful verification as Stage admission.

The exact mechanism used to detect evidence change is not established by this
discovery.

---

# Implementation Independence

This discovery establishes an invariant, not an implementation mechanism.

Verification integrity MAY eventually be enforced using mechanisms including:

- manifests,
- hashes,
- snapshots,
- controlled metadata,
- transactional operations,
- direct evidence comparison, or
- other procedurally sufficient mechanisms.

No particular mechanism is required by this discovery.

The governing requirement is that the evidence condition admitted is the
evidence condition for which the required procedural verification remains
valid.

---

# Implications

Origination and Succession share a common verification-integrity requirement.

The requirement belongs to the Stage-admission boundary rather than uniquely
to either admission form.

Procedural verification is evidence-specific.

Verification does not attach permanently to a proposed Stage.

Changing required evidence after verification may require affected
reverification before admission.

Earlier verification remains truthful historical evidence of what was
actually inspected.

Reverification SHALL NOT rewrite that history.

Stage Admission remains a category encompassing Origination and Succession and
does not create a third Stage-creation form or additional lifecycle state.

---

# Bedrock

> **Admission authority extends only to the evidence condition actually
> verified.**
>
> **If required admission evidence changes before admission, affected
> verification must be repeated.**
>
> **Verification history records what was actually inspected and must not be
> rewritten to claim otherwise.**

---

# Depends On

- FD-0005 — Dual Authority
- FD-0006 — Lifecycle Determinism
- FD-0009 — Lifecycle Transition Governance
- FD-0010 — Stage Origination
- FD-0011 — Stage Origination Authority
- FD-0012 — Stage Succession Authority
- FD-0013 — Controlled Stage Admission

---

# Open Questions

This discovery does not define:

- the machine-readable representation of a verified evidence condition,
- the mechanism used to detect changes to required admission evidence,
- whether hashes, manifests, snapshots, transactions, or another mechanism
  SHALL be used,
- the exact persistence format of verification records,
- the command or Stage Method verb responsible for performing verification,
- whether verification and admission may be implemented as one atomic
  operation,
- the artifact-specific post-admission mutability rules, or
- the broader governance status of engineering activity performed before a
  proposed Stage is admitted into the Stage lifecycle.

These remain matters for subsequent specification or investigation.

---

## History

| Version | Status | Description |
|---|---|---|
| 0.1.0 | Hold | Stage Admission Verification Integrity |
