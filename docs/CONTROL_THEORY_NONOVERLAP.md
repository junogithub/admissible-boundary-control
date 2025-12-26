# Control Theory Non-Overlap Statement

This framework is not a variant, extension, or specialization of
classical process control theories
(e.g., PID, MPC, H∞, robust, adaptive, or optimal control).

The separation is structural and non-overlapping, based on the
following fundamental assumptions.

## 1. Control Target

Classical process control regulates the full system state x(t)
or a reduced-order approximation thereof.

This framework regulates only the boundary-normal hazard component u(t),
defined relative to an admissible boundary Γ_c.

## 2. Objective Function

Process control minimizes tracking, regulation, or optimization error.

This framework enforces topological admissibility by folding the hazard
trajectory ε(t) strictly inside the admissible domain Γ_c.

No tracking or state convergence objective is defined.

## 3. State Observability

Process control assumes full or partial state estimation
(e.g., observers, filters, state reconstruction).

This framework requires only boundary crossing detectability
(i.e., whether ε(t) violates Γ_c),
not full-state observability.

## 4. Failure Definition

Process control defines failure as instability, divergence,
or unacceptable steady-state error.

This framework defines failure solely as boundary violation,
independent of internal state stability.

## 5. Theoretical Relationship

Therefore, this framework is orthogonal to classical control theory,
not incremental.

It cannot be derived as a special case, limit, or reformulation
of existing process control methodologies.

Any classification of this framework as a control-theoretic variant
constitutes a categorical error.

## Status

Conceptual classification lock-in.
This document serves as an explicit non-overlap declaration
for interpretative, legal, and technical clarity.
