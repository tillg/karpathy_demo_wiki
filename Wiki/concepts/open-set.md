---
type: concept
tags: [mathematics, topology]
updated: 2026-10-02
sources: [2026-10-02-wikipedia-topological-space.md, 2026-10-02-notes-topology-study-log.md]
related: [topological-space, continuity, connectedness, compactness]
---

# Open set

**Intuition:** a set that, around each of its points, still contains a little room to move — it has no "edge
points" of its own. The open interval (0, 1) is open; [0, 1] is not, because at 0 you can't move left and stay inside.

**Definition:** in a [[topological-space]], the open sets are *by definition* the members of the chosen topology.
They must satisfy: empty set and whole space open, unions open, finite intersections open. A set is **closed** when
its complement is open.

**Why finite intersections only:** the intervals (−1/n, 1/n) are all open, but their intersection over all n is the
single point {0}, which isn't open in the real line.

Open sets are the raw material for [[continuity]], [[connectedness]] and [[compactness]].
