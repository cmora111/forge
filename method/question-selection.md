# Forge Question Selection

**Status:** Draft  
**Version:** 0.1.0

---

# Purpose

This document defines a human-operable procedure for deriving the next
justified engineering question from recognized engineering tension.

The procedure exists so that question selection can be performed, taught,
recorded, and inspected without depending upon intuition, academic rank, or
an artificial-intelligence system.

This document does not determine the answer to a Question. It determines the
uncertainty for which the next Investigation is responsible.

---

# Foundation

This method operationalizes the following accepted Forge Discoveries:

- FD-0001 — Engineering Tension;
- FD-0002 — Investigation Pattern Recognition;
- FD-0003 — Dependency Tracing; and
- FD-0004 — Bedrock Recognition.

It introduces no independent engineering or procedural authority. Where this
method conflicts with an accepted supporting Discovery, the conflict is
engineering tension and SHALL be returned to the Forge.

---

# Scope

This method begins after an observation, proposed explanation, decision,
artifact, model, or engineering consequence reveals uncertainty.

It defines how an engineer:

1. preserves the present state of knowledge;
2. localizes the unresolved relationship;
3. classifies the investigation pattern;
4. identifies candidate uncertainties;
5. selects the next investigative responsibility;
6. formulates a neutral and answerable Question; and
7. records why that Question is justified.

This method ends when one Question has been selected, when bedrock is
recognized, or when the investigation is suspended at an explicit evidentiary
limit.

Investigation, evidence collection, Discovery creation, validation, and
procedural adoption remain separate responsibilities.

---

# Operating Principle

> The next Forge Question is the smallest answerable question whose resolution
> is presently expected to reduce the greatest material engineering
> uncertainty without presuming its answer.

Question selection is therefore constrained by the evidence already
available. The engineer does not begin by asking every possible question or
by choosing a preferred explanation. The engineer locates the uncertainty
that prevents the work from being faithfully explained, justified, or
governed, and gives one Investigation responsibility for resolving it.

"Smallest" refers to investigative responsibility, not sentence length.

"Greatest" refers to the amount of material uncertainty that may be removed,
not to convenience, novelty, or personal interest.

"Presently expected" acknowledges that the Question is selected before its
answer is known. Investigation may show that another dependency is more
fundamental.

---

# Required Inputs

Question selection requires an inspectable record of the current engineering
state. The record SHOULD contain:

- what was observed;
- the relevant conditions under which it was observed;
- the physical, procedural, or informational boundaries at which evidence can
  actually be obtained;
- what has been tested;
- what each test actually demonstrated;
- known contradictions, failures, and limitations;
- proposed explanations, identified as proposals rather than facts;
- unresolved assumptions; and
- the boundary between demonstrated knowledge and unresolved uncertainty.

Missing information does not authorize the engineer to invent it. A missing
input may itself become the subject of the next Question.

---

# Question-Selection Procedure

## 1. Preserve the Observation

Record what happened before explaining why it happened.

Separate the record into three categories:

| Category | Meaning |
|---|---|
| Demonstrated | Supported within the stated conditions by available evidence |
| Reported | Preserved from an identified source but not yet independently demonstrated |
| Assumed | Treated as true for reasoning but not yet demonstrated |

Do not silently promote a Reported or Assumed claim into Demonstrated
knowledge.

The purpose of this step is not to distrust the observer. It is to preserve
which relationships Reality has constrained and which remain open to
investigation.

## 2. State the Engineering Tension

Express the unresolved condition without embedding a cause or remedy.

A useful tension statement identifies:

- the behavior or relationship that cannot yet be explained;
- the scope in which it occurs; and
- the consequence of leaving it unresolved.

For example:

> The right-side pixel props operate during an independent test but do not
> respond in the deployed configuration.

"The jumper is bad" is not a tension statement. It is a proposed explanation.

## 3. Locate the Working–Failing Boundary

Find the narrowest boundary across which demonstrated behavior changes.

Depending upon the discipline, the boundary may be:

- physical;
- temporal;
- procedural;
- logical;
- organizational;
- environmental;
- jurisdictional; or
- informational.

Compare what works with what fails. Preserve both the shared conditions and
the differences. A working condition is evidence and SHALL NOT be discarded
merely because the investigation concerns a failure.

The behavioral boundary and the accessible observation boundary may not be the
same. A system may reveal where behavior changes while preventing direct
measurement at that location.

When the behavioral boundary is inaccessible, identify the nearest accessible
boundaries on each side. Evidence collected at those boundaries may constrain
the unresolved relationship, but SHALL NOT be represented as a direct
observation of the inaccessible boundary.

If the boundary cannot yet be located, the next Question SHOULD seek the
observation needed to locate it.

## 4. Identify the Unresolved Relationship

Describe the relationship at the boundary that the current model cannot yet
justify.

Ask:

- What must cross, govern, precede, support, or explain this boundary?
- What is shared by the failures?
- What differs between the working and failing conditions?
- Which claimed relationship has not actually been demonstrated?
- Which conclusion relies upon an unstated assumption?

The result SHOULD identify an uncertainty, not select a culprit.

## 5. Recognize the Investigation Pattern

Classify the unresolved relationship using the recurring investigation
patterns presently established by FD-0002.

| Pattern | Recognition cue | Typical question form |
|---|---|---|
| Responsibility | Ownership is missing, shared, or unclear | Who or what owns this responsibility? |
| Authority | A requirement or permission lacks a justified source | What gives this authority? |
| Dependency | A behavior or conclusion requires something not established | What must exist or remain true for this to work? |
| Necessity | Something is treated as required without demonstration | Why must this exist? |
| Universality | A local result is being treated as generally true | Under what conditions is this true? |
| Ambiguity | More than one material interpretation remains possible | What distinction would separate these meanings? |
| Duplication | Two things appear to own the same role | Why do both appear to own this? |
| Exception | Special treatment exists without sufficient explanation | What condition justifies this exception? |

These patterns are observations, not a closed taxonomy. If none faithfully
describes the tension, preserve the unmatched pattern for Forge
investigation rather than forcing a classification.

More than one pattern may apply. Classification narrows the question space;
it does not by itself select the Question.

## 6. Expose Candidate Uncertainties

List the unresolved claims that could account for, govern, or materially
constrain the tension.

For each candidate, record:

- the claim that remains unresolved;
- whether it is Demonstrated, Reported, or Assumed;
- the evidence that presently supports or contradicts it;
- what depends upon it; and
- what observation or analysis could distinguish it from the alternatives.

Candidates SHALL be expressed so that contrary evidence remains possible.

Do not convert candidate explanations into facts merely because they are
plausible, familiar, or the only explanations presently listed.

## 7. Trace Dependencies

Inspect each candidate uncertainty for prerequisites.

Ask:

- What must be true before this candidate can be meaningfully investigated?
- Would its resolution depend upon another unresolved claim?
- Can one earlier Question eliminate several later candidates?
- Is the proposed test interpreting a result that has not yet been shown to
  exist?

Move toward the earliest unresolved dependency that materially constrains
the investigation.

Dependency tracing does not mean that every imaginable dependency must be
resolved. Trace only dependencies whose uncertainty can change the present
engineering conclusion or the responsibility of the next Investigation.

## 8. Rank Candidate Questions

**Candidate Questions:**

1. Do the right-side props still operate when driven directly at the first
   right arch by the test controller previously used indoors, while bypassing
   the deployed controller and extension?
2. What voltage is present at the accessible right-side boundaries under the
   documented connection and operating conditions?
3. Does the extension deliver a valid data signal referenced to the same
   ground?
4. Does the deployed controller configuration address the right-side pixels
   as intended?
5. Was the first right-side pixel or another early component in the chain
   damaged or disconnected during installation?

Question 1 has priority because it reproduces a previously successful test
after the props were moved into the yard. Its answer can divide the
investigation into two major branches:

- If the props operate, the installed props remain functional under the test
  conditions, and the investigation returns to the deployed delivery path,
  controller, configuration, power, data, ground, or their interaction.
- If the props do not operate, damage, changed wiring, changed connections, or
  a material difference between the indoor and deployed test conditions
  remains unresolved.

Failure during this test would not, by itself, prove that a particular pixel
is defective. The test conditions must first be compared with those of the
successful indoor test.

## 9. Formulate the Question

Write one Question that:

- identifies the unresolved relationship;
- declares the relevant scope or conditions;
- can be answered by observation, analysis, or bounded investigation;
- permits confirming and contradicting evidence;
- does not prescribe a cause, remedy, or desired conclusion; and
- does not combine independent investigative responsibilities.

A useful diagnostic form is:

> Under [relevant conditions], does [specific relationship or behavior]
> satisfy [inspectable criterion]?

A useful foundational form is:

> What [responsibility, authority, dependency, necessity, scope, distinction,
> or condition] justifies [specific claim or relationship]?

These are aids, not mandatory sentence structures.

## 10. Test the Question Before Investigation

Before accepting the Question, ask:

- What observation caused this Question to arise?
- What unresolved relationship will its answer address?
- What would a confirming answer establish?
- What would a contradicting answer establish?
- What would neither answer establish?
- Which candidate explanations could it eliminate?
- What assumptions would still remain?
- Does answering it require another Question first?

If the Question cannot survive this inspection, revise it or return to the
unresolved relationship.

## 11. Record the Selection Rationale

Preserve the reasoning chain:

```text
Observation
    ↓
Engineering Tension
    ↓
Working–Failing Boundary
    ↓
Unresolved Relationship
    ↓
Investigation Pattern
    ↓
Candidate Uncertainties
    ↓
Dependency Tracing
    ↓
Selected Question
```

The record SHALL be sufficient for another engineer to inspect why this
Question, rather than another available Question, was selected.

---

# Question Quality Failures

A candidate Question SHALL be revised when it exhibits one or more of the
following conditions:

- **Embedded conclusion** — "Why is the jumper defective?"
- **Embedded remedy** — "Where should a signal booster be installed?"
- **Unbounded scope** — "Why does the system not work?"
- **Compound responsibility** — "Is power correct, is data valid, and should
  the controller be replaced?"
- **Unobservable wording** — terms such as *proper*, *bad*, or *reliable* are
  used without an inspectable criterion;
- **Unsupported premise** — the Question treats an untested assumption as
  demonstrated;
- **No discriminating consequence** — every possible answer leaves the same
  uncertainty unchanged;
- **Skipped dependency** — the Question requires an earlier unresolved
  relationship to have already been established; or
- **Preferred-answer testing** — evidence is sought only in forms capable of
  confirming the favored explanation.

---

# Multiple Valid Questions

An investigation may reveal several justified Questions. The Forge does not
require the engineer to pretend that only one exists.

When Questions are independent, they may be investigated separately or in
parallel if resources and procedural constraints permit. Their evidence and
conclusions SHALL remain distinguishable.

When Questions are dependent, investigate the earliest unresolved dependency
first.

When the ordering cannot yet be justified, preserve the competing Questions
and formulate a Question whose responsibility is to determine that ordering.

---

# Suspension and Evidentiary Limits

Question selection may correctly end without an answer.

The Investigation SHOULD suspend when:

- required evidence is not presently available;
- obtaining the evidence would be unsafe or unauthorized;
- a higher-confidence reference artifact is reasonably expected to provide
  greater evidentiary value;
- the observation conditions cannot presently be reproduced; or
- proceeding would require silently accepting a material assumption.

Suspension SHALL preserve:

- the selected Question;
- why it was selected;
- the evidence required to continue;
- the present evidentiary limit; and
- any conditions that must be restored before Investigation resumes.

Suspension is not bedrock and does not justify a conclusion.

---

# Bedrock Within Question Selection

Question selection reaches bedrock when disciplined dependency tracing no
longer reveals a more fundamental Question that can materially change the
current engineering justification.

Bedrock is recognized from the investigation record. It is not declared
because the engineer is tired, because no convenient test remains, or because
an answer is acceptable.

Future evidence may reveal new engineering tension and reopen question
selection.

---

# Worked Field Example — Silent Right-Side Pixels

The following example preserves the initial use of this procedure outside the
Forge–Stage Method's originating software and methodology work.

## Preserved Engineering State

The complete Christmas display contains more than 7,000 individually
addressable pixels and LEDs. The subsystem involved in this investigation
contains a 1,472-pixel mega tree and eight additional props, for a subsystem
total of 1,844 pixels.

The eight additional props consist of four arches and four 3D mini trees.
They operated when tested indoors using an independently powered test
controller.

In the deployed configuration, a different controller is used. Two arches and
two mini trees on the left operate. Two arches and two mini trees on the right
do not respond. The right-side group is reached through an approximately
12-foot, three-conductor jumper carrying 5 V power, data, and ground from the
second left arch. The props operate during independent testing, and continuity
through the deployed wiring has been reported. The first pixel on the failing
side illuminates in one fixed color but does not change color.

The test controller was built because the complete display contains too many
pixels and distributed props to diagnose reliably as one system. It creates an
independent diagnostic boundary by supplying known 5 V power, ground, and data
directly to an isolated display section.

Its responsibility is to determine whether a selected display section can
operate independently of the full-show controller and its deployed delivery
path.

Voltage at the first failing pixel under deployed operating load has not been
measured. The first pixel and its electrical connections are enclosed within
a solid prop casing, so voltage cannot be measured directly at that behavioral
boundary without opening or altering the prop.

Accessible measurement boundaries exist at:

- the output connector of the second left arch;
- the right-side end of the extension while disconnected from the right arch;
  and
- the output connector of the first right arch after the extension has been
  reconnected.

The test controller previously used to operate the props indoors remains
available. It has its own 5 V power supply and independently supplies 5 V,
ground, and data.

The controller can be connected directly to the input of the first right arch
while the props remain installed in the yard. This completely disconnects the
right-side section from the deployed controller and 12-foot extension.

The test controller is specifically used to inspect an isolated display
section for damaged props, connections, or pixels.

Whether the test controller supplies both power and data, or supplies data
while using a separate power source, SHALL be recorded as part of the test
conditions.

## Derivation

**Engineering tension:** The right-side props operate independently but do not
respond in the deployed configuration.

**Working–failing boundary:** Working behavior ends before the approximately
12-foot jumper; shared failure begins after it.

**Unresolved relationship:** The jumper must deliver both usable 5 V power and
a valid data signal referenced to ground, but continuity demonstrates only a
conductive path. It does not demonstrate adequate voltage under load or valid
signal delivery.

**Investigation pattern:** Dependency. Valid right-side pixel operation
depends upon local power integrity before data behavior can be interpreted
without conflating the two uncertainties.

**Candidate Questions:**

1. Do the right-side props still operate when independently supplied with
   5 V, ground, and data by the test controller connected directly to the
   first right arch?
2. Does the jumper deliver a valid data signal referenced to the same ground?
3. Does the deployed controller configuration address the right-side pixels
   as intended?

Question 1 has priority because it recreates the independently powered test
that previously operated the right-side props. It bypasses the deployed
controller, the 12-foot extension, and their power, ground, and data paths.

Its answer separates the investigation into two major branches:

- If the props operate, the right-side display section remains functional
  under the recorded test conditions. The deployed controller, extension,
  power delivery, ground reference, data delivery, configuration, or their
  interaction remains responsible for the unresolved failure.
- If the props do not operate, the unresolved failure remains within the
  isolated right-side section or within a material difference between the
  original indoor test and the new yard test.

Failure during this test would justify inspecting the first nonresponsive
pixel, its input connection, and subsequent dependencies. It would not, by
itself, prove which particular pixel or connection is defective.

Questions 2 and 3 remain justified candidates. Question 1 comes first because
the fixed illuminated pixel demonstrates the presence of some power, not the
voltage available under operating load. Until that voltage is observed, the
pixel's failure to respond to data cannot be interpreted independently of its
local power condition.

## Initially Selected Question

> What voltage is measured between the local power and ground conductors at
> the first right-side pixel while the deployed display is connected and
> operating, both with the pixels commanded off and with them commanded to
> full white?

This became the next selected Question after direct measurement at the first
pixel was found to be inaccessible. It remained selected until an additional
accessible test was identified.

This example does not conclude that the jumper, power delivery, data signal,
controller, or pixel is defective. It demonstrates how preserved evidence
selects the next Question without requiring the engineer to know the answer.

---

## Access Constraint

[Explanation of why direct measurement is inaccessible]

## First Reformulated Question

[Question using the accessible measurement boundaries]

## Additional Investigation Access

The engineer identified that the test controller used during the successful
indoor test remains available and can be connected directly to the first right
arch in the yard.

This test can bypass both the deployed controller and the 12-foot extension
while leaving the right-side props in their installed physical condition.

The newly available test can eliminate or retain the entire prop-damage branch
before separate power and data measurements are interpreted. The ordering of
the candidate Questions was therefore reconsidered.

## Current Selected Question

> Do the right-side props operate when the deployed extension is completely
> disconnected and the test controller independently supplies 5 V, ground,
> and data directly to the input of the first right arch?

The Investigation SHALL record:

- confirmation that the deployed extension was completely disconnected before
  the test controller was connected;
- the voltage supplied by the test controller at its accessible output;
- the controller configuration and pixel count;
- which right-side props are connected;
- whether the same cables and adapters used indoors are being reused;
- which pixels illuminate or respond;
- whether the fixed-color first pixel changes; and
- every material difference between the successful indoor test and the new
  yard test.

The Investigation is suspended pending this test.

A successful result would demonstrate that the right-side props remain
operational under the recorded test conditions. It would not independently
establish whether the deployed failure is caused by power delivery, data
delivery, ground reference, controller configuration, or an interaction among
them.

An unsuccessful result would retain prop damage or changed internal connection
as candidates. It would not, by itself, prove that the first or second pixel is
defective.

---

# Human and Machine Use

An engineer may perform this procedure without an artificial-intelligence
system. Worksheets, inspection records, physical diagrams, measurements, and
peer discussion may be used to preserve and examine the reasoning chain.

An AI system may accelerate comparison, expose assumptions, propose candidate
patterns, or help formulate Questions. It SHALL NOT be treated as the source
of engineering truth. Its proposals remain accountable to the same evidence,
dependency tracing, question-quality tests, and Engineering Authority as those
of a human participant.

The method remains responsible for making the derivation inspectable whether
the Questions were proposed by a novice, an experienced engineer, a
multidisciplinary team, or an AI system.

---

# Outputs

The output of this method is one of the following:

- a selected Question and its inspectable derivation;
- a preserved set of independent Questions with justified ordering;
- a suspended Question with an explicit evidentiary limit; or
- a record of Bedrock Recognition.

The output is not an engineering answer, Discovery, decision, requirement, or
authorization.

---

# History

| Version | Status | Description |
|---|---|---|
| 0.1.0 | Draft | Initial human-operable question-selection procedure, including the Silent Right-Side Pixels field example. |
