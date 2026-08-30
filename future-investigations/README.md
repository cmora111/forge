# Forge Future Investigations

## Purpose

Future Investigations preserve legitimate engineering questions exposed during
Forge investigation whose resolution has not been demonstrated to be necessary
to the engineering dependency currently being investigated.

The purpose of this mechanism is to preserve those questions and any useful
investigative work already performed without allowing a non-blocking dependency
to divert the Forge from the engineering problem that invoked it.

A Future Investigation is therefore a deliberate deferral mechanism.

It preserves the question.

It does not require the question to be answered now.

---

## Governing Distinction

The Future Investigations mechanism preserves the distinction:

    Interesting Dependency ≠ Blocking Dependency

and:

    Unresolved Question ≠ Required Present Investigation

The existence of a legitimate unresolved question does not, by itself, require
the Forge to pursue that question.

---

## Future Investigation

A Future Investigation records an unresolved engineering question that:

1. was legitimately exposed by Forge or related engineering work;
2. may warrant future investigation;
3. is not presently demonstrated to block the engineering dependency under
   investigation; and
4. should be preserved so that the work already performed is not lost.

A Future Investigation may preserve:

- the question that was exposed;
- the engineering context in which it arose;
- partial findings;
- distinctions and invariants;
- relevant evidence;
- related artifacts;
- unresolved subquestions; and
- the condition under which investigation should resume.

---

## Authority Boundary

A Future Investigation is an investigative record.

It is not a Forge Discovery and does not acquire Discovery standing merely
because it is recorded.

Therefore:

    Future Investigation ≠ Forge Discovery

    Future Investigation ≠ Accepted Finding

    Future Investigation ≠ Engineering Requirement

    Future Investigation ≠ Blocking Dependency

    Deferred ≠ Rejected

Findings preserved within a Future Investigation retain only the standing they
possessed when they were deferred.

Recording them in an FI does not increase their epistemic, procedural,
normative, or canonical authority.

---

## Deferral Rule

When dependency tracing exposes a legitimate question, the Forge should
determine whether resolution of that question is necessary to resolve the
engineering dependency that invoked the current investigation.

If resolution is presently necessary, the question remains active Forge work.

If resolution is not presently necessary, the question may be preserved as a
Future Investigation and the Forge returns to the blocking dependency.

Conceptually:

    Question Exposed
          │
          ▼
    Does It Block the
    Current Engineering
    Dependency?
       │         │
      YES        NO
       │         │
       ▼         ▼
    Continue    Preserve as FI
     Forge          │
                    ▼
                  Return

---

## Re-entry Rule

A Future Investigation SHOULD be reopened only when subsequent engineering
demonstrates that resolution of the preserved question has become materially
necessary.

The mere existence of the unresolved question is not sufficient reason to
reopen it.

Therefore:

    Curiosity ≠ Re-entry Condition

and:

    Unanswered ≠ Blocking

When an FI is reopened, the engineering condition requiring its resolution
SHOULD be recorded in the FI.

---

## Records

Future Investigation records are stored in:

`forge/future-investigations/`

Each investigation receives an identifier of the form:

`FI-NNNN`

Individual records SHOULD be created using:

`forge/templates/FI-TEMPLATE.md`

The Future Investigation index is maintained in:

`forge/future-investigations/INDEX.md`

---

## Scope

This mechanism governs preservation and re-entry of deferred Forge
investigations.

It does not establish:

- the Forge Discovery lifecycle;
- Canonical Discovery Acceptance;
- epistemic eligibility;
- Stage engineering requirements;
- authority for any Discovery finding;
- authority for any Stage specification;
- or a requirement that every unanswered engineering question become an FI.

Questions that are trivial, speculative, duplicative, or unrelated to the
engineering work need not be preserved merely because they were asked.

---

## Version History

### 0.1.0 — 2026-08-30

Initial definition of the Forge Future Investigations mechanism.

Established the distinction between unresolved questions and presently blocking
dependencies, the authority boundary of FI records, the deferral rule, and the
re-entry rule.

---
