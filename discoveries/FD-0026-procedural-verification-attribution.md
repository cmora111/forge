# FD-0026 — Procedural Verification Attribution

**Status:** Accepted
**Version:** 1.0.0

---

# Forge Question

What must be established for a procedural verification performed through an
authorized procedure to be attributable to the governing Procedural Authority?

---

# Context

Controlled Stage Admission requires Procedural Authority verification before
Admission Commit.

During implementation of Controlled Stage Admission, the Stage admission
adapter reached a point where it could:

- collect and preserve Engineering Authority determinations;
- construct proposed admission evidence;
- perform procedural verification;
- preserve the exact evidence that passed verification;
- prepare a complete admission result outside authoritative Stage custody;
- publish that result into authoritative Stage custody;
- establish the initial ACTIVE lifecycle representation through Admission
  Commit;
- distinguish pre-commit failure from post-commit failure; and
- prevent post-commit cleanup from rolling back an authoritative publication.

The resulting adapter was sent to the Anvil.

The Admission Commit mechanics, exact-evidence boundary, publication boundary,
cleanup and non-rollback behavior, and lifecycle representation survived
adversarial inspection.

The Anvil exposed a remaining crack in procedural provenance.

The adapter could record that procedural verification had passed and identify
the mechanism through which that verification was performed:

```text
PROCEDURAL_VERIFICATION=PASSED
VERIFIED_EVIDENCE_RECORD=VERIFIED-EVIDENCE-MANIFEST
PROCEDURAL_MECHANISM=new-stage.sh
EVIDENCE_INTEGRITY=PASSED
```

This established that a particular procedural mechanism performed particular
verification operations.

It did not establish why the resulting verification was attributable to the
governing Procedural Authority.

The crack was therefore returned to the Forge rather than repaired directly in
the adapter.

---

# Procedural Correctness Does Not Establish Procedural Authority

A procedure may be performed correctly without establishing the authority
under which the procedure is performed.

Successful execution may establish that:

- required checks were performed;
- those checks produced a particular result;
- evidence passed those checks; and
- the procedural mechanism behaved according to its implementation.

Those facts do not independently establish that the verification was performed
under legitimate Procedural Authority.

Therefore:

> **Procedural Correctness ≠ Procedural Authority**

Correct execution is necessary where the governing procedure requires it.

Correct execution is not the source of the authority governing that procedure.

---

# Procedural Mechanism Does Not Establish Procedural Authority

A procedural mechanism may perform verification operations.

Examples of such mechanisms may include:

- a shell script;
- a graphical application;
- a workbook;
- a paper checklist;
- a field procedure;
- or another implementation capable of carrying out the applicable procedural
  requirements.

Performance of those operations does not make the mechanism the source of
Procedural Authority.

Therefore, replacing:

```text
PROCEDURAL_MECHANISM=new-stage.sh
```

with:

```text
PROCEDURAL_AUTHORITY=new-stage.sh
```

would not establish the missing authority relationship.

It would merely rename the mechanism as the authority without establishing why
the mechanism possesses authority.

Therefore:

> **Procedural Mechanism ≠ Procedural Authority**

The mechanism is an instrument through which authorized procedure may be
performed.

---

# Execution Does Not Establish Standing

The person or mechanism capable of invoking or executing a procedure does not
acquire Procedural Authority merely by performing it.

Otherwise, the ability to execute a procedure would itself establish standing
to govern the procedure.

That would allow procedural authority to arise from execution alone.

Therefore:

> **Procedural Execution ≠ Procedural Standing**

Execution may be an act performed under authority.

Execution does not independently establish the authority under which the act is
performed.

---

# Engineering Authority Does Not Substitute for Procedural Authority

Engineering Authority and Procedural Authority perform distinct functions.

Engineering Authority supplies substantive engineering determinations.

Procedural Authority governs whether the applicable procedural requirements
have been satisfied.

A single person, institution, or other legitimate authority holder may occupy
both roles.

Coincidence of identity does not collapse the roles.

Standing as Engineering Authority does not automatically establish standing as
Procedural Authority, and attribution of Engineering Authority determinations
does not automatically establish attribution of Procedural Authority
verification.

Therefore:

> **Engineering Authority Standing ≠ Procedural Authority Standing**

Where one actor occupies both roles, the authority relationship applicable to
each role must remain distinguishable.

---

# Specification Does Not Become Procedural Authority

A specification may define the requirements governing a procedural operation.

The existence of those requirements does not make the specification itself the
Procedural Authority.

A specification describes or establishes the procedure to be followed within
the authority structure applicable to it.

It does not acquire authority merely because procedural requirements are
written within it.

Therefore:

> **Governing Specification ≠ Governing Procedural Authority**

However, a legitimate Procedural Authority may authorize a procedure expressed
through a governing specification.

The distinction is between the authority and the procedural expression through
which that authority governs an operation.

---

# Authority May Operate Through Procedure

Procedural Authority need not personally perform every mechanical verification
operation.

A legitimate Procedural Authority may govern a procedural operation through an
authorized procedure.

That procedure may in turn be realized through an authorized procedural
mechanism.

The relevant relationship is:

```text
Governing Procedural Authority
             |
             | authorizes
             v
      Governing Procedure
             |
             | realized through
             v
     Procedural Mechanism
             |
             | performs
             v
   Particular Verification
             |
             | produces
             v
Procedural Verification Evidence
```

The procedural mechanism therefore need not itself possess Procedural
Authority.

The particular verification must instead occur within an authority relationship
sufficient to make that verification attributable to the governing Procedural
Authority.

---

# Authorization Must Apply to the Procedure Actually Performed

The existence of a Procedural Authority is not sufficient by itself.

The authority relationship must extend to the procedure under which the
particular verification is performed.

Likewise, authorization of one procedural mechanism or implementation does not
automatically authorize every later mechanism or every later modification
bearing the same name.

A claim such as:

```text
new-stage.sh is authorized
```

cannot by itself establish that every artifact subsequently named
`new-stage.sh` remains within that authorization.

The verification must be attributable to the governing Procedural Authority
through the procedure actually applicable to the verification being performed.

Therefore:

> **Authority Existence ≠ Authorization of Every Procedure**

and:

> **Mechanism Identity ≠ Continuing Authorization**

The exact means by which an implementation establishes the identity or
applicability of an authorized procedure is an operational question distinct
from the authority relationship established by this finding.

---

# Procedural Verification Attribution

A procedural verification becomes attributable to a governing Procedural
Authority when sufficient provenance establishes that the particular
verification was performed under a procedure legitimately authorized by that
Procedural Authority.

The required relationship is therefore not merely:

```text
Mechanism
    ↓
Verification
```

but:

```text
Procedural Authority
        ↓
Authorized Procedure
        ↓
Particular Verification
```

with the procedural mechanism acting as the means through which that authorized
procedure is performed where such a mechanism is used.

This establishes the distinction:

> **Verification Occurrence ≠ Verification Attribution**

Evidence that verification occurred answers whether a procedural act took
place.

Procedural attribution answers under whose legitimate procedural authority
that act was performed.

Both may be required for sufficient procedural provenance.

---

# Procedural Provenance

Procedural verification evidence is not sufficient merely because it records
that verification occurred.

For the verification to be attributable to the governing Procedural Authority,
sufficient provenance must preserve the relationship among:

1. the governing Procedural Authority;
2. the procedure authorized by that authority; and
3. the particular procedural verification performed under that authorization.

Where a procedural mechanism is used, provenance may also identify the
mechanism through which the authorized procedure was performed.

Identification of that mechanism does not substitute for identification of the
authority relationship.

Therefore:

```text
Procedural Mechanism Identification
                +
Procedural Verification Result
```

does not necessarily establish:

```text
Procedural Authority Attribution
```

unless the applicable authorization relationship is also sufficiently
established.

---

# Bounded Authority Provenance

Procedural provenance need not reproduce the complete constitutive history of
the governing Procedural Authority for every procedural act.

Requiring every Stage operation to reconstruct the entire authority dependency
chain would make bounded engineering operations depend upon repeatedly solving
questions already outside the immediate engineering boundary.

Instead, the procedural record must preserve sufficient provenance to establish
the authority relationship applicable to the bounded procedural operation being
performed.

Therefore:

> **Sufficient Procedural Attribution ≠ Complete Reconstruction of Constitutive Authority**

This does not waive the requirement for legitimate Procedural Authority.

It establishes only that the evidence necessary for a bounded procedural act
need not reproduce every deeper dependency from which that authority ultimately
derives.

Where a deeper authority dependency becomes necessary to determine whether the
claimed Procedural Authority is legitimate, that dependency remains subject to
separate investigation.

---

# Consequences for Controlled Stage Admission

Controlled Stage Admission cannot establish sufficient procedural provenance
merely by recording that an admission adapter performed its checks.

A record such as:

```text
PROCEDURAL_VERIFICATION=PASSED
PROCEDURAL_MECHANISM=new-stage.sh
```

may establish procedural occurrence and mechanism identity.

It does not, by itself, establish Procedural Authority attribution.

An admission implementation must preserve sufficient evidence connecting the
particular verification to the governing Procedural Authority through the
authorized procedure under which that verification was performed.

This finding does not prescribe a particular serialization, file format,
software architecture, signature mechanism, identity mechanism, or storage
medium for establishing that relationship.

Those are matters for Stage operationalization after the authority requirement
has survived adversarial inspection.

---

# Does Not Establish

FD-0026 does not establish:

- the identity of the governing Procedural Authority for Controlled Stage
  Admission;
- that any particular person, organization, software artifact, repository
  owner, operator, or mechanism possesses Procedural Authority;
- the constitutive source from which a particular Procedural Authority derives
  legitimate standing;
- that Engineering Authority automatically possesses Procedural Authority;
- that the operator of a procedural mechanism possesses Procedural Authority;
- that a procedural mechanism can authorize itself;
- the complete requirements for establishing Procedural Authority legitimacy;
- the exact mechanism by which an authorized procedure must be identified;
- the exact evidence required to prove that a particular mechanism implements
  an authorized procedure;
- the exact serialization required for Procedural Authority provenance;
- that a commit timestamp, signature, hash, identity token, or other particular
  technical mechanism is required;
- that the current Stage admission adapter already establishes sufficient
  Procedural Authority provenance;
- that the current Stage admission adapter must be modified in any particular
  way.

---

# Depends On

FD-0026 depends upon the authority distinctions established or investigated in:

- FD-0020 — Procedural Authority Legitimacy
- FD-0021 — Constitutive Authority Standing

It also operates within the bounded authority condition investigated in:

- FD-0022 — Authority Condition of a Discovery in Hold

These dependencies identify the authority distinctions necessary to state the
present finding.

---

# Open Dependencies

FD-0026 leaves unresolved:

1. What Procedural Authority governs Controlled Stage Admission?
2. What establishes that the governing Stage admission procedure is authorized
   by that Procedural Authority?
3. What evidence is sufficient to preserve that authorization relationship for
   a particular admission verification?
4. How must an implementation establish that the procedural mechanism actually
   used corresponds to the authorized procedure?
5. When the same actor occupies Engineering Authority and Procedural Authority
   roles, what evidence is sufficient to preserve the distinction between those
   roles?
6. What procedural provenance must enter permanent Stage custody upon successful
   Admission Commit?
7. Whether the current Controlled Stage Admission specification sufficiently
   expresses the attribution requirement established by this finding.

These questions belong to subsequent Forge investigation, Anvil inspection, or
Stage operationalization according to whether they become blocking
dependencies.

---

# Forge Finding

> **Procedural verification is attributable to a governing Procedural Authority when sufficient provenance establishes that the particular verification was performed under a procedure legitimately authorized by that Procedural Authority.**
>
> **Procedural correctness, procedural execution, and procedural mechanism identity do not independently establish Procedural Authority or Procedural Authority attribution.**
>
> **Procedural provenance must preserve sufficient evidence connecting the governing Procedural Authority, the authorized procedure, and the particular verification performed under that authorization.**
>
> **A procedural mechanism may perform an authorized procedure without itself being the source of the authority governing that procedure.**
>
> **The same actor may occupy Engineering Authority and Procedural Authority roles, but standing and attribution in one role do not automatically establish standing or attribution in the other.**
>
> **For a bounded engineering operation, sufficient procedural attribution does not require reconstruction of the complete constitutive history of Procedural Authority unless that deeper dependency becomes necessary to establish the legitimacy of the authority being relied upon.**

## Invariants

```text
Procedural Correctness ≠ Procedural Authority

Procedural Mechanism ≠ Procedural Authority

Procedural Execution ≠ Procedural Standing

Engineering Authority Standing ≠ Procedural Authority Standing

Governing Specification ≠ Governing Procedural Authority

Verification Occurrence ≠ Verification Attribution

Authority Existence ≠ Authorization of Every Procedure

Mechanism Identity ≠ Continuing Authorization

Procedural Mechanism Identification
        ≠
Procedural Authority Attribution

Sufficient Procedural Attribution
        ≠
Complete Reconstruction of Constitutive Authority
```

---

# Status

| Field | Value |
|---|---|
| Status | Accepted |
| Version | 1.0.0 |


FD-0026 survived Anvil inspection without a demonstrated crack.

The finding establishing the conditions under which procedural verification
may be attributed to governing Procedural Authority is Accepted.

The unresolved questions identified under Open Dependencies remain unresolved
and are not established by this acceptance.

---

# Version History

| Version | Status | Description |
|---|---|---|
| 0.1.0 | Hold | Initial memorialization of the Forge finding establishing the conditions under |
| | | which procedural verification may be attributed to governing Procedural Authority. |
| 1.0.0 | Accepted | Finding survived Anvil inspection without a demonstrated crack. |


---

