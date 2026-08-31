<!--
Forge Discovery Record Template

Discovery Template Version: 2.0.0

This is the current canonical template for new Forge Discovery records.

It supersedes discovery-v1.md for creation of new discoveries.
discovery-v1.md is retained as the historical first-generation template.

This template defines the structure of a Forge Discovery record. It does not
prescribe the result or internal analytical structure of a Forge investigation.

CORE SECTIONS

The standard discovery-record structure is:

    Forge Question
    Context
    Forge Investigation
    Forge Finding
    Invariants
    Does Not Establish
    Open Dependencies
    Depends On
    Status
    Version History

Core sections should be retained in new discovery records.

If a core section has no substantive content for a particular discovery, state
that condition explicitly rather than silently omitting the section or
manufacturing content merely to populate it.

CONDITIONAL SECTIONS

Additional analytical sections may be introduced when required by the
discovery.

Examples include:

    Consequences
    <Discovery-Specific> Structure
    <Discovery-Specific> Condition

Conditional sections must serve the discovery being recorded. Their existence
in one discovery does not make them mandatory in later discoveries.

Forge Investigation is the standard container for the reasoning that produced
the finding.

Numbered strikes are preferred when the Forge investigates by attacking
assumptions, counterexamples, boundaries, or failure conditions.

The number and form of strikes are determined by the investigation.

The template must not force the Forge to manufacture attacks or analytical
structures merely to satisfy the record format.

DEPENDENCY DIRECTION

Depends On records the established dependency basis upon which the present
finding relies.

Open Dependencies records unresolved questions exposed or preserved by the
present finding.

Neither relationship should be inferred merely from proximity, numbering, or
subject similarity.

HISTORICAL RECORDS

Discovery records created before Discovery Template Version 2.0.0 remain
historical records of the Forge as it developed.

Adoption of this template does not by itself require earlier discoveries to be
rewritten into the present structure.

Historical structural variation must not be silently erased merely to create
retrospective formatting uniformity.
-->

# FD-XXXX — <Discovery Title>

**Status:** Hold
**Version:** 0.1.0

---

# Forge Question

<!--
State the focused engineering question investigated by this discovery.

The question should identify the unresolved dependency or engineering tension
that caused the investigation without assuming its answer.
-->

<Forge Question>

---

# Context

<!--
Describe the engineering context in which this investigation became necessary.

Identify prior discoveries, observations, specifications, engineering events,
or unresolved dependencies required to understand why the question entered the
Forge.

Do not expand into dependencies that are merely interesting but do not bear
upon the present investigation.
-->

<Context>

---

# Forge Investigation

<!--
Record the reasoning through which the Forge attacked the question.

When the investigation proceeds through explicit strikes, use H2 headings:

    ## Strike 1 — <Attack>
    ## Strike 2 — <Attack>

Each strike should test a distinct assumption, counterexample, boundary, or
failure condition.

The investigation need not contain a predetermined number of strikes.
-->

## Strike 1 — <Attack>

<Investigation>

---

<!--
DISCOVERY-SPECIFIC ANALYTICAL EXTENSION POINT

When necessary, insert discovery-specific analytical sections HERE, after the
Forge Investigation and before the Forge Finding.

Examples:

    # <Discovery-Specific> Structure

    # <Discovery-Specific> Condition

These sections may express structures, conditions, models, distinctions, or
other analytical results developed during the investigation.

Their names and internal structures should describe the actual discovery rather
than imitate sections used by an earlier FD.

Delete this comment when instantiating the discovery if no such sections are
required.
-->

# Forge Finding

<!--
State the bounded engineering finding produced by the investigation.

The finding should state what the Forge has established without silently
expanding into unresolved dependencies.

A block quote may be used to distinguish the formal finding from the
investigation that produced it.
-->

> **<Forge Finding>**

---

# Invariants

<!--
Record distinctions or relationships that must remain true if the finding is
preserved.

Concise expressions may be used:

    Concept A
        ≠
    Concept B

Do not manufacture invariants merely to populate this section.

If the discovery establishes no meaningful invariant beyond the Forge Finding,
state that explicitly.
-->

```text
<Invariant A>
    ≠
<Invariant B>
```

---

# Does Not Establish

<!--
State the boundaries of the discovery.

Identify questions, authorities, mechanisms, implementations, representations,
or downstream dependencies that the finding does not establish.

This section prevents the authority or meaning of the discovery from expanding
beyond what the Forge actually established.
-->

This discovery does not establish:

- <Boundary>

---

<!--
OPTIONAL CONSEQUENCES SECTION

Insert the following section HERE when the finding creates consequences that
should be preserved separately from the formal Forge Finding:

# Consequences

<State what follows from the discovery, what prior assumptions can no longer be
made, or what subsequent engineering work is affected.>

---

Do not include Consequences merely to repeat the Forge Finding.

Delete this comment when instantiating the discovery if the section is not
required.
-->

# Open Dependencies

<!--
Record unresolved questions exposed or preserved by this discovery.

Open Dependencies point forward from the present finding.

An Open Dependency is not established merely because the discovery identifies
it.

Do not include a question merely because it is interesting. Include it when it
is a legitimate unresolved dependency exposed by the investigation.

Where a deferred Future Investigation is related but its re-entry condition has
not been satisfied, preserve that boundary explicitly.
-->

1. <Open Dependency>

---

# Depends On

<!--
Record discoveries upon which the present finding directly depends.

Depends On points backward to the dependency basis of the finding.

Distinguish direct dependencies from discoveries that provide only context.

Do not allow the dependency declaration itself to manufacture authority or
standing that has not otherwise been established.
-->

- FD-XXXX — <Discovery Title>

<!--
Where a Future Investigation or another record is related but is not a direct
dependency, identify that distinction explicitly when necessary.
-->

---

# Status

| Field | Value |
|---|---|
| Status | Hold |
| Version | 0.1.0 |

<!--
State what this FD memorializes.

For a newly memorialized finding awaiting Anvil inspection, state that the
finding remains in Hold pending Anvil inspection.

State that unresolved Open Dependencies remain unresolved and are not
established by the finding.

After successful Anvil inspection, update the status and version according to
the applicable discovery-acceptance procedure.

Do not rewrite the historical investigation merely because its authority
condition changes.
-->

FD-XXXX memorializes the Forge finding concerning <subject>.

The finding remains in Hold pending Anvil inspection.

The Open Dependencies remain unresolved and are not established by this
finding.

---

# Version History

| Version | Status | Description |
|---|---|---|
| 0.1.0 | Hold | Initial memorialization of the Forge finding concerning |
| | | <subject>. |


---

