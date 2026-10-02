---
type: synthesis
tags: [mathematics, topology]
updated: 2026-10-02
sources: [2026-10-02-notes-topology-study-log.md, 2026-10-02-wikipedia-fundamental-group.md, 2026-10-02-wikipedia-euler-characteristic.md, 2026-10-02-wikipedia-surface-topology.md, 2026-10-02-wikipedia-knot-theory.md, 2026-10-02-notes-topology-who-is-who.md]
related: [luitzen-brouwer, connectedness, compactness, fundamental-group, euler-characteristic, knot, homeomorphism, homotopy]
---

# Topological invariants compared

An invariant is anything that two [[homeomorphism|homeomorphic]] spaces must share. Invariants can only prove
spaces *different*: if they agree, the question stays open (unless a classification theorem says otherwise).

| Invariant | Type | Survives homotopy equivalence? | Separates… | Fails to separate… |
|---|---|---|---|---|
| [[connectedness]] | yes / no (or number of components) | yes | line vs plane (remove a point) | circle vs sphere |
| [[compactness]] | yes / no | **no** — the real line is homotopy equivalent to a point but not compact | [0, 1] vs (0, 1) | sphere vs torus |
| [[euler-characteristic]] | integer | yes | sphere (2) vs torus (0) | torus vs Klein bottle (both 0) |
| [[fundamental-group]] | group | yes | sphere (trivial) vs torus (ℤ × ℤ) vs circle (ℤ) | disk vs point (homotopy equivalent, not homeomorphic) |
| knot invariants (crossing number, Alexander / Jones polynomial) | integer / polynomial | — (about the embedding, not the space) | unknot vs trefoil | nothing about the space itself — every knot is a circle |

**Observations.**

- The cheap invariants (connectedness, compactness) are yes/no and blunt. The [[euler-characteristic]] is one number;
  the [[fundamental-group]] carries the most information of the three, but is hardest to compute.
- [[homotopy]]-invariant quantities can't tell a disk from a point; that needs a homeomorphism invariant that is
  not a homotopy invariant, such as dimension ([[luitzen-brouwer]]'s invariance of dimension).
- For closed surfaces the [[classification-of-surfaces]] closes the gap: χ plus orientability is a *complete*
  invariant. For 3-dimensional spaces, the [[poincare-conjecture]] shows π₁ is enough to recognise the 3-sphere.
- [[knot]]s are all homeomorphic to a circle, so space invariants are useless there; knot invariants measure how the
  circle sits in space.
