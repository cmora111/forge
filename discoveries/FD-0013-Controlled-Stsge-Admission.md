# FD-0013 — Controlled Stage Admission

**Status:** Accepted
**Version:** 1.0.0

---

# Context

Stage Origination and Stage Succession are the recognized means by which a
proposed Stage enters the Stage lifecycle as `ACTIVE`.

FD-0011 establishes the authority and minimum evidence required for
Origination.

FD-0012 establishes the authority and minimum evidence required for
Succession.

Both require Engineering Authority determinations and Procedural Authority
verification before legitimate Stage admission may occur.

This creates an operational question.

Required Engineering Authority evidence must exist before Procedural Authority
can determine whether the applicable admission requirements have been
satisfied.

However, requiring that evidence to exist does not require the proposed Stage
itself to possess lifecycle authority before admission.

A mechanism performing Stage admission may therefore need to:

- solicit required Engineering Authority determinations,
- record those determinations,
- construct proposed Stage artifacts,
- verify the applicable procedural requirements, and
- give lifecycle effect to authorized Origination or Succession.

The relationship between these activities must preserve Dual Authority and
Lifecycle Determinism.

In particular, the mechanism used to collect or record Engineering Authority
determinations must not become the source of those determinations, and the
physical existence of proposed Stage artifacts must not itself create a Stage.

Therefore the controlled boundary through which proposed engineering evidence
becomes authoritative Stage evidence must be established.

---

# Discovery

Stage admission MAY be performed as one controlled operation containing:

1. collection of required Engineering Authority determinations,
2. persistence of those determinations as proposed Stage evidence,
3. construction or preparation of other required proposed Stage artifacts,
4. Procedural Authority verification of the applicable admission requirements,
   and
5. successful commit of Origination or Succession.

Procedural Authority MAY provide the mechanism through which Engineering
Authority supplies and records the engineering determinations required for
Stage admission.

Providing that mechanism SHALL NOT transfer Engineering Authority to
Procedural Authority.

Required substantive engineering determinations SHALL originate from
Engineering Authority.

Procedural Authority MAY verify their presence, attribution, structural
completeness, and procedural consistency.

Procedural Authority SHALL NOT determine their technical correctness or
substitute its own engineering judgment.

Before successful admission, the collected artifacts constitute proposed Stage
evidence and possess no Stage lifecycle authority.

Proposed Stage artifacts acquire Stage authority only upon successful
completion of authorized Origination or Succession.

Successful admission establishes the admitted evidence as authoritative Stage
evidence and establishes the Stage as `ACTIVE`.

---

# Controlled Admission Operation

A controlled Stage-admission operation MAY perform the activities necessary to
prepare, verify, and admit a proposed Stage within one governed operation.

Conceptually:

    begin controlled admission
              |
              v
    collect Engineering Authority
          determinations
              |
              v
       persist proposed
           evidence
              |
              v
       construct required
       proposed artifacts
              |
              v
      Procedural Authority
          verification
              |
          +---+---+
          |       |
        FAIL     PASS
          |       |
          v       v
       no Stage  commit
                  |
          +-------+-------+
          |               |
      Origination      Succession
          |               |
          +-------+-------+
                  |
                  v
                ACTIVE

The activities preceding successful commit SHALL NOT themselves constitute
Stage admission.

The controlled operation SHALL give lifecycle effect to Origination or
Succession only after the applicable Engineering Authority and Procedural
Authority requirements have been satisfied.

A failed admission operation SHALL NOT result in a lifecycle-recognized Stage.

---

# Engineering Authority Collection

Procedural Authority MAY solicit Engineering Authority determinations required
for Stage admission.

The mechanism MAY:

- present questions,
- present required evidence categories,
- provide structurally neutral prompts,
- provide fields in which determinations may be entered, and
- persist the determinations supplied by Engineering Authority.

For example, a mechanism MAY request Engineering Authority to supply:

- Engineering Responsibility,
- bounded Scope,
- Discharge Criteria,
- lineage applicability or lineage continuation determinations,
- identification of engineering state material to a successor baseline, and
- known material baseline divergences where applicable.

The exact required determinations depend upon whether the applicable admission
form is Origination or Succession.

The fact that Procedural Authority requests, receives, or records a
determination SHALL NOT make Procedural Authority the author of that
determination.

Authorship and authority remain with the Engineering Authority that supplied
the substantive engineering content.

---

# Structural Prompting

Procedural Authority or automation MAY provide structural prompts describing
the kind of Engineering Authority determination required.

A structural prompt MAY identify:

- the required evidence category,
- the form in which an answer is expected,
- required subdivisions of a determination, or
- procedural information necessary to record the determination.

Structural prompting SHALL NOT predetermine the substantive engineering
answer.

For example, a mechanism MAY ask Engineering Authority to describe the bounded
Scope of a proposed Stage.

The mechanism SHALL NOT independently determine what that Scope should be.

Therefore:

> Structural prompting is not Engineering Authority.

and:

> Substantive engineering determination remains the responsibility of
> Engineering Authority.

---

# Substantive Engineering Content

Required Engineering Authority determinations SHALL originate from Engineering
Authority.

Procedural Authority and automation SHALL NOT manufacture substantive
engineering determinations in order to satisfy an admission requirement.

Procedural Authority SHALL NOT substitute generated engineering content for a
missing Engineering Authority determination.

The presence of generated placeholder text SHALL NOT constitute evidence that
Engineering Authority has made the required determination.

Automation MAY construct the structure in which a determination will be
recorded.

Automation SHALL NOT treat its own substantive engineering content as the
Engineering Authority determination required for admission.

---

# Procedural Verification

After the required proposed evidence has been collected or constructed,
Procedural Authority SHALL perform the verification required by the applicable
admission form.

Procedural Authority MAY verify matters including:

- required evidence exists,
- required evidence is attributable to the proper authority,
- required determinations have been supplied,
- unresolved required placeholders are absent,
- required Stage and predecessor identities are present,
- predecessor state satisfies applicable procedural requirements,
- required baseline records and provenance are present where applicable, and
- the proposed admission evidence is procedurally consistent.

Procedural Authority SHALL NOT determine:

- whether an Engineering Responsibility is technically correct,
- whether a Scope is technically sufficient,
- whether Discharge Criteria are technically adequate,
- whether an engineering lineage determination is technically correct,
- which engineering state is technically material, or
- whether two different engineering determinations are technically
  equivalent.

Those remain Engineering Authority judgments.

Procedural Authority verifies procedural admissibility.

It does not certify technical correctness.

---

# Procedural Sufficiency

Procedural sufficiency SHALL be determined using requirements that do not
require Procedural Authority to assume Engineering Authority.

Procedural Authority MAY reject a proposed admission where:

- required evidence is absent,
- required evidence remains in a generated placeholder condition,
- required attribution is absent,
- a required declaration has not been made,
- a required predecessor does not exist,
- a required predecessor is not `FROZEN`,
- required baseline provenance is absent, or
- required evidence is procedurally contradictory.

Procedural Authority SHALL NOT reject or approve an engineering determination
merely because it considers the underlying engineering judgment technically
wise, unwise, sufficient, or insufficient.

If Engineering Authority supplies a substantive determination and properly
assumes responsibility for that determination, technical adequacy remains an
Engineering Authority responsibility.

---

# Admission Form

Controlled Stage admission does not create a new form of Stage creation.

The applicable lifecycle-recognition event remains:

- Origination, or
- Succession.

Origination applies where the requirements for legitimate Origination have
been satisfied.

Succession applies where the requirements for legitimate Succession have been
satisfied.

Procedural observations alone SHALL NOT establish which engineering lineage
relationship exists.

Engineering Authority SHALL make the lineage determination required by the
applicable admission form.

Procedural Authority MAY verify that the declared engineering relationship is
procedurally consistent with observable Stage history.

For example:

- a claimed Succession SHALL identify a predecessor that exists and is
  `FROZEN`; and
- a declared engineering relationship SHALL NOT be represented procedurally
  in a manner that contradicts the admission form being performed.

Procedural consistency verification SHALL NOT transfer authority over
engineering lineage determination to Procedural Authority.

---

# Proposed Stage Evidence

Artifacts MAY physically exist before Stage admission.

They MAY contain:

- completed Engineering Authority determinations,
- proposed Stage identity,
- proposed responsibility records,
- proposed Scope,
- proposed Discharge Criteria,
- proposed lineage evidence,
- proposed predecessor references,
- proposed baseline records, and
- other evidence required for admission.

Physical existence SHALL NOT confer Stage authority.

Completion of required artifacts SHALL NOT confer Stage authority.

Engineering Authority approval of its determinations SHALL NOT independently
confer Stage authority.

Beginning Procedural Authority verification SHALL NOT confer Stage authority.

Successful procedural verification SHALL establish admissibility but SHALL NOT
by itself constitute Stage admission.

Before successful admission, such artifacts remain proposed Stage evidence
outside the Stage lifecycle.

---

# Admission Commit

Stage authority is acquired only when authorized Origination or Succession
successfully takes effect.

The point at which the applicable admission event successfully takes effect is
the admission commit.

"Commit" describes the point at which authorized Origination or Succession
takes lifecycle effect.

It SHALL NOT be interpreted as a third Stage-admission form or an additional
lifecycle transition.

Before commit:

- proposed artifacts MAY exist,
- Engineering Authority determinations MAY be complete,
- Procedural Authority verification MAY have succeeded, and
- the proposal possesses no Stage lifecycle state.

Upon successful commit:

- Origination or Succession has occurred,
- the proposed Stage becomes a lifecycle-recognized Stage,
- its initial lifecycle state is `ACTIVE`, and
- the admitted evidence becomes authoritative Stage evidence.

Therefore:

> Procedural verification establishes admissibility.

and:

> Successful Stage admission establishes authority.

---

# Artifact Authority

Stage authority is not an intrinsic property of artifact content.

An artifact does not become authoritative Stage evidence merely because:

- it exists in a Stage-shaped directory,
- it has the expected filename,
- it contains apparently complete engineering content,
- it contains an `ACTIVE` status representation, or
- it has passed an isolated procedural inspection.

Before admission, such an artifact may be proposed evidence.

After successful authorized admission, the admitted artifact may become
authoritative Stage evidence.

The content of an artifact MAY be identical immediately before and immediately
after admission.

Its authority differs because successful admission establishes its governed
relationship to the Stage lifecycle.

Therefore:

> Procedural verification establishes the admissibility of proposed evidence;
> successful admission establishes its Stage authority.

---

# Lifecycle Status Representation

A representation of lifecycle status does not independently confer lifecycle
authority.

Writing, copying, or otherwise producing a value such as:

    ACTIVE

SHALL NOT by itself create an `ACTIVE` Stage.

Rather, successful authorized Origination or Succession establishes the
Stage's `ACTIVE` lifecycle status.

Lifecycle metadata records or represents that authoritative lifecycle fact.

Therefore:

> Lifecycle authority determines valid status representation.

The reverse SHALL NOT be assumed.

---

# Admission Failure

An admission operation that does not complete successfully SHALL NOT result in
a lifecycle-recognized Stage.

Failure MAY occur during:

- evidence collection,
- artifact preparation,
- Engineering Authority input,
- procedural verification, or
- execution of the admission commit.

The handling of proposed artifacts following failure is not established by
this discovery.

A failed proposal MAY potentially be:

- retained for correction,
- retained as non-Stage evidence,
- discarded, or
- otherwise handled as permitted by later specification.

Regardless of implementation:

> Failed admission SHALL NOT create a Stage.

A failed or incomplete proposal SHALL NOT be represented as `ACTIVE`.

---

# Admission Completion

Successful Stage admission SHALL produce an unambiguous lifecycle result.

The externally authoritative result of the admission operation SHALL be either:

- no lifecycle-recognized Stage was created; or
- authorized Origination or Succession completed and the Stage exists as
  `ACTIVE`.

The Stage Method SHALL NOT recognize a partially admitted Stage.

The implementation mechanism used to guarantee this result is not established
by this discovery.

---

# Verification and Commit

Procedural verification and Stage admission are conceptually distinct.

Verification determines procedural admissibility.

Origination or Succession gives lifecycle effect to the authorized admission.

However, they MAY occur within one controlled Stage-admission operation.

The Stage Method does not require an independently exposed waiting period
between successful procedural verification and admission commit.

A controlled admission mechanism MAY proceed directly from successful
verification to commit.

The evidence committed by Origination or Succession SHALL be the evidence
upon which the successful procedural verification was based.

The controlled admission operation SHALL NOT substitute altered or different
required admission evidence between successful procedural verification and
the admission commit.

Therefore:

> Verification is not admission.

and:

> Verification and admission may nevertheless form consecutive parts of one
> controlled operation.

This distinction preserves the authority boundary without requiring a mutable
post-verification proposal state.

---

# Dual Authority

Controlled Stage admission preserves Dual Authority.

Engineering Authority:

- supplies substantive Engineering Responsibility,
- determines bounded Scope,
- establishes Discharge Criteria,
- makes required engineering lineage determinations,
- determines engineering materiality where required, and
- assumes responsibility for those engineering determinations.

Procedural Authority:

- provides or governs the mechanism through which required evidence may be
  collected,
- records or preserves Engineering Authority determinations without assuming
  their authorship,
- verifies required attribution,
- verifies procedural completeness,
- verifies procedural consistency,
- verifies applicable lifecycle prerequisites, and
- permits the admission mechanism to proceed only when the applicable
  procedural requirements have been satisfied.

Neither authority independently creates legitimate Stage authority.

The authorized admission boundary gives lifecycle effect to the determinations
and verification required from both authorities.

---

# Automation Boundary

Automation MAY:

- initiate a controlled Stage-admission workflow,
- inspect procedural Stage context,
- present structurally neutral prompts,
- collect Engineering Authority input,
- persist Engineering Authority determinations,
- construct proposed Stage artifacts,
- construct temporary or provisional workspaces,
- verify procedural prerequisites,
- verify required evidence presence and attribution,
- verify unresolved placeholders are absent,
- verify procedural consistency,
- reject procedurally inadmissible proposals, and
- execute the authorized admission commit as permitted by the governing Stage
  Method specification.

Automation SHALL NOT:

- originate substantive Engineering Authority determinations,
- determine technical correctness,
- determine engineering Scope,
- establish engineering Discharge Criteria,
- independently determine engineering lineage,
- independently determine engineering materiality,
- manufacture evidence that Engineering Authority made a determination,
- treat proposal construction as Stage creation,
- treat procedural verification alone as Stage admission, or
- represent a failed admission as an `ACTIVE` Stage.

The mechanism executing an authorized admission commit gives effect to the
governed authority established by the Stage Method.

The mechanism SHALL NOT be treated as an independent source of Engineering
Authority.

---

# Implementation Independence

This discovery does not require Stage admission to be performed by a shell
script.

A controlled admission mechanism MAY be implemented through:

- an interactive command,
- a shell script,
- a graphical interface,
- another controlled software mechanism, or
- a future mechanism consistent with Stage Method governance.

Interactive prompting is one permissible implementation of Engineering
Authority evidence collection.

It is not itself a constitutional requirement.

Likewise, this discovery does not prescribe:

- temporary-directory design,
- filesystem transaction mechanisms,
- atomic rename operations,
- rollback procedures,
- persistence mechanisms,
- locking,
- hashes,
- manifests, or
- recovery procedures.

Those remain matters for specification and implementation.

---

# Implications

Engineering Authority evidence may be constructed before a Stage exists.

Procedural Authority may provide the mechanism through which that evidence is
collected and persisted without becoming its engineering author.

A proposed Stage may be structurally complete before it possesses lifecycle
authority.

Procedural verification establishes whether the proposal is admissible.

Verification does not itself create the Stage.

Successful Origination or Succession establishes the Stage's lifecycle
authority.

The admitted Stage begins as `ACTIVE`.

A controlled Stage-admission operation may therefore perform:

    collect -> persist -> verify -> commit

without creating an intermediate Stage lifecycle state.

This permits a single controlled admission mechanism to preserve both Dual
Authority and Lifecycle Determinism.

---

# Bedrock

> **Engineering evidence may be constructed before Stage authority exists;
> Stage authority arises only when the verified proposal successfully crosses
> the authorized admission boundary.**
>
> **The mechanism that collects an Engineering Authority determination does
> not thereby become the source of that determination.**
>
> **Procedural verification establishes admissibility; successful Origination
> or Succession establishes Stage authority.**

---

# Depends On

- FD-0005 — Dual Authority
- FD-0006 — Lifecycle Determinism
- FD-0009 — Lifecycle Transition Governance
- FD-0010 — Stage Origination
- FD-0011 — Stage Origination Authority
- FD-0012 — Stage Succession Authority

---

# Open Questions

This discovery does not define:

- the exact command or mechanism implementing controlled Stage admission,
- the exact prompts used to collect Engineering Authority determinations,
- the persistence format used for proposed Stage evidence,
- whether proposed evidence is constructed in a temporary directory or another
  provisional workspace,
- how failed proposals are retained, corrected, or discarded,
- the exact mechanism used to commit Origination or Succession,
- the mechanism used to guarantee that partially completed admission cannot be
  represented as an `ACTIVE` Stage,
- rollback or recovery behavior following implementation failure,
- locking or concurrency requirements,
- the exact machine-readable representation of Engineering Authority
  attribution,
- whether one implementation mechanism SHALL perform both Origination and
  Succession,
- the detailed changes required to existing Stage Method tooling, or
- the broader governance status of engineering activity performed outside a
  controlled admission operation before Stage admission.

These remain matters for subsequent specification or investigation.

---

## History

| Version | Status | Description |
|---|---|---|
| 0.1.0 | Draft | Controlled Stage Admission |
| 1.0.0 | Accepted | Controlled Stage Admission |


