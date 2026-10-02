---
type: concept
tags: [mathematics, topology]
updated: 2026-10-02
sources: [2026-10-02-notes-topology-study-log.md, 2026-10-02-wikipedia-fundamental-group.md]
related: [fundamental-group, continuity, homeomorphism, henri-poincare]
---

# Homotopy

**Intuition:** a film that continuously morphs one map into another.

**Definition:** maps f, g: X → Y are homotopic if there is a continuous H: X × [0, 1] → Y with H(x, 0) = f(x) and
H(x, 1) = g(x) — the second coordinate is time.

**Homotopy equivalence and contractibility:** two spaces are homotopy equivalent if maps back and forth compose to
something homotopic to the identity. A space is *contractible* if it is homotopy equivalent to a point: a solid
disk is, a circle isn't.

**Example:** a disk and a point are homotopy equivalent but not [[homeomorphism|homeomorphic]] — homotopy is
coarser.

Loops up to homotopy give the [[fundamental-group]]. Introduced by [[henri-poincare]] (1895).
