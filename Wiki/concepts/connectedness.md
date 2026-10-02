---
type: concept
tags: [mathematics, topology]
updated: 2026-10-02
sources: [2026-10-02-notes-topology-study-log.md]
related: [open-set, continuity, homeomorphism, topological-invariants-overview]
---

# Connectedness

**Intuition:** the space is all in one piece.

**Definition:** X is connected if it cannot be written as the union of two disjoint nonempty [[open-set]]s.
*Path-connected* (any two points joined by a continuous path) is stronger: path-connected implies connected, but the
topologist's sine curve is connected without being path-connected.

**Examples:** any interval is connected; (0, 1) ∪ (1, 2] is not.

**Use as an invariant:** a [[continuity|continuous]] image of a connected space is connected (the intermediate
value theorem in disguise). Removing one point cuts a line in two but leaves a plane in one piece, so they are not
[[homeomorphism|homeomorphic]]. See [[topological-invariants-overview]].
