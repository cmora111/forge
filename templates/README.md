# Forge Templates

## Purpose

The `templates` directory contains reusable document structures for Forge
artifacts.

A template defines the expected organization of an artifact without containing
the engineering content of any particular artifact.

This directory has one exclusive responsibility:

> Preserve the canonical structure of Forge artifact types.

---

## Naming Convention

Template filenames describe the artifact type only.

The containing `templates` directory already establishes that each file is a
template. Template filenames therefore SHALL NOT repeat the word `template`.

Examples:

```text
templates/
├── decision.md
├── discovery.md
├── inspection.md
└── README.md
```

Numbered artifact identifiers SHALL NOT be used for templates.

For example:

```text
FD-0001.md
```

identifies a specific Forge Discovery, while:

```text
templates/discovery.md
```

defines the reusable structure from which Forge Discovery artifacts are created.

---

## Current Templates

### `decision.md`

Defines the canonical structure for recording a Forge decision.

### `discovery.md`

Defines the canonical structure for recording a Forge Discovery.

### `inspection.md`

Defines the canonical structure for recording a Forge inspection.

---

## Template Requirements

Each template SHALL:

- serve exactly one artifact class;
- contain structure rather than project-specific engineering content;
- use neutral placeholders where artifact-specific content is required;
- remain consistent with the governing standard or specification for that
artifact class;
- avoid imposing requirements that are not established by an authoritative
source.

A template SHALL NOT:

- become the authority that defines an artifact class;
- contain completed engineering conclusions;
- include a numbered artifact identity;
- duplicate responsibilities already owned by a governing specification,
standard, or constitutional law.

---


## Discovery Template Applicability

The canonical Discovery template distinguishes between core and conditional
sections.

Core sections preserve the standard structure of a Discovery record. When a
core section has no substantive content applicable to a particular Discovery,
the section remains and states that condition explicitly rather than
manufacturing content merely to populate the structure.

Conditional sections are included only when the condition requiring them
exists. Their use in one Discovery does not make them mandatory in another.

A conditional section may be added in a later version when its triggering
condition subsequently arises. Such an addition preserves the historical
content and chronology of earlier versions.

The canonical Discovery template defines standardized conditional sections and
their placement when that guidance has been adopted. A template extension does
not itself establish the substantive condition that would require an artifact
instance to use the extension.

### Dependency Resolution Records

`Dependency Resolution Record` is a conditional Discovery section. It may be
used when an Open Dependency preserved by an earlier version has subsequently
been resolved or materially advanced.

The template provides structure for recording that later state. It does not
itself resolve the dependency, establish the authority or standing of the later
basis, or authorize a lifecycle transition.

The historical Open Dependency remains part of the earlier record. Later
resolution is represented without silently rewriting the earlier state of
knowledge, authority, evidence, or lifecycle.

## Authority

Templates derive their authority from the governing documents that define their
artifact classes.

A template SHALL conform to its governing authority.

If a template conflicts with a governing document, the governing document SHALL
prevail.

---

## Change Discipline

Changes to a template may affect every future artifact created from it.

Template changes SHALL therefore be reviewed for:

- consistency with governing documents;
- backward compatibility where applicable;
- unintended changes to artifact responsibility;
- effects on existing tooling or automation.

Existing artifacts SHALL NOT be rewritten merely because their template changes
unless a separate requirement authorizes that migration.

---

## Relationship to Other Forge Artifacts

| Artifact | Responsibility |
|---|---|
| Constitutional laws | Establish foundational authority |
| Standards and specifications | Define what an artifact must be |
| Templates | Preserve the reusable structure of an artifact type |
| Artifact instances | Contain the actual engineering record |

The dependency order is:

```text
Constitutional Authority
        ↓
Standard or Specification
        ↓
Template
        ↓
Artifact Instance
```

---

