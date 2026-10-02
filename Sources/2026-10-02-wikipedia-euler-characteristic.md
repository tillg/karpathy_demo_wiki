# Euler characteristic (Wikipedia)

*Source: https://en.wikipedia.org/wiki/Euler_characteristic (accessed 2026-10-02). Summarised in own words.*

The **Euler characteristic** χ is a single integer attached to a shape. For a polyhedron, or any surface cut into
polygons, count vertices V, edges E and faces F and compute

  χ = V − E + F.

A cube gives 8 − 12 + 6 = 2, and so does every other convex polyhedron. The surprising part is that the answer
does not depend on how you cut the surface up: it is a property of the surface itself.

**Values to remember.**

| Surface | χ |
|---|---|
| sphere | 2 |
| torus | 0 |
| real projective plane | 1 |
| Klein bottle | 0 |

For a closed orientable surface with g handles (genus g), χ = 2 − 2g.

**History.** The number was first defined for polyhedra and used to prove results about them, including the
classification of the Platonic solids. Euler stated the formula for convex polyhedra in 1758 but did not rigorously
prove that it is invariant. It was later generalised through homology theory to spaces of any dimension.

**Properties.** χ is a *homotopy invariant*: spaces that deform into each other share the same value. It also
behaves well with products: χ(M × N) = χ(M) · χ(N). For instance the torus is a circle times a circle, and the
circle has χ = 0, so χ(torus) = 0.

Note: the Euler characteristic alone does not tell sphere-like shapes apart from everything (the torus and the Klein
bottle both have 0); combined with orientability it classifies closed surfaces.
