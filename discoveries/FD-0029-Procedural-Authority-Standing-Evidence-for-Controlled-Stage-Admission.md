# FD-0029 — Procedural Authority Standing Evidence for Controlled Stage Admission

**Status:** Accepted
**Version:** 1.0.0

---

# Forge Question

What evidence is sufficient to establish and preserve the identity and standing
of the governing Procedural Authority for a particular Controlled Stage
Admission?

---

# Context

FD-0026 established that procedural verification is attributable to a governing
Procedural Authority only when sufficient provenance connects the governing
Procedural Authority, the authorized procedure, and the particular verification
performed under that authorization.

FD-0027 established that the Procedural Authority governing Controlled Stage
Admission is the legitimate authority holder whose standing under governance
applicable to the Stage domain includes authority over the Controlled Stage
Admission operation.

FD-0028 established the bounded condition under which a particular authority
holder possesses that standing.

For Controlled Stage Admission, sufficient Procedural Authority standing
requires:

```text
Governance Legitimately Applicable
to the Stage Domain
        +
Legitimate Authority Holder
        +
Authority Scope Including
Controlled Stage Admission
        +
Applicability to the
Governed Operation
```

FD-0028 did not establish what evidence is sufficient to establish and preserve
that relationship for a particular admission.

The present investigation addresses that evidentiary dependency.

It does not determine what ultimately establishes the legitimacy of applicable
governance.

That deeper question remains deferred under FI-0006 unless its re-entry
condition is satisfied.

---

# Forge Investigation

## Strike 1 — Authority Holder Identity

Suppose an admission record identifies:

```text
PROCEDURAL_AUTHORITY=<identity>
```

This identifies an asserted authority holder.

It does not establish why that holder possesses Procedural Authority over
Controlled Stage Admission.

Therefore:

```text
Authority Identity Evidence
    ≠
Authority Standing Evidence
```

A particular identity is necessary where the governing authority is held by a
particular holder, but identity alone is insufficient evidence of standing.

---

## Strike 2 — Authority Declaration

Suppose the evidence identifies both a holder and an asserted scope:

```text
PROCEDURAL_AUTHORITY=<identity>
AUTHORITY_SCOPE=Controlled Stage Admission
```

This still does not establish that the claimed scope was legitimately granted
or recognized.

If an authority holder could establish standing merely by declaring that the
holder possesses the authority, an authority claim could manufacture its own
standing.

FD-0028 already established:

```text
Procedural Authority Claim
    ≠
Procedural Authority Standing
```

Therefore:

```text
Authority Claim
    ≠
Evidence Establishing Authority
```

Sufficient standing evidence cannot consist solely of an unsupported assertion
by the claimed authority holder.

---

## Strike 3 — Applicable Governance Basis

FD-0028 established that Procedural Authority standing must arise under
governance legitimately applicable to the Stage domain.

Evidence identifying only:

```text
Authority Holder
        +
Authority Scope
```

does not establish the governance relationship from which that authority
arises.

Without evidence of that relationship, an authority established by applicable
governance cannot be distinguished from an authority merely asserted by the
claimed holder.

Therefore sufficient standing evidence must establish the applicable governance
basis under which the claimed Procedural Authority standing arises.

This does not require reconstruction of the complete constitutive history of
that governance.

The bounded relationship required is:

```text
Applicable Governance
        |
        | establishes or recognizes
        v
Procedural Authority
```

---

## Strike 4 — Complete Governance Reconstruction

Must sufficient standing evidence reproduce the complete governing instrument
or the complete constitutive history of the applicable governance?

No such requirement has been established.

The evidentiary requirement is to establish the authority relationship required
for the bounded governed operation.

Depending upon the implementation and governance environment, that relationship
may be established through preserved governing evidence, a durable reference,
an authoritative record, or another legitimate evidentiary mechanism.

Therefore:

```text
Evidence of Governance Basis
    ≠
Complete Constitutive Governance History
```

The Stage Method must not require one particular technical or documentary
representation unless that representation becomes necessary to preserve the
required authority relationship.

---

## Strike 5 — Role-Based Authority

Procedural Authority may be established through an authorized role.

For example:

```text
Applicable Governance
        |
        v
Authorized Role
        |
        v
Authority Scope
```

Evidence that the role possesses authority does not establish which particular
holder legitimately occupies that role.

Likewise, evidence that a particular holder occupies a role does not establish
that the role possesses authority over Controlled Stage Admission.

FD-0028 established:

```text
Authority Role
    ≠
Particular Authority Holder

Role Occupancy
    ≠
Role Authority
```

Therefore, where Procedural Authority is role-based, sufficient standing
evidence must establish both:

1. that applicable governance establishes or recognizes the role and grants the
   required authority to that role; and
2. that the particular authority holder legitimately occupied that role when
   the governed admission occurred.

The role-occupancy evidence question exposed by FD-0028 is therefore a
conditional component of standing evidence whenever the governing authority is
role-based.

---

## Strike 6 — Direct Authority

Applicable governance may establish or recognize Procedural Authority directly
in a particular holder without using an intermediate role.

In that case the authority relationship may be:

```text
Applicable Governance
        |
        v
Particular Authority Holder
        |
        v
Authority Scope
```

The Stage Method must not manufacture a role merely to satisfy an evidentiary
structure designed for role-based authority.

Therefore:

> Where Procedural Authority is established directly in a particular holder,
> sufficient standing evidence does not require evidence of an intermediate
> authority role or role occupancy.

---

## Strike 7 — Authority Scope

Evidence that a particular holder possesses some Procedural Authority within a
Stage domain does not establish authority over Controlled Stage Admission.

FD-0028 established:

```text
Domain Procedural Authority
    ≠
Authority Over Every Domain Operation
```

Therefore sufficient standing evidence must establish that the authority scope
includes Controlled Stage Admission or a legitimately defined class of
operations that includes Controlled Stage Admission.

Authority identity without applicable authority scope is insufficient.

---

## Strike 8 — Applicability to the Particular Admission

Authority may exist during one period, project, Stage domain, operation class,
or other bounded condition and not another.

FD-0028 established:

```text
Historical Authority
    ≠
Necessarily Present Authority
```

Therefore sufficient standing evidence must establish that the authority
relationship was applicable to the particular Controlled Stage Admission when
that governed operation occurred.

The Stage Method does not require a timestamp as the universal mechanism for
establishing this relationship.

Applicability may be established through time, sequence, term, appointment,
version, project scope, continuing standing, contemporaneous evidence, or
another legitimate mechanism appropriate to the governing environment.

The requirement is the authority relationship, not a particular serialization.

---

## Strike 9 — Evidence Producer

The particular authority holder need not personally produce the evidence that
establishes the holder's standing.

The evidence may arise from governance records, institutional records,
authorized appointments, project records, registers, documented procedures,
paper instruments, or other legitimate evidentiary mechanisms.

Therefore:

```text
Authority Holder
    ≠
Necessarily Evidence Author
```

Requiring the claimed authority holder to author the evidence would
unnecessarily constrain legitimate governance arrangements and could encourage
circular self-attestation.

---

## Strike 10 — Evidence Does Not Create Standing

A record containing:

```text
PROCEDURAL_AUTHORITY=...
GOVERNANCE=...
AUTHORITY_SCOPE=...
APPLICABILITY=...
```

does not acquire constitutive authority merely because the record exists.

Procedural Authority standing arises from the applicable governance
relationship.

Evidence establishes or preserves that relationship for the governed
operation.

Therefore:

```text
Evidence of Standing
    ≠
Source of Standing
```

An evidentiary artifact must not be interpreted as manufacturing the authority
it records.

---

## Strike 11 — Standing Assertion Versus Standing Evidence

An unsupported statement that applicable governance grants authority remains an
assertion.

For evidence to establish standing rather than merely claim standing, the
required authority relationship must be determinable from evidence sufficient
under the applicable governance.

This does not inherently require:

- a digital signature;
- a cryptographic hash;
- a certificate;
- an external database;
- a third-party witness;
- a particular file format; or
- any other universal technical mechanism.

Therefore:

```text
Standing Assertion
    ≠
Standing Evidence
```

Sufficiency is determined by whether the evidence establishes the required
authority relationship under the governance applicable to the bounded
operation.

---

## Strike 12 — Establishment Versus Preservation

Evidence sufficient to establish standing when an admission occurs may cease to
be available later.

The authority holder may leave a role.

An appointment may expire.

Governance may change.

An external authority record may be replaced or become unavailable.

If the legitimacy of an admitted Stage depends entirely upon mutable present
state, the authority relationship governing the historical admission may no
longer be establishable.

Therefore:

```text
Present Standing
    ≠
Historical Evidence of Standing
```

A successful Controlled Stage Admission must preserve sufficient standing
evidence to establish the Procedural Authority relationship that governed that
admission after the authority relationship changes, expires, or otherwise
ceases to describe present authority.

---

## Strike 13 — Preservation Does Not Continue Authority

Preserving evidence that a holder possessed authority for a historical
admission must not imply that the holder continues to possess that authority.

Historical evidence records the authority relationship applicable to the
governed operation.

It does not perpetuate that relationship.

Therefore:

```text
Preserved Authority Evidence
    ≠
Continuing Authority
```

The preserved evidence remains historical provenance after the governed
operation.

---

## Strike 14 — Ultimate Governance Legitimacy

The present evidentiary structure requires sufficient evidence of:

```text
Applicable Governance
        |
        v
Authority Holder or Authorized Role
        |
        v
Authority Scope
        |
        v
Applicability to the
Particular Admission
```

Nothing demonstrated in this investigation requires resolution of what
ultimately establishes the constitutive legitimacy of the applicable
governance.

That deeper investigation remains preserved in FI-0006.

FI-0006's re-entry condition is not satisfied merely because sufficient
standing evidence must identify or establish the applicable governance basis.

Therefore:

> Evidence of the bounded governance relationship does not require complete
> reconstruction of the ultimate constitutive legitimacy of the governance
> unless that deeper question becomes a demonstrated blocking dependency.

---

# Standing Evidence Structure

For directly held Procedural Authority:

```text
Applicable Governance
        |
        | establishes or recognizes
        v
Particular Authority Holder
        |
        | possesses
        v
Authority Scope
        |
        | includes
        v
Controlled Stage Admission
        |
        | applicable to
        v
Particular Governed Admission
```

Sufficient evidence must establish and preserve this relationship.

For role-based Procedural Authority:

```text
Applicable Governance
        |
        | establishes or recognizes
        v
Authorized Role
        |
        | possesses
        v
Authority Scope
        |
        | includes
        v
Controlled Stage Admission

AND

Particular Authority Holder
        |
        | legitimately occupies
        v
Authorized Role
        |
        | applicable during
        v
Particular Governed Admission
```

Sufficient evidence must establish and preserve both relationships.

---

# Sufficient Standing Evidence Condition

Evidence is sufficient to establish and preserve Procedural Authority standing
for a particular Controlled Stage Admission when it establishes and preserves:

1. the governance basis legitimately applicable to the Stage domain;
2. the particular authority holder;
3. the relationship through which that holder possesses the governing
   Procedural Authority, whether directly or through a legitimately occupied
   role;
4. the authority scope that includes Controlled Stage Admission or a
   legitimately defined class containing it; and
5. the applicability of that authority relationship to the particular governed
   admission.

Where authority is role-based, sufficient evidence must additionally establish
both the authority granted to the role and the particular holder's legitimate
occupancy of that role for the governed operation.

The evidence need not reproduce the complete constitutive history of applicable
governance unless that deeper history becomes necessary to establish the
bounded authority relationship being relied upon.

---

# Consequences

A Controlled Stage Admission cannot establish sufficient Procedural Authority
standing merely by recording an authority identity.

Likewise, none of the following independently establishes sufficient standing
evidence:

- an authority claim;
- a holder identity;
- a role name;
- role occupancy;
- an unsupported authority scope;
- general authority within the Stage domain;
- execution of the admission procedure;
- control of the admission mechanism;
- authorship of the admission specification;
- custody of Stage artifacts; or
- an evidentiary record that merely declares its own authority.

Where the governing authority is role-based, role-occupancy evidence becomes a
required component of the standing evidence relationship.

Where the authority is directly held, an artificial role must not be required.

Evidence sufficient at the time of admission must be preserved sufficiently to
establish the historical authority relationship after present authority
changes.

Preserved historical standing evidence does not grant continuing authority.

---

# Does Not Establish

FD-0029 does not establish:

- the ultimate source of legitimate governance;
- what ultimately makes applicable governance legitimate;
- one universal governance structure for all Stage domains;
- one universal Procedural Authority;
- who presently possesses Procedural Authority for the Marlin Stage domain;
- that the Engineering Authority is also the Procedural Authority;
- that the same actor cannot legitimately occupy both authority roles;
- that Procedural Authority must be held through a role;
- that Procedural Authority must be held directly;
- one required identity representation;
- one required governance representation;
- one required role-occupancy representation;
- one required evidence format;
- that a timestamp is required;
- that a signature is required;
- that a hash is required;
- that an external authority registry is required;
- that evidence itself creates Procedural Authority standing;
- what establishes that the governing Controlled Stage Admission procedure is
  authorized by the governing Procedural Authority;
- how a particular procedural verification is connected to the authorized
  procedure and governing Procedural Authority;
- what exact portion of standing evidence must enter permanent Stage custody;
- whether the current Controlled Stage Admission specification sufficiently
  expresses this finding;
- how the current Stage admission adapter must implement this finding; or
- that FI-0006's re-entry condition has been satisfied.

---

# Depends On

FD-0029 directly depends upon:

- FD-0005 — Dual Authority
- FD-0013 — Controlled Stage Admission
- FD-0020 — Procedural Authority Legitimacy
- FD-0021 — Constitutive Authority Standing
- FD-0026 — Procedural Verification Attribution
- FD-0027 — Governing Procedural Authority for Controlled Stage Admission
- FD-0028 — Procedural Authority Standing for Controlled Stage Admission

FD-0022 — Authority Condition of a Discovery in Hold provides relevant
authority-boundary context but is not a direct dependency of the present
finding.

FI-0006 — Ultimate Legitimacy of Applicable Governance is related but is not a
direct dependency of FD-0029.

Its re-entry condition remains unsatisfied by the present investigation.

---

# Open Dependencies

FD-0029 leaves unresolved:

1. What establishes that the governing Controlled Stage Admission procedure is
   authorized by the governing Procedural Authority?
2. How must a particular procedural verification be connected to that
   authorized procedure and governing Procedural Authority?
3. What evidence is sufficient to establish and preserve legitimate role
   occupancy where the governing Procedural Authority is role-based?
4. Where the same actor occupies both Engineering Authority and Procedural
   Authority roles, what evidence is sufficient to preserve the distinction
   between those roles?
5. What portion of Procedural Authority standing evidence must enter permanent
   Stage custody upon successful Admission Commit?
6. How must preserved authority-standing evidence distinguish historical
   authority applicable to an admitted Stage from present or continuing
   authority?
7. Does the current Controlled Stage Admission specification sufficiently
   express the standing-evidence requirements established by this discovery?

The deeper question of the ultimate legitimacy of applicable governance remains
preserved in FI-0006 and SHALL NOT be reopened through these dependencies unless
FI-0006's re-entry condition is satisfied.

---

# Forge Finding

> **Evidence is sufficient to establish the Procedural Authority standing governing a particular Controlled Stage Admission when it establishes the applicable governance basis, the particular authority holder, the relationship by which that holder possesses the governing authority, the authority scope that includes Controlled Stage Admission, and the applicability of that authority to the particular admission being governed.**
>
> **Where authority is role-based, the evidence must additionally establish both the authority of the role and the particular holder's legitimate occupancy of that role. Where authority is established directly, no role relationship is required.**
>
> **Authority identity, authority assertion, role identity, role occupancy, general domain authority, procedural execution, mechanism control, specification authorship, custody, or unsupported declaration of scope does not independently establish sufficient standing evidence.**
>
> **Evidence of Procedural Authority standing establishes or preserves the governing authority relationship for the operation; the evidence does not itself create the authority it records.**
>
> **Sufficient standing evidence need not reproduce the complete constitutive history of applicable governance, provided that the bounded authority relationship required for the governed operation can be established without resolving that deeper dependency.**
>
> **The standing evidence applicable to a successful Controlled Stage Admission must be preserved sufficiently to establish the authority relationship that governed that admission after the relationship changes, expires, or otherwise ceases to describe present authority. Preservation of historical standing evidence does not confer continuing authority.**

---

# Invariants

```text
Authority Identity Evidence
    ≠
Authority Standing Evidence

Authority Claim
    ≠
Evidence Establishing Authority

Standing Assertion
    ≠
Standing Evidence

Evidence of Standing
    ≠
Source of Standing

Authority Role
    ≠
Particular Authority Holder

Role Occupancy
    ≠
Role Authority

Present Standing
    ≠
Historical Evidence of Standing

Preserved Authority Evidence
    ≠
Continuing Authority

Sufficient Standing Evidence
    ≠
Complete Constitutive Governance History
```

---

# Status

| Field | Value |
|---|---|
| Status | Accepted |
| Version | 1.0.0 |


FD-0029 survived Anvil inspection without a demonstrated crack.

The finding establishing the evidence sufficient to establish and preserve
Procedural Authority standing for a particular Controlled Stage Admission is
Accepted.

The Open Dependencies remain unresolved and are not established by this
acceptance.

---

# Version History

| Version | Status | Description |
|---|---|---|
| 0.1.0 | Hold | Initial memorialization of the Forge finding establishing the evidence required |
| | | to establish and preserve Procedural Authority standing for a particular |
| | | Controlled Stage Admission. |
| 1.0.0 | Accepted | Survived the Anvil inspection |

---

