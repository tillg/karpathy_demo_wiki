---
type: synthesis
tags: [mathematics, topology]
updated: 2026-10-02
sources: [2026-10-02-wikipedia-topology.md, 2026-10-02-wikipedia-fundamental-group.md, 2026-10-02-wikipedia-euler-characteristic.md, 2026-10-02-wikipedia-surface-topology.md]
related: [homeomorphism, fundamental-group, euler-characteristic, classification-of-surfaces, topological-invariants-overview]
---

# Why a coffee mug is a doughnut

The standard joke: a topologist can't tell a coffee mug from a doughnut. Here is the joke checked against the rest
of the wiki.

**1. The deformation.** Think of the mug as soft clay. Squash the cup part down into the handle until only a thick
ring is left. Nothing was cut and nothing was glued, so the mug and the doughnut (a solid torus) are
[[homeomorphism|homeomorphic]].

**2. Their surfaces agree on every invariant.** The surface of a doughnut is the torus:

| Invariant | Torus (mug surface) | Sphere (e.g. surface of a bowl without handle) |
|---|---|---|
| [[euler-characteristic]] | 0 | 2 |
| genus (handles) | 1 | 0 |
| [[fundamental-group]] | ℤ × ℤ | trivial |

**3. Why a mug is *not* a bowl.** Different χ (0 vs 2) and different π₁ prove no homeomorphism exists — the handle
is a hole that can't be removed without tearing. A mug with two handles would have genus 2 and χ = −2.

**4. The complete answer.** By the [[classification-of-surfaces]], a closed orientable surface is determined by its
genus, so "one handle" is *all* the topology there is to a mug's surface.

Caveat: the joke is about shapes, not physics — a clay model is a picture of a continuous map, not a proof. See
[[topological-invariants-overview]] for how the invariants compare.
