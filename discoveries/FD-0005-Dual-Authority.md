# FD-0005 — Dual Authority

**Status:** Accepted

**Version:** 0.1.0

---

# Summary

The Forge discovered that engineering investigations are governed by two
independent authorities.

Engineering Authority determines what is justified.

Procedural Authority determines what is permitted.

Neither authority derives its authority from the other.

---

# Engineering Tension

During development of the Forge–Stage Method, engineering decisions
repeatedly became entangled with procedural decisions.

Questions such as:

- Should a frozen stage be reopened?
- May a frozen stage be reopened?
- Does engineering justify the change?
- Does procedure permit the change?

appeared to ask a single question.

Inspection revealed that they actually represented two distinct
questions governed by different authorities.

The absence of a clear distinction repeatedly produced architectural
confusion.

---

# Discovery

Engineering Authority determines whether an engineering conclusion is
justified.

Procedural Authority determines whether an engineering action is
permitted.

Each governs a distinct aspect of engineering practice.

Engineering Authority and Procedural Authority are independent 
authorities because they govern different responsibilities. 

Neither authority can replace or derive its authority from the other.

# Rationale

Engineering investigations exist to discover justified engineering
understanding.

Procedures exist to govern disciplined execution.

Confusing these responsibilities causes engineering justification 
to become dependent upon procedure, or procedural permission to 
become dependent upon engineering judgment.

Neither outcome preserves architectural integrity.

Maintaining the independence of these authorities preserves both
engineering integrity and procedural integrity.

Engineering remains responsible for determining what is justified.

Procedure remains responsible for determining what is permitted.

---

# Implications

Recognition of Dual Authority establishes that:

- engineering conclusions cannot be justified by procedure alone;
- procedural permission cannot justify an engineering conclusion;
- justified engineering conclusions do not automatically authorize
  procedural action;
- procedural authorization does not determine engineering correctness.

Engineering and procedure therefore cooperate without replacing one
another.

---

# Relationship to Other Discoveries

This discovery builds upon:

- FD-0001 — Engineering Tension
- FD-0002 — Investigation Pattern Recognition
- FD-0003 — Dependency Tracing
- FD-0004 — Bedrock Recognition

The distinction between Engineering Authority and Procedural Authority
provides the foundation for Lifecycle Determinism and subsequent Forge
governance.

---

# Validation

Dual Authority emerged repeatedly during investigation of lifecycle
behavior, restoration, frozen stages, constitutional governance, and
engineering decision making.

Each investigation demonstrated that engineering justification and
procedural permission remained independent despite appearing closely
related.

Broader validation across additional engineering disciplines remains
future work.

This discovery remains subject to continued validation through future
engineering efforts.

---

# History

| Version | Status | Description |
|----------|--------|-------------|
| 0.1.0 | Accepted | Initial formulation of Dual Authority. |
