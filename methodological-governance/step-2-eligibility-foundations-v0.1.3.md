# Forge Investigation — Step 2: Eligibility Foundations

**Status:** OPEN — investigative workpiece; no procedural act
**Version:** 0.1.3
**Date:** 2026-09-17
**Predecessor:** `step-2-eligibility-foundations-v0.1.2.md` (preserved)
**Anvil input:** A-01 retained; A-02 bounded wording repaired, completeness
open; A-03 retained; A-04 new finding that archived Git history was available
but unexamined.
**Evidence boundary:** Git repository embedded in `forge(20260917-122512).zip`,
plus the predecessor's named Stage archive. Git commit dates and messages are
historical repository records, not independently validated procedural
authorization or proof of present governing force.

## Investigation question

What can the embedded Git objects actually establish about the Knowledge
Lifecycle transition and FD-0009 artifact identity, and which authority,
terminology, and eligibility questions remain unproven?

## A-04 — Embedded Git evidence recovered

The ZIP contains `forge/.git` with commit history. Earlier v0.1.2's statement
that no Git history was provided was incorrect. Inspected with `git log --all`,
`git show`, and `git diff` in an extracted copy. The extracted working tree
includes uncommitted changes; commit objects are distinguished from the ZIP's
working-tree bytes. No remote, external record, or current live checkout has
been verified.

### A-01 — Knowledge Lifecycle transition

**Record 1**

**Evidence:**

Commit `5cc8b159d3fd09a08682e4adfdc1c932ed5b9f1b`, authored/committed
2026-08-08 21:19:40 -0400, message `finally Approved by the forge and the
anvil`

**Demonstrates:**

Its actual diff changes `specifications/KNOWLEDGE-LIFECYCLE.md` header from
`Draft — Forge Procedural-Authority Review Complete; Anvil Final Inspection
Pending`, v0.9.0, to `Approved`, v1.0.0. The repository therefore records an
actual header transition, not merely FI-0003's retrospective description.

**Does not demonstrate:**

The message does not independently demonstrate Anvil silence, the authorized
actor's authority, an external approval instrument, or a valid procedural act.

**Record 2**

**Evidence:**

Commit `3777e8e4644c6a4b6a52a655250461ebeab8dcc9`, 2026-08-09 21:24:23 -0400

**Demonstrates:**

Adds a `History` entry `1.0.0 | Accepted | KNOWLEDGE-LIFECYCLE.md` to a
document whose header was `Approved`.

**Does not demonstrate:**

Does not explain or authorize the differing status labels.

**Record 3**

**Evidence:**

ZIP working tree relative to repository HEAD

**Demonstrates:**

Changes lifecycle header `Approved` → `Accepted`, adds a `Status` table
`Accepted` v1.0.0 and renames `History` to `Version History`.

**Does not demonstrate:**

Uncommitted changes do not provide a commit timestamp, authorization, or
historical transition record. They cannot be projected backward onto August 8.

**Record 4**

**Evidence:**

Approval Gate in historical `5cc8b15` version

**Demonstrates:**

Requires Anvil absence of unresolved tension *and* an authorized procedural act
recording approval/version transition.

**Does not demonstrate:**

Its requirement is not evidence that the requirement was met.

**Finding:** A-04's missing-primary-source problem is repaired by direct Git
inspection. A-01 remains OPEN on authority and governing applicability.
`Approved` and `Accepted` are **distinct recorded labels**, with an August 9
history entry and later uncommitted working-tree changes explaining how both
appear; their legal/procedural equivalence is not established. FI-0003's
retrospective statement is now corroborated as to the repository header
transition only.

### A-03 — FD-0009 identity

**Record 1**

**Evidence:**

Commit `6432010b68b3eef066f02ec7da127d10ee109551`, 2026-08-11 21:33:51 -0400,
message `Backing up and updating FD-0009`

**Demonstrates:**

Adds `discoveries/FD-0009-Lifecycle-Transition-Governance.md` under that path
with header `Accepted`, version `0.1.0`; its history lists `0.1.0 Draft` and
`1.0.0 Accepted`.

**Does not demonstrate:**

No separate acceptance act or explanation of header/history mismatch is
established by the commit.

**Record 2**

**Evidence:**

Commit `247ed629f61a9aa4f89fb336c5f7c9d4514c6e7e`, 2026-08-18 09:01:33 -0400

**Demonstrates:**

Changes the `1.0.0 Accepted` history description from `Lifecycle Transition
Governance` to `Passed Anvil Inspection`; does not change the header version.

**Does not demonstrate:**

A history description asserting Anvil inspection is not the inspection record,
and does not prove a valid acceptance or identify the accepted bytes.

**Record 3**

**Evidence:**

Discovery index

**Demonstrates:**

Lists FD-0009 Accepted without accepted version or original act.

**Does not demonstrate:**

Cannot settle which version was accepted.

**Finding:** The metadata discrepancy is traceable to the earliest inspected
commit of the current filename and persists through August 18. A-03 remains
OPEN: exact accepted artifact/version and legitimacy of acceptance are
unverified. Do not change metadata or choose 0.1.0 versus 1.0.0 by inference.
Earlier history under another filename, if material, requires separate
identity/provenance proof.

## A-02 — Eligibility governance remains bounded

The primary Git evidence addresses repository history, **not**
Discovery-specific eligibility predicates, thresholds, an operative Eligibility
Case, or CDA authorization. Earlier E01–E08 trace remains provisional. No claim
of global absence is made. Current governing indexes, adopted predicate
instruments, and any supersession records still require verification. Recorded
`Accepted` and `Approved` labels alone do not confer demonstrated governing
standing.

## Next evidence actions

1. Locate the contemporaneous Anvil final inspection and authorized procedural
   approval instrument for the Knowledge Lifecycle, with actor, scope, status
   semantics and provenance; check whether any subsequent authorized act maps
   `Approved` to `Accepted`.
2. Trace FD-0009's predecessor identity, inspection, actual acceptance event,
   and exact accepted bytes; distinguish a historical description from a
   procedural act.
3. Verify current live authoritative index and supersession chain; locate any
   adopted Discovery-specific predicates and Eligibility Case mechanism, or
   keep these gaps explicitly open.
4. Update the CDA requirement-to-source trace only with sources whose identity,
   applicability, and governing standing have been independently established;
   separately establish Stage review and CDA authorization.

## Forge disposition

**Step 2 OPEN. A-04 repaired by examining the actual embedded Git history. A-01
and A-03 remain OPEN on authority and identity; A-02 wording remains repaired,
source completeness OPEN.** This workpiece does not perform approval, Anvil
inspection, Stage review, CDA authorization, canonical inclusion, or historical
revision. Submit this version for Anvil inspection after verifying its factual
trace.
