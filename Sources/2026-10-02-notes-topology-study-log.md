# Topology study log — weeks 1–3

*Own notes, written while working through these pages (accessed 2026-10-02):
https://en.wikipedia.org/wiki/Connected_space, https://en.wikipedia.org/wiki/Compact_space,
https://en.wikipedia.org/wiki/Homotopy, https://en.wikipedia.org/wiki/Manifold,
https://en.wikipedia.org/wiki/Hairy_ball_theorem. Summarised in own words.*

**Week 1 — connectedness.** A space is *connected* if it can't be split into two disjoint nonempty open sets;
equivalently, the only subsets that are both open and closed are the empty set and the whole space. An interval is
connected, (0, 1) ∪ (1, 2] is not. *Path-connected* (any two points joined by a continuous path) is stronger: every
path-connected space is connected, but the "topologist's sine curve" is connected without being path-connected.
Every space falls apart into maximal connected pieces, its *components*. Key fact: the continuous image of a
connected space is connected — this is the intermediate value theorem in disguise. Trick to remember: delete one
point from a line and it falls in two; delete one point from the plane and it stays in one piece. So the line and the
plane are not homeomorphic.

**Week 2 — compactness.** Definition: every open cover has a finite subcover. Heine–Borel: in Euclidean space, compact means closed and bounded. So [0, 1] is compact, (0, 1)
and ℝ are not. Payoff: a continuous real-valued function on a nonempty compact space
is bounded and reaches its maximum (extreme value theorem). History: Bolzano (1817) on bounded sequences; Fréchet
named "compactness" in 1906; Alexandrov and Urysohn gave the open-cover form.

**Week 3 — homotopy and manifolds.** A *homotopy* between maps f, g: X → Y is a continuous H: X × [0, 1] → Y with
H(x, 0) = f(x) and H(x, 1) = g(x) — think of the second coordinate as time. A space is *contractible* if its identity
map can be deformed to a constant map: a solid disk or the real line yes, a circle no. A disk and a point are homotopy equivalent but
not homeomorphic.
A *manifold* of dimension n looks locally like n-dimensional Euclidean space: circles and lines are 1-manifolds (a
figure-eight is not — its crossing point fails), spheres and tori are 2-manifolds. A *chart* maps a patch to flat
space; an *atlas* is a set of charts covering everything. Riemann introduced the idea
in his 1854 Göttingen lecture ("Mannigfaltigkeit").

**Bonus — hairy ball theorem.** You can't comb a hairy sphere flat: every continuous tangent vector field on an
even-dimensional sphere vanishes somewhere. Poincaré proved it for the ordinary sphere in 1885, Brouwer for higher
even dimensions in 1912. A hairy torus *can* be combed: Euler characteristic 2 vs 0.
