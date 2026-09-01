# FD-0030 — Controlled Stage Admission Procedure Authorization

**Status:** Accepted
**Version:** 1.0.0

---

# Forge Question

What establishes that the governing Controlled Stage Admission procedure is
authorized?

---

# Context

FD-0026 established that procedural verification attribution requires a
relationship between the governing Procedural Authority, an authorized
procedure, and the particular verification performed.

FD-0027 established what Procedural Authority governs Controlled Stage
Admission.

FD-0028 established what constitutes legitimate Procedural Authority standing
for that operation.

FD-0029 established what evidence is sufficient to establish and preserve the
identity and standing of the governing Procedural Authority for a particular
Controlled Stage Admission.

That dependency chain exposed a remaining question.

Establishing legitimate Procedural Authority over Controlled Stage Admission
does not yet establish why a particular procedure is authorized to govern that
operation.

The unresolved relationship is:

```text
Applicable Governance
        |
        v
Procedural Authority Standing
        |
        | ?
        v
Governing Admission Procedure
```

The present investigation addresses the authorization of the procedure itself.

It does not yet establish what evidence is sufficient to preserve that
authorization for a particular admission.

It also does not establish how a particular procedural verification is connected
to the authorized procedure and governing Procedural Authority.

---

# Forge Investigation

## Strike 1 — Procedural Authority Standing Automatically Authorizes Procedure

Suppose the standing of the governing Procedural Authority has been completely
established:

```text
Applicable Governance
        |
        v
Procedural Authority
        |
        | scope includes
        v
Controlled Stage Admission
```

Does that automatically authorize whatever procedure the authority holder uses?

No.

Applicable governance may grant authority over Controlled Stage Admission while
also constraining how that authority may be exercised.

For example:

```text
Procedural Authority
has authority over
Controlled Stage Admission

BUT

Controlled Stage Admission
must follow Procedure A
```

Use of Procedure B does not become authorized merely because an otherwise
legitimate Procedural Authority used it.

Therefore:

```text
Procedural Authority Standing
    ≠
Procedure Authorization
```

Authority over the governed operation and authorization of the procedure
governing that operation are distinct relationships.

---

## Strike 2 — Procedure Authorship Establishes Authorization

Suppose the governing Procedural Authority authors the admission procedure.

Does authorship establish authorization?

Not necessarily.

An authority holder may possess authority over an operation without possessing
authority to define, adopt, approve, select, or otherwise authorize the
procedure governing that operation.

Conversely, a person or body may legitimately author a procedure without
possessing authority to authorize its use.

Therefore:

```text
Procedure Authorship
    ≠
Procedure Authorization
```

Authorship may be relevant within a particular governance arrangement, but
authorship alone cannot universally establish authorization.

---

## Strike 3 — Specification Existence Establishes Authorization

Suppose a specification accurately describes the Controlled Stage Admission
procedure.

Does existence of that specification establish that the procedure is
authorized?

No.

A specification can express a procedure without establishing the authority
relationship that gives the procedure governing force.

Therefore:

```text
Procedure Specification
    ≠
Procedure Authorization
```

The procedure expressed by a specification must possess authorization through
a legitimate governance relationship.

---

## Strike 4 — Correct Procedure Execution Establishes Authorization

Suppose a mechanism successfully performs every operation required by a
procedure.

Does successful execution establish that the procedure was authorized?

No.

An unauthorized procedure can be executed correctly.

Procedural correctness answers:

> Was the procedure performed correctly?

Procedure authorization answers:

> Was this procedure legitimately authorized to govern the operation?

Therefore:

```text
Procedure Execution
    ≠
Procedure Authorization
```

Correct execution cannot manufacture authorization.

---

## Strike 5 — Mechanism Control Establishes Authorization

Suppose an authority holder owns, controls, installs, invokes, or maintains the
mechanism that performs the admission procedure.

Does control of that mechanism establish authorization of the procedure?

No.

Control of an implementation mechanism does not independently establish the
authority relationship governing the procedure embodied by that mechanism.

Therefore:

```text
Mechanism Control
    ≠
Procedure Authorization
```

Otherwise possession or control of a procedural mechanism could manufacture
procedure authorization.

---

## Strike 6 — Procedural Authority Approval Is Always Sufficient

Suppose a legitimate Procedural Authority explicitly approves a procedure for
Controlled Stage Admission.

Is that approval necessarily sufficient?

No.

Applicable governance may grant an authority holder standing over Controlled
Stage Admission while reserving authority to define, adopt, approve, select, or
otherwise authorize its governing procedure.

Therefore:

```text
Authority Over Operation
    ≠
Necessarily Authority Over
Governing Procedure
```

Where an authority holder authorizes the governing procedure, authority to
perform that authorization must itself arise under governance legitimately
applicable to the Stage domain.

---

## Strike 7 — Distinct Authority Function Requires Distinct Authority Holder

Does the distinction between authority over the operation and authority over
its governing procedure require a separate authority holder?

No.

The same authority holder may legitimately possess both authority functions.

Applicable governance may instead establish the governing procedure directly.

Governance may also allocate procedure-authorizing authority through another
legitimate role, body, or authority holder.

Therefore:

```text
Distinct Authority Function
    ≠
Necessarily Distinct Authority Holder
```

The Stage Method must not manufacture a universal third authority merely because
procedure authorization is distinct from Procedural Authority standing.

The required distinction concerns authority functions, not a predetermined
organizational topology.

---

## Strike 8 — Applicable Governance May Directly Authorize the Procedure

Suppose governance legitimately applicable to the Stage domain establishes:

```text
Controlled Stage Admission
shall follow Procedure A.
```

Must a Procedural Authority separately authorize Procedure A?

No.

The procedure may already possess governing authorization through applicable
governance.

The authorization relationship can therefore take this form:

```text
Applicable Governance
        |
        | establishes / adopts / mandates
        v
Governing Admission Procedure
        |
        | governs
        v
Controlled Stage Admission
```

Procedure authorization does not universally require a separate act of approval
by the Procedural Authority governing the operation.

---

## Strike 9 — Applicable Governance May Establish Authorizing Authority

Applicable governance may instead establish authority under which an authority
holder authorizes the governing procedure.

The relationship can take this form:

```text
Applicable Governance
        |
        | establishes authority to
        | authorize procedure
        v
Authorized Authority Holder
        |
        | legitimately authorizes
        v
Governing Admission Procedure
        |
        | governs
        v
Controlled Stage Admission
```

This structure is also coherent.

In either structure, procedure authorization arises through governance
legitimately applicable to the Stage domain.

The exact governance topology may vary.

The authorization relationship must remain establishable.

---

## Strike 10 — Authorization Requires a Particular Phrase

Must authorization contain a literal declaration such as:

```text
THIS PROCEDURE IS AUTHORIZED
```

No.

Applicable governance may establish procedure authorization through adoption,
designation, incorporation, mandate, delegation, approval, selection, or
another legitimate governance action.

Therefore:

```text
Procedure Authorization
    ≠
Required Authorization Phrase
```

The Stage Method must require the authorization relationship rather than a
particular phrase used to express it.

---

## Strike 11 — Procedure Identity Is Irrelevant

Suppose applicable governance authorizes:

```text
The Stage Admission Procedure
```

but multiple materially different procedures claim that identity.

The authorization cannot reliably govern a particular operation unless the
procedure to which the authorization applies is sufficiently determinable.

Therefore:

> Procedure authorization requires sufficiently determinable procedure identity
> to distinguish the authorized procedure from materially different procedures.

This does not establish a universal requirement for:

- a filename;
- a version number;
- a cryptographic hash;
- a Git commit;
- a URL;
- a document identifier; or
- another particular technical representation.

Those may be implementation-specific mechanisms for establishing procedure
identity.

The required relationship is:

```text
Procedure Authorization
        |
        | applies to
        v
Determinable Governing Procedure
```

---

## Strike 12 — Authorization Automatically Follows Procedure Modification

Suppose Procedure P is legitimately authorized.

Procedure P is later materially modified.

Does authorization of the original procedure automatically authorize the
modified procedure?

No.

Otherwise authorization of one procedure could silently authorize arbitrary
future procedures.

Therefore:

```text
Authorization of Procedure P
    ≠
Authorization of Arbitrary
Modification of Procedure P
```

The procedure actually governing the operation must remain within the
authorization applicable to it.

---

## Strike 13 — Every Modification Necessarily Requires Reauthorization

Does the previous strike establish that every spelling correction, formatting
change, or other non-substantive modification necessarily requires a new
authorization?

No.

Whether a modification changes the identity or authorization condition of the
procedure depends upon the applicable governance and authorization
relationship.

The Stage Method therefore cannot infer a universal reauthorization boundary
merely from the existence of a modification.

The governing requirement remains:

> The procedure actually used must remain within the authorization applicable
> to it.

---

## Strike 14 — Later Authorization Automatically Authorizes Prior Execution

Suppose Procedure P was not authorized when an admission occurred.

The procedure is authorized afterward.

Does later authorization automatically establish that the earlier operation was
authorized?

No.

Authorization applicable after an operation does not automatically establish
authorization applicable to the earlier operation.

Therefore:

```text
Later Procedure Authorization
    ≠
Necessarily Prior Operational Authorization
```

This does not establish that retrospective authorization is impossible.

If applicable governance permits retrospective authorization, that authority
and its applicability would themselves require establishment.

The Stage Method does not assume retrospective authorization merely from later
authorization of the procedure.

---

## Strike 15 — Historical Authorization Establishes Present Authorization

Suppose Procedure P was authorized historically, but that authorization has
expired, been withdrawn, been superseded, or otherwise ceased to apply.

Does historical authorization establish authorization for a later operation?

No.

Therefore:

```text
Historical Procedure Authorization
    ≠
Necessarily Present Procedure Authorization
```

Authorization must be applicable to the procedure governing the particular
Controlled Stage Admission.

---

## Strike 16 — Authorization Evidence Creates Authorization

Suppose an artifact contains:

```text
PROCEDURE_AUTHORIZED=TRUE
```

Does existence of that record authorize the procedure?

No.

An assertion that a procedure is authorized does not create the authorization
relationship.

Therefore:

```text
Authorization Assertion
    ≠
Procedure Authorization
```

Likewise:

```text
Evidence of Procedure Authorization
    ≠
Source of Procedure Authorization
```

Evidence may establish or preserve an authorization relationship.

The evidence does not itself manufacture the authorization it records.

---

# Procedure Authorization Structure

The Forge exposed at least two legitimate forms by which Controlled Stage
Admission procedure authorization may arise.

Applicable governance may directly establish the governing procedure:

```text
Applicable Governance
        |
        | establishes / adopts / mandates
        v
Governing Admission Procedure
        |
        | governs
        v
Controlled Stage Admission
```

Alternatively, applicable governance may establish authority under which an
authority holder legitimately authorizes the governing procedure:

```text
Applicable Governance
        |
        | establishes authority to
        | authorize procedure
        v
Authorized Authority Holder
        |
        | legitimately authorizes
        v
Governing Admission Procedure
        |
        | governs
        v
Controlled Stage Admission
```

These structures do not exhaust every possible legitimate governance
arrangement.

The Stage Method does not require one universal organizational topology.

The essential structure is:

```text
Legitimate Governance Basis
        |
        v
Legitimate Procedure Authorization
        |
        v
Determinable Governing Procedure
        |
        v
Applicability to Particular
Controlled Stage Admission
```

---

# Procedure Authorization Condition

A procedure governing Controlled Stage Admission is authorized when governance
legitimately applicable to the Stage domain either:

1. establishes that procedure as governing Controlled Stage Admission; or
2. establishes authority under which that procedure is legitimately authorized;

and the resulting authorization:

3. applies to a sufficiently determinable governing procedure; and
4. applies to that procedure for the particular Controlled Stage Admission.

Where an authority holder exercises procedure-authorizing authority, that
authority must itself arise under governance legitimately applicable to the
Stage domain.

Authorization of one procedure does not automatically extend to materially
different procedures or to modifications outside the applicable authorization.

---

# Forge Finding

> **A procedure governing Controlled Stage Admission is authorized when
> governance legitimately applicable to the Stage domain either establishes
> that procedure as governing the operation or establishes authority under
> which that procedure is legitimately authorized, and that authorization
> applies to the determinable procedure governing the particular Controlled
> Stage Admission.**
>
> **Procedural Authority standing over Controlled Stage Admission does not by
> itself establish authority to define, adopt, approve, select, or otherwise
> authorize the procedure governing that operation. Where procedure
> authorization is exercised by an authority holder, that authority to
> authorize the procedure must itself arise under governance legitimately
> applicable to the Stage domain.**
>
> **Procedure authorship, specification existence, procedural correctness,
> procedural execution, mechanism control, custody, or an assertion that a
> procedure is authorized does not independently establish procedure
> authorization.**
>
> **Authorization must apply to the procedure actually governing the operation.
> Authorization of one procedure does not automatically authorize materially
> different procedures or later modifications outside the applicable
> authorization.**
>
> **Evidence of procedure authorization establishes or preserves the applicable
> authorization relationship; the evidence does not itself create the
> authorization it records.**

---

# Invariants

```text
Procedural Authority Standing
    ≠
Procedure Authorization

Authority Over Operation
    ≠
Necessarily Authority Over
Governing Procedure

Procedure Authorship
    ≠
Procedure Authorization

Procedure Specification
    ≠
Procedure Authorization

Procedure Execution
    ≠
Procedure Authorization

Mechanism Control
    ≠
Procedure Authorization

Distinct Authority Function
    ≠
Necessarily Distinct Authority Holder

Procedure Authorization
    ≠
Required Authorization Phrase

Authorization Assertion
    ≠
Procedure Authorization

Evidence of Procedure Authorization
    ≠
Source of Procedure Authorization

Authorization of Procedure P
    ≠
Authorization of Arbitrary
Modification of Procedure P

Later Procedure Authorization
    ≠
Necessarily Prior Operational Authorization

Historical Procedure Authorization
    ≠
Necessarily Present Procedure Authorization
```

---

# Does Not Establish

FD-0030 does not establish:

- the ultimate source of legitimate governance;
- what ultimately makes applicable governance legitimate;
- one universal governance structure for every Stage domain;
- one universal procedure-authorizing authority;
- that procedure-authorizing authority must be held by the governing
  Procedural Authority;
- that procedure-authorizing authority must be held by a different authority
  holder;
- that a third authority role is required;
- one required procedure-authorization mechanism;
- one required procedure-identity representation;
- that a filename is required to establish procedure identity;
- that a version number is required to establish procedure identity;
- that a cryptographic hash is required to establish procedure identity;
- that a Git commit is required to establish procedure identity;
- that every procedure modification requires reauthorization;
- what modifications remain within an existing authorization;
- that retrospective authorization is universally permitted;
- that retrospective authorization is universally prohibited;
- what evidence is sufficient to establish and preserve procedure
  authorization for a particular Controlled Stage Admission;
- how a particular procedural verification is connected to the authorized
  procedure and governing Procedural Authority;
- what procedure-authorization evidence must enter permanent Stage custody;
- whether the current Controlled Stage Admission specification sufficiently
  expresses the procedure-authorization requirement;
- whether any particular existing Controlled Stage Admission procedure is
  authorized;
- how a Stage admission adapter must represent procedure authorization; or
- that FI-0006's re-entry condition has been satisfied.

---

# Consequences

Legitimate Procedural Authority standing over Controlled Stage Admission does
not independently establish authorization of the procedure used to govern that
admission.

Applicable governance may authorize the governing procedure directly.

Applicable governance may instead establish authority under which an authority
holder legitimately authorizes the governing procedure.

The same authority holder may possess both authority over Controlled Stage
Admission and authority to authorize its governing procedure, but possession of
the first authority does not establish possession of the second.

The procedure governing a particular Controlled Stage Admission must be
sufficiently determinable and must remain within the authorization applicable
to that operation.

Procedure authorization therefore becomes a distinct dependency in establishing
the procedural provenance of Controlled Stage Admission.

---

# Open Dependencies

FD-0030 leaves unresolved:

1. What evidence is sufficient to establish and preserve authorization of the
   governing Controlled Stage Admission procedure for a particular admission?
2. How must a particular procedural verification be connected to the authorized
   procedure and governing Procedural Authority?
3. What evidence is sufficient where procedure-authorizing authority is
   delegated to or exercised through a role?
4. How must procedure identity be preserved sufficiently to establish which
   procedure was authorized for a historical admission?
5. What determines whether a modification remains within the authorization of
   an already authorized procedure?
6. What portion of procedure-authorization evidence must enter permanent Stage
   custody upon successful Admission Commit?
7. Where the same authority holder possesses authority over Controlled Stage
   Admission and authority to authorize its governing procedure, what evidence
   is sufficient to preserve those distinct authority functions?
8. Does the current Controlled Stage Admission specification sufficiently
   express the procedure-authorization requirements established by this
   discovery?

FI-0006 — Ultimate Legitimacy of Applicable Governance remains deferred.

The present investigation does not demonstrate an engineering dependency that
requires resolution of FI-0006 in order to establish the bounded procedure
authorization relationship identified here.

Its re-entry condition therefore remains unsatisfied.

---

# Depends On

FD-0030 directly depends upon:

- FD-0013 — Controlled Stage Admission
- FD-0020 — Procedural Authority Legitimacy
- FD-0021 — Constitutive Authority Standing
- FD-0026 — Procedural Verification Attribution
- FD-0027 — Governing Procedural Authority for Controlled Stage Admission
- FD-0028 — Procedural Authority Standing for Controlled Stage Admission
- FD-0029 — Procedural Authority Standing Evidence for Controlled Stage
  Admission

FI-0006 — Ultimate Legitimacy of Applicable Governance is related but is not a
direct dependency of FD-0030.

Its re-entry condition remains unsatisfied by the present investigation.

---

# Status

| Field | Value |
|---|---|
| Status | Accepted |
| Version | 1.0.0 |

FD-0030 memorializes the Forge finding concerning authorization of the procedure
governing Controlled Stage Admission.

The finding survived Anvil inspection and is Accepted.

The Open Dependencies remain unresolved and are not established by this
finding.

---

# Version History

| Version | Status | Description |
|---|---|---|
| 0.1.0 | Hold | Initial memorialization of the Forge finding establishing |
| | | authorization of the procedure governing Controlled Stage Admission. |
| 1.0.0 | Accepted | Survived Anvil inspection and accepted as a canonical |
| | | Forge Discovery. |

---

