# FD-0010 — Stage Origination

**Status:** Accepted
**Version:** 1.0.0

---

# Context

During inspection of the Stage lifecycle, the requirement that a new Stage
be created only from a `FROZEN` predecessor exposed an unresolved condition.

The requirement is valid for a successor Stage because succession occurs
within an existing Stage lineage.

An originating Stage, however, has no predecessor.

Requiring an originating Stage to possess a `FROZEN` predecessor produces an
infinite dependency: every predecessor would itself require an earlier
predecessor, and no Stage lineage could ever legitimately begin.

The investigation therefore examined whether all Stage creation is the same
kind of lifecycle operation.

---

# Discovery

Stage creation has two distinct forms:

1. **Origination**
2. **Succession**

Origination establishes the first Stage of a Stage lineage.

Because no Stage lineage exists before origination, an originating Stage does
not require a predecessor Stage.

Succession continues an existing Stage lineage.

A successor Stage therefore remains subject to the lifecycle requirements
governing succession, including the requirement for a legitimate `FROZEN`
predecessor.

Origination is not an exception to succession.

Origination and succession are distinct forms of Stage creation.

---

# Rationale

A predecessor requirement can govern succession only after a Stage lineage
already exists.

Applying that requirement to origination makes Stage creation impossible,
because the first Stage would require a predecessor whose own creation would
require another predecessor without termination.

The absence of a predecessor during origination therefore does not constitute
a waiver of the succession rules.

There is no predecessor because no succession is occurring.

Once a Stage lineage has been originated, subsequent Stage creation within
that lineage is governed by succession and its associated lifecycle
requirements.

Origination SHALL NOT be used to bypass an existing applicable Stage lineage
or an undischarged Stage responsibility.

---

# Implications

This discovery establishes that lifecycle rules governing Stage creation must
distinguish origination from succession.

Therefore:

- an originating Stage SHALL NOT require a predecessor merely in order for a
  Stage lineage to begin,
- a successor Stage SHALL remain subject to the predecessor requirements of
  lifecycle succession,
- the absence of a predecessor SHALL NOT be treated as a general exception to
  lifecycle governance,
- origination SHALL NOT provide a mechanism for escaping an unresolved Stage
  responsibility, and
- Stage lifecycle specifications and automation SHOULD distinguish Stage
  origination from Stage succession where Stage creation is governed.

This discovery does not define the complete procedural requirements for
legitimate Stage origination.

Those requirements remain subject to further specification and inspection.

---

# Bedrock

**A Stage lineage must be originated before it can be succeeded.**

**Origination requires no predecessor; succession requires a legitimate
predecessor.**

---

# Dependencies

- FD-0003 — Dependency Tracing
- FD-0006 — Lifecycle Determinism
- FD-0009 — Lifecycle Transition Governance

---


## History


| Version | Status | Description |
|---|---|---|
| 0.1.0 | Draft | Stage Origination |
| 1.0.0 | Accepted | Passed Anvil Inspection |



