---
type: concept
tags: [mathematics, topology]
updated: 2026-10-02
sources: [2026-10-02-wikipedia-euler-characteristic.md, 2026-10-02-mactutor-history-of-topology.md, 2026-10-02-wikipedia-surface-topology.md]
related: [leonhard-euler, classification-of-surfaces, hairy-ball-theorem, topological-invariants-overview, emmy-noether]
---

# Euler characteristic

**Intuition:** one number that counts holes, however you slice the shape.

**Definition:** cut a surface into polygons and compute χ = V − E + F (vertices − edges + faces). The result
doesn't depend on the cutting.

**Examples:** a cube: 8 − 12 + 6 = 2, as for every convex polyhedron and the sphere. Torus 0, projective plane 1,
Klein bottle 0. A closed orientable surface with g handles: χ = 2 − 2g (Lhuilier found this for solids with holes
in 1813).

It is a homotopy invariant and, with orientability, decides the [[classification-of-surfaces]]. It also explains
the [[hairy-ball-theorem]]. Named after [[leonhard-euler]] — sources disagree on the year (1750 vs 1758). Today it
is computed from [[homology]] groups (see [[emmy-noether]]).
