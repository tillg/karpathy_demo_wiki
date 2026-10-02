---
type: concept
tags: [mathematics, topology]
updated: 2026-10-02
sources: [2026-10-02-wikipedia-topological-space.md, 2026-10-02-wikipedia-topology.md]
related: [open-set, homeomorphism, homotopy, topological-space]
---

# Continuity

**Intuition:** a continuous map sends nearby points to nearby points — no jumps, no tearing.

**Definition:** a map f: X → Y between [[topological-space]]s is continuous if the preimage of every
[[open-set]] in Y is open in X. For functions of real numbers this is the same as the epsilon–delta definition from
calculus.

**Example:** f(x) = x² is continuous; the step function that is 0 for x < 0 and 1 for x ≥ 0 is not — the preimage
of the open interval (1/2, 2) is [0, ∞), which isn't open.

Continuous images keep [[connectedness]] and [[compactness]]. A continuous bijection with continuous inverse is a
[[homeomorphism]]; a continuous deformation of a map is a [[homotopy]].
