# The Forge

The Forge is a disciplined engineering methodology for discovering and
validating engineering knowledge through inspection.

## Purpose of This Repository

The Forge preserves the questions, investigations, findings, dependencies,
inspections, and governing records through which engineering knowledge is
examined and developed.

Repository placement does not itself create engineering truth, Procedural
Authority, canonical standing, or acceptance. Each artifact derives its
meaning and standing from the applicable Forge governance and lifecycle.

## Discovery Record Structure

Forge Discovery records use the canonical Discovery template in
`templates/discovery.md`.

The Discovery template distinguishes between core and conditional sections.

### Core Sections

Core sections are retained in each Discovery record. If a core section has no
substantive content applicable to a particular finding, the section remains
and states that condition explicitly. Content is not manufactured merely to
populate a required section.

### Conditional Sections

Conditional sections are included only when the condition requiring them
exists. Their use in one Discovery does not make them mandatory in another.

A conditional section may be added in a later version when its triggering
condition subsequently arises. Adding a conditional section must preserve the
historical content and chronology of earlier versions.

Standardized conditional sections and their placement are defined by the
applicable Discovery template when such guidance has been adopted.

## Discovery Dependencies

Forge Discovery records distinguish among established dependency basis,
unresolved dependencies, and later dependency resolution.

### `Depends On`

`Depends On` records the established dependency basis upon which the present
finding relies.

A dependency is not established merely because another artifact is nearby,
numbered earlier, similarly named, or concerned with related subject matter.

### `Open Dependencies`

`Open Dependencies` records unresolved questions or relationships exposed or
preserved by the finding when they are recorded.

An Open Dependency does not answer its own question and does not become an
established premise merely because it is named in a Discovery.

Open Dependencies should identify unresolved relationships that materially
follow from the investigation. Interesting but non-blocking questions are not
made dependencies merely because they can be asked.

### Dependency Resolution Record

A Dependency Resolution Record is a conditional Discovery section used when an
Open Dependency preserved by an earlier version has subsequently been resolved
or materially advanced.

The historical `Open Dependencies` section is not silently rewritten, removed,
or made to appear as though the later resolution had always been known.
Instead, the later state is recorded separately.

A Dependency Resolution Record should identify, where applicable:

1. the historical dependency being addressed;
2. the later basis that resolved or materially advanced it;
3. the resulting resolution;
4. the boundaries of what that resolution establishes;
5. any new dependency exposed by the resolution; and
6. the relevant lifecycle or inspection state where material.

A Dependency Resolution Record reports a later change in the state of
knowledge. It does not retroactively alter the investigation, finding,
authority state, evidence state, or lifecycle state recorded by an earlier
version.

## Historical Preservation

Forge records preserve the state of knowledge and governance that existed when
they were created or revised.

Later knowledge may clarify, resolve, supersede, or constrain an earlier open
question without erasing the fact that the question was unresolved at the
earlier point in the record.

Accordingly:

- historical investigation text is not silently rewritten for present-day
  narrative cleanliness;
- an earlier Open Dependency remains part of the historical record even after
  it is later resolved;
- later resolution is recorded through an appropriate later-version section
  or artifact relationship;
- later authority does not silently create earlier authority;
- later evidence does not silently become historical evidence; and
- later lifecycle state does not rewrite the state under which an earlier
  event occurred.

The Forge may accumulate knowledge without manufacturing a history in which it
always possessed that knowledge.

## Dependency Direction

Dependency relationships have direction.

```text
Established basis
        ↓
Present finding
        ↓
Open dependency
        ↓
Later investigation
        ↓
Later resolution record, when earned
```

`Depends On` points backward to an established basis.

`Open Dependencies` points forward to unresolved work exposed or preserved by
the present finding.

A later Dependency Resolution Record connects the preserved historical
question to the later basis that changed its state.

None of these relationships is inferred merely from chronology, numbering,
repository location, or subject similarity.

## Forge and Anvil

The Forge investigates unresolved questions and dependencies and produces
bounded findings.

The Anvil inspects claims, findings, or complete artifacts by attacking their
assumptions, boundaries, derivations, contradictions, and unsupported
extensions.

Anvil survival establishes inspection evidence. It does not, by itself, create
Procedural Authority, authorize a procedure, or perform a lifecycle transition
unless applicable governance separately establishes that result.

Questions enter the Forge. Findings and complete artifacts go to the Anvil.

## Authority Boundary

This README explains repository practice and the relationships among Forge
records. It does not independently create authority for a Discovery, template,
procedure, lifecycle transition, or governance relationship.

Where this README conflicts with applicable constitutional authority,
standards, specifications, or other governing artifacts, the applicable higher
authority prevails.
