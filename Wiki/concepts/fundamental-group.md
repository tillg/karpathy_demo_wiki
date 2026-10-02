---
type: concept
tags: [mathematics, topology, algebraic-topology]
updated: 2026-10-02
sources: [2026-10-02-wikipedia-fundamental-group.md, 2026-10-02-mactutor-history-of-topology.md, 2026-10-02-notes-topology-who-is-who.md]
related: [homotopy, poincare-conjecture, topological-invariants-overview, henri-poincare, euler-characteristic]
---

# Fundamental group

**Intuition:** record which loops in a space can be shrunk to a point and which get stuck around a hole.

**Definition:** fix a base point; π₁(X) is the set of loops at that point up to [[homotopy]]. Running one loop after
another is the group operation.

| Space | π₁ |
|---|---|
| plane, disk, 2-sphere | trivial ("simply connected") |
| circle | ℤ (winding number) |
| torus | ℤ × ℤ |

It is a homotopy invariant, so different groups prove spaces differ — a sphere is not a torus. Introduced by
[[henri-poincare]]; trivial π₁ is the hypothesis of the [[poincare-conjecture]]. Compare
[[topological-invariants-overview]].

Date: Wikipedia gives 1895 (*Analysis Situs*); MacTutor's Poincaré biography says the group appears in his 1894
paper.
