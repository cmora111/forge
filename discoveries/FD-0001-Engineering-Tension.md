# FD-0001 — Engineering Tension

**Status:** Accepted  
**Version:** 0.1.0

---

## Summary

Engineering tension is the observable indication that an engineering model, decision, artifact, or architecture contains unresolved uncertainty.

The tension may appear as ambiguity, contradiction, overlap, unexplained authority, missing dependency, unnecessary complexity, or a conclusion that cannot yet justify itself.

Engineering tension does not prove that the current design is wrong. It demonstrates that the design has not yet earned sufficient confidence to be accepted without further examination.

---

## Context

This discovery emerged while developing the Forge–Stage Method during the restoration of a Creality CR-10S 3D printer.

Questions concerning stage lifecycle, artifact ownership, frozen history, restoration, command authority, and specification structure repeatedly produced a recognizable condition: a proposed answer appeared plausible, yet some part of the engineering model remained unresolved.

The next useful Forge question did not arise from arbitrary curiosity. It arose from locating the unresolved part of the model.

This recurring condition became identifiable as engineering tension.

---

## Engineering Tension

Engineering work commonly reaches points where a proposal appears complete but still produces one or more of the following conditions:

- two components appear to own the same responsibility;
- a requirement exists without a clearly established authority;
- a concept depends upon something that has not yet been defined;
- a new component is proposed without demonstrated necessity;
- a principle appears tied to one implementation;
- a state or term permits contradictory interpretations;
- a conclusion answers the immediate question but leaves a deeper dependency unresolved;
- the architecture requires an exception that cannot yet justify itself.

These conditions create uncertainty about whether the engineering model is complete, coherent, and trustworthy.

The uncertainty is not noise to be ignored. It is evidence that further investigation is required.

---

## Forge Investigation

The Forge investigation began by observing how productive questions were selected during engineering discussions.

The initial assumption was that the Forge began with a question.

Further inspection showed that the question was preceded by something else: recognition that the current engineering model was unstable, incomplete, ambiguous, or insufficiently justified.

The investigation therefore asked:

1. What causes the need for another Forge question?
2. Why do some questions reduce uncertainty while others merely add discussion?
3. What common condition exists before responsibility, authority, dependency, necessity, or universality questions are asked?
4. Does that condition indicate error, or does it indicate unresolved engineering uncertainty?
5. Can that condition be recognized and taught?

The investigation found that the next useful question consistently originated from an unresolved relationship within the engineering model.

The unresolved relationship was the source of the question.

---

## Discovery

> **The Forge begins with the recognition of engineering tension.**

Engineering tension is the observable indication that unresolved engineering uncertainty remains within a model, decision, artifact, requirement, or architecture.

The Forge SHALL treat recognized engineering tension as a signal to suspend acceptance and begin disciplined investigation.

Engineering tension SHALL NOT, by itself, be interpreted as proof that the current design is incorrect.

It SHALL be interpreted as evidence that the current design has not yet fully justified itself.

---

## Bedrock

Bedrock was reached when the investigation no longer produced a more fundamental cause for the need to ask another question.

Questions concerning responsibility, authority, dependency, necessity, and universality were found to be responses to engineering tension rather than its cause.

The investigation therefore established the following dependency:

```text
Engineering Model
        ↓
Unresolved Relationship
        ↓
Engineering Tension
        ↓
Forge Trigger
        ↓
Forge Question
```

Further questions depended upon the recognition of engineering tension rather than undermining it.

Engineering tension was therefore accepted as the originating condition of Forge investigation.

---

## Rationale

A question-selection method based only on intuition cannot be reliably explained, taught, inspected, or repeated.

Recognizing engineering tension provides an observable basis for invoking the Forge.

This discovery explains why the Forge does not begin by asking every possible question. It begins by identifying where uncertainty is concentrated and then selecting a question capable of reducing that uncertainty.

Engineering tension also protects the Forge from premature acceptance. A proposal may be elegant, familiar, or apparently complete while still containing unresolved relationships.

The continued presence of tension means the work has not yet earned acceptance.

---

## Implications

This discovery establishes that:

- Forge investigations begin with observation rather than arbitrary questioning;
- uncertainty should be localized before a question is formulated;
- engineering discomfort may contain useful architectural information;
- the first answer should not be accepted while material tension remains;
- Forge triggers may be classified according to the kind of tension observed;
- question selection can become a teachable engineering discipline;
- bedrock cannot be claimed while unresolved engineering tension remains.

This discovery provides the foundation for:

- Forge Triggers;
- Dependency Tracing;
- Question Formulation;
- Bedrock Recognition;
- the Forge Decision Process.

---

## Related Discoveries

- FD-0002 — Forge Triggers
- FD-0003 — Dependency Tracing
- FD-0004 — Bedrock

---

## Related Constitutional Laws

- LAW-0001 — Every component shall have one clearly defined engineering responsibility.

---

## Related Specifications

None at the time of creation.

---

## Validation

Engineering tension has been observed during multiple Forge–Stage Method investigations, including:

- determining whether `CREATED` was a genuine lifecycle state;
- distinguishing lifecycle state from engineering outcome;
- determining whether a frozen stage could be reopened;
- distinguishing restoration from lifecycle transition;
- separating milestone accomplishment from methodology discovery;
- determining whether template filenames should repeat directory context;
- identifying independent Engineering Authority and Procedural Authority.

In each case, recognizing the unresolved relationship led to a higher-leverage question and a clearer architecture.

Broader validation across independent engineers and additional engineering domains remains future work.

This discovery remains subject to continued validation through future engineering efforts.



---

## History

| Version | Status | Description |
|---|---|---|
| 0.1.0 | Accepted | Initial formulation of Engineering Tension as the originating condition of Forge investigation. |
