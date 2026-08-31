# FD-0028 — Procedural Authority Standing for Controlled Stage Admission

**Status:** Accepted
**Version:** 1.0.0

---

# Question

What establishes that a particular authority holder possesses legitimate
Procedural Authority over Controlled Stage Admission within a Stage domain?

---

# Context

FD-0027 — Governing Procedural Authority for Controlled Stage Admission
identified the structural condition for the Procedural Authority governing a
Controlled Stage Admission.

It established that the governing Procedural Authority is the legitimate
authority holder whose standing under governance applicable to the Stage
domain includes authority over the Controlled Stage Admission operation.

That finding identifies the required authority relationship but does not by
itself establish how a particular authority holder obtains that standing.

The resulting dependency is:

```text
Controlled Stage Admission
        |
        v
Governing Procedural Authority
        |
        v
Particular Authority Holder
        |
        | standing established by
        v
?
```

This discovery investigates that bounded question.

It does not investigate the ultimate legitimacy of the governance under which
that authority standing arises.

That deeper question is preserved separately as:

- FI-0006 — Ultimate Legitimacy of Applicable Governance

---

# Forge Investigation

## Strike 1 — Can an Authority Holder Establish Their Own Standing?

Suppose an authority holder declares:

```text
I possess Procedural Authority
over Controlled Stage Admission.
```

The declaration identifies a claimed authority relationship.

It does not establish that relationship.

If assertion alone established standing, any actor could acquire Procedural
Authority merely by claiming it.

Therefore:

> **Procedural Authority Claim ≠ Procedural Authority Standing**

A source other than the authority claim itself is required to establish the
standing claimed.

---

## Strike 2 — Can Applicable Governance Establish the Standing?

Suppose governance applicable to the Stage domain establishes or recognizes:

```text
Authority Holder
        |
        | possesses authority over
        v
Controlled Stage Admission
```

This differs materially from self-assertion.

The authority relationship now arises through governance applicable to the
Stage domain rather than solely through the authority holder's own claim.

For that relationship to establish the required standing, it must establish
both:

```text
Authority Identity
        +
Authority Scope
```

Knowing who the authority holder is does not establish what that authority is
authorized to govern.

Likewise, knowing that an authority role exists does not identify the
particular holder exercising that authority.

Therefore:

> **Authority Identity ≠ Authority Scope**

Sufficient standing for Controlled Stage Admission requires both an authority
holder and authority scope applicable to the admission operation.

---

## Strike 3 — Must Governance Name a Particular Person?

No.

Governance may establish authority through a role rather than by permanently
naming an individual.

For example:

```text
Applicable Governance
        |
        | establishes authority of
        v
Procedural Authority Role
        |
        | legitimately occupied by
        v
Particular Authority Holder
```

The role may possess authority over Controlled Stage Admission while different
holders occupy that role over time.

However, the existence of the role does not by itself establish that a
particular actor occupies it.

Therefore:

> **Authority Role ≠ Particular Authority Holder**

Where authority is role-based, the relationship between the particular
authority holder and the governing role must also be established.

---

## Strike 4 — Does Occupying a Role Establish the Authority of the Role?

No.

An actor may legitimately occupy a role without that role possessing authority
over Controlled Stage Admission.

For example:

```text
Actor
    |
    | legitimately occupies
    v
Project Role
```

does not establish:

```text
Project Role
    |
    | possesses authority over
    v
Controlled Stage Admission
```

The authority of the role and the occupancy of the role are distinct
relationships.

Therefore:

> **Role Occupancy ≠ Role Authority**

Where Procedural Authority is role-based, sufficient standing requires both:

1. establishment that the role possesses authority applicable to Controlled
   Stage Admission; and
2. establishment that the particular authority holder legitimately occupies
   that role.

---

## Strike 5 — Must Procedural Authority Be Permanent?

No.

Nothing in Controlled Stage Admission requires the governing Procedural
Authority to possess permanent authority.

Authority may be:

- standing;
- temporary;
- role-based;
- project-bounded;
- domain-bounded;
- operation-bounded; or
- otherwise legitimately limited.

The relevant requirement is not permanence.

The relevant requirement is applicability to the governed operation.

Therefore:

> **Legitimate Procedural Authority ≠ Necessarily Permanent Procedural
> Authority**

A temporary or bounded authority may possess sufficient standing if that
authority legitimately applies to the Stage domain and Controlled Stage
Admission when the governed operation occurs.

---

## Strike 6 — Is a Separate Authorization Required for Every Admission?

Not necessarily.

Applicable governance may establish standing authority over a class of
Controlled Stage Admissions.

For example:

```text
Applicable Governance
        |
        | establishes
        v
Procedural Authority
        |
        | authorized for
        v
Controlled Stage Admissions
within the Stage Domain
```

If that standing authority legitimately includes a particular admission, a
new grant of authority for every individual execution is not inherently
required.

Therefore:

> **Legitimate Standing Authority May Govern Multiple Admissions**

This does not establish that every standing authorization applies to every
admission.

The particular admission must remain within the authority's legitimate scope.

---

## Strike 7 — Is General Domain Authority Sufficient?

No.

An authority holder may possess legitimate authority within a Stage domain
without possessing authority over every operation in that domain.

For example:

```text
Legitimate Domain Authority
        ≠
Authority Over Every
Stage Method Operation
```

The authority granted must include the operation being governed.

For this discovery, that operation is:

```text
Controlled Stage Admission
```

Therefore:

> **Domain Authority ≠ Controlled Stage Admission Authority**

The scope of the Procedural Authority must apply specifically to Controlled
Stage Admission or to a class of operations that legitimately includes it.

---

## Strike 8 — Must Authority Be Applicable When the Operation Occurs?

Yes.

An authority relationship that existed previously but no longer applies
cannot establish standing for a later operation merely because it once
existed.

Likewise, authority established only after an admission cannot retroactively
serve as the governing authority for that admission merely by being recorded
later.

The authority relationship must be applicable to the governed operation when
that operation is performed.

Therefore:

> **Historical Authority ≠ Necessarily Present Authority**

and:

> **Future Authority ≠ Prior Governing Authority**

Sufficient standing requires authority applicable to the particular governed
operation.

---

## Strike 9 — Does the Identity Form Determine Standing?

No.

A Procedural Authority might be represented as:

- a named person;
- an organizational role;
- a project role;
- an institution;
- a governing body; or
- another authority form recognized by the applicable governance.

The representation does not itself establish authority.

Therefore:

> **Procedural Authority Identity Form ≠ Procedural Authority Standing**

The relevant question remains whether the identified authority possesses the
required legitimate standing for the governed operation.

---

## Strike 10 — Does This Require Resolving Ultimate Governance Legitimacy?

The investigation now reaches a deeper question:

```text
Procedural Authority
        |
        | obtains standing under
        v
Applicable Governance
        |
        | legitimacy established by
        v
?
```

That question is legitimate.

It is not presently demonstrated to block the bounded engineering problem
being investigated here.

The present problem requires sufficient legitimate Procedural Authority for
Controlled Stage Admission.

It does not presently require a universal theory of governance legitimacy or
resolution of every constitutive authority dependency.

Therefore:

> **Interesting Dependency ≠ Blocking Dependency**

and:

> **Unresolved Question ≠ Required Present Investigation**

The deeper question is preserved as:

- FI-0006 — Ultimate Legitimacy of Applicable Governance

FI-0006 may re-enter active investigation only under its defined re-entry
condition.

FD-0028 does not resolve that question.

---

# Positive Standing Structure

The investigation supports the following bounded structure:

```text
Governance Legitimately Applicable
to the Stage Domain
        |
        | establishes or recognizes
        v
Procedural Authority
        |
        | held directly or through
        | a legitimately occupied role
        v
Particular Authority Holder
        |
        | authority scope includes
        v
Controlled Stage Admission
        |
        | authority applicable to
        v
Particular Governed Operation
```

Where authority is assigned directly to a particular holder, no separate
role-occupancy relationship is required.

Where authority is role-based, both the authority of the role and the
particular holder's legitimate occupancy of that role must be established.

---

# Sufficient Standing Condition

For the bounded Controlled Stage Admission operation investigated here,
sufficient Procedural Authority standing requires establishment that:

1. governance legitimately applicable to the Stage domain establishes or
   recognizes the relevant Procedural Authority;

2. the particular authority holder is connected to that authority either
   directly or through legitimate occupancy of an authorized role;

3. the authority scope includes Controlled Stage Admission or a class of
   operations that legitimately includes Controlled Stage Admission; and

4. the authority is applicable to the particular admission operation being
   governed.

This establishes the authority relationship required for the bounded
operation.

It does not establish the ultimate constitutive legitimacy of the governance
from which that relationship arises.

---

# Consequences

If FD-0028 is accepted, then a Controlled Stage Admission cannot establish
governing Procedural Authority merely by recording:

```text
PROCEDURAL_AUTHORITY=<identity>
```

unless the required standing relationship is also established.

Likewise, none of the following alone is sufficient:

```text
Authority Holder Identity
Authority Claim
Role Name
Role Occupancy
General Domain Authority
Historical Authority
Procedural Execution
Procedural Mechanism
Admission Specification
Artifact Custody
```

The Stage Method must distinguish:

```text
Who the authority holder is
```

from:

```text
Why that holder possesses authority
over the operation being governed
```

and from:

```text
What operation that authority
legitimately covers
```

This distinction is necessary if later procedural verification is to be
attributable to a governing Procedural Authority rather than merely to a
mechanism or executor.

---

# Does Not Establish

FD-0028 does not establish:

- the ultimate source of legitimate governance;
- what ultimately makes governance legitimate;
- a universal governance structure for every Stage domain;
- one universal Procedural Authority for the Stage Method;
- that the Stage Method creator is the governing Procedural Authority;
- that Engineering Authority is Procedural Authority;
- that the same actor may not legitimately occupy both EA and PA roles;
- that a Procedural Authority must be a person;
- that a Procedural Authority must be an institution;
- that Procedural Authority must be permanent;
- that every admission requires a new authority grant;
- that possession of a role establishes the authority of that role;
- that authority over one Stage Method operation establishes authority over
  every Stage Method operation;
- what evidence is sufficient to preserve the standing relationship;
- what evidence is sufficient to preserve role occupancy;
- how procedural verification must record its attribution to the governing
  Procedural Authority;
- how the governing admission procedure is authorized by that Procedural
  Authority;
- that the current Marlin Controlled Stage Admission already possesses an
  established governing Procedural Authority; or
- that FI-0006 has satisfied its re-entry condition.

---

# Depends On

FD-0028 directly depends on:

- FD-0005 — Dual Authority
- FD-0013 — Controlled Stage Admission
- FD-0020 — Procedural Authority Legitimacy
- FD-0021 — Constitutive Authority Standing
- FD-0026 — Procedural Verification Attribution
- FD-0027 — Governing Procedural Authority for Controlled Stage Admission

It also operates within the bounded authority condition investigated in:

- FD-0022 — Authority Condition of a Discovery in Hold

FI-0006 — Ultimate Legitimacy of Applicable Governance is related to the
boundary exposed by this discovery but is not a direct dependency of FD-0028.

---

# Open Dependencies

FD-0028 exposes but does not answer:

1. What evidence is sufficient to establish and preserve the identity and
   standing of the governing Procedural Authority for a particular Controlled
   Stage Admission?

2. Where authority is role-based, what evidence is sufficient to establish
   and preserve legitimate occupancy of the governing authority role?

3. What establishes that the governing Controlled Stage Admission procedure
   is authorized by the governing Procedural Authority?

4. How must a particular procedural verification be connected to that
   authorized procedure and governing Procedural Authority?

5. Where the same actor occupies both Engineering Authority and Procedural
   Authority roles, what evidence is sufficient to preserve the distinction
   between those roles?

6. What portion of the authority-standing relationship must enter permanent
   Stage custody upon successful Admission Commit?

7. Does the current Controlled Stage Admission specification sufficiently
   express the authority-standing requirements established by this discovery?

The deeper question of the ultimate legitimacy of applicable governance is
preserved in FI-0006 and SHALL NOT be reopened through these dependencies
unless FI-0006's re-entry condition is satisfied.

---

# Forge Finding

A particular authority holder possesses Procedural Authority over Controlled
Stage Admission when governance legitimately applicable to the Stage domain
establishes or recognizes that authority holder, directly or through a
legitimately occupied role, and the authority granted includes the Controlled
Stage Admission operation being governed.

The authority relationship must establish both authority identity and
applicable authority scope. Mere identity, assertion, execution, mechanism
control, specification authorship, custody, or possession of a role name does
not establish the required standing.

The authority may be standing, temporary, role-based, or otherwise bounded,
provided that it legitimately applies to the Stage domain and Controlled Stage
Admission when the governed operation occurs.

Establishing sufficient authority standing for this bounded engineering
operation does not require resolution of the ultimate constitutive legitimacy
of every authority in the governance chain unless that deeper question becomes
a demonstrated blocking dependency.

---

# Invariants

```text
Procedural Authority Claim
    ≠
Procedural Authority Standing
```

```text
Authority Identity
    ≠
Authority Scope
```

```text
Authority Role
    ≠
Particular Authority Holder
```

```text
Role Occupancy
    ≠
Role Authority
```

```text
Domain Procedural Authority
    ≠
Authority Over Every Domain Operation
```

```text
Historical Authority
    ≠
Necessarily Present Authority
```

```text
Procedural Authority Identity Form
    ≠
Procedural Authority Standing
```

```text
Legitimate Procedural Authority
    ≠
Necessarily Permanent Procedural Authority
```

```text
Sufficient Controlled Stage Admission
Procedural Authority Standing
    =
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

---

# Status

| Field | Value |
|---|---|
| Status | Accepted |
| Version | 1.0.0 |


FD-0028 survived Anvil inspection without a demonstrated crack.

The finding establishing the bounded condition for sufficient Procedural
Authority standing over Controlled Stage Admission is Accepted.

The Open Dependencies remain unresolved and are not established by this
acceptance.

---

# Version History

| Version | Status | Description |
|---|---|---|
| 0.1.0 | Hold | Initial memorialization of the Forge finding establishing the bounded |
| | | standing condition for a particular Procedural Authority governing |
| | | Controlled Stage Admission. |
| 1.0.0 | Accepted | Has passed the anvil inspection. |

---

