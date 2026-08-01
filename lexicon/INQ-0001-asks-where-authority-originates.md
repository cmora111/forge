# INQ-0001 — What gives the originating source the authority to require anything at all?

## Status

UNDER INVESTIGATION

---

## Question

What gives a Stage Method verb the authority to govern its implementations?

---

## Motivation

As the Stage Method evolved, verbs such as `stage-backup`,
`stage-create`, and `stage-verify` emerged as fundamental engineering
operations.

A question naturally arose:

Does an implementation define the behavior of a verb,
or does the verb possess an authority that implementations
must obey?

If the implementation determines the meaning of the verb,
then multiple incompatible implementations could redefine
the Stage Method.

If, however, the verb possesses authority independent of any
implementation, then implementations become adapters whose
responsibility is to faithfully realize the specification of the verb.

This inquiry seeks to determine the originating source of that authority.

---

## Observations

Current observations include:

- Multiple implementations of the same verb should behave consistently.
- An implementation may change while the meaning of the verb remains unchanged.
- Implementations appear to derive their legitimacy from conformity to the verb, not the other way around.
- This suggests that authority may exist above the implementation layer.

---

## Hypotheses

Possible hypotheses include:

1. Authority originates from the specification of the verb.
2. Authority originates from constitutional principles of the Stage Method.
3. Authority originates from dependencies that every valid implementation must satisfy.
4. Authority originates elsewhere and has not yet been identified.

No hypothesis has yet been established.

---

## Related Concepts

- Verb
- Specification
- Adapter
- Authority
- Dependency
- Invariant

---

## Related Inquiries

_None currently._

---

## Notes

This inquiry was discovered while separating the Stage Method
from project-specific implementations.

The question arose after recognizing that adapters should realize
verbs rather than define them.

No conclusion has yet been reached.
