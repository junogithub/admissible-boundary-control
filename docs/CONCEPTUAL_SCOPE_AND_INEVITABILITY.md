# Conceptual Scope and Inevitability of Admissible Boundary Folding

## 1. Purpose

This document defines the conceptual scope of the
Admissible Boundary Folding Control Framework.

It is not an implementation guide.
It does not disclose algorithms, system designs, or tuning rules.

Its sole purpose is to fix the **conceptual boundary**
within which any realization of the framework must necessarily fall.

---

## 2. Conceptual Boundary

The framework is defined by the following invariant statement:

> System safety is ensured by folding the trajectory of a measurable
> hazard deviation ε(t) back into an admissible domain Γ_c
> by enforcing a negative boundary-normal component u(t) < 0.

This definition is:
- Independent of system dimension
- Independent of full-state modeling
- Independent of specific actuation mechanisms

Only the **boundary condition** is regulated.
The full system state may remain uncontrolled.

---

## 3. Inevitability of Means

Any system that enforces u(t) < 0 relative to Γ_c
must, by necessity, involve at least one of the following conceptual categories:

1. A dissipative mechanism that guarantees monotonic reduction
   of boundary-normal deviation.

2. A boundary-crossing detection or labeling process
   capable of distinguishing admissible versus inadmissible trajectories.

3. A directional influence mechanism capable of reversing
   the sign of the boundary-normal component.

This is not a design choice.
It is a structural inevitability.

Any proposed realization, regardless of terminology or tooling,
must instantiate at least one of these categories,
and therefore remains within the same conceptual scope.

---

## 4. Non-Equivalence to Classical Control Paradigms

This framework is not a variant, extension, or tuning
of classical process control methodologies.

Key non-overlapping assumptions include:

- Classical control regulates full or reduced-order system states.
  This framework regulates only the boundary-normal hazard component.

- Classical control minimizes tracking or regulation error.
  This framework enforces topological admissibility.

- Classical control defines failure as instability or divergence.
  This framework defines failure exclusively as boundary violation.

As such, the framework is orthogonal, not incremental,
to PID, MPC, H∞, robust, or adaptive control paradigms.

---

## 5. Scope Lock

Any method, system, or architecture that:

- Defines a measurable hazard deviation ε(t),
- Defines an admissible boundary Γ_c,
- Enforces negative boundary-normal behavior u(t) < 0,

whether through physical actuation, software logic,
heuristic rules, learned systems, or hybrid approaches,

constitutes a realization within this conceptual framework.

No restriction on implementation technique
alters this classification.
