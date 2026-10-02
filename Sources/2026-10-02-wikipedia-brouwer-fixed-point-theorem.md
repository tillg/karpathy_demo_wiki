# Brouwer fixed-point theorem (Wikipedia)

*Source: https://en.wikipedia.org/wiki/Brouwer_fixed-point_theorem (accessed 2026-10-02). Summarised in own words.*

**Statement.** Every continuous function from a nonempty compact convex set (for example a closed disk or a closed
ball in any finite dimension) to itself has at least one **fixed point**: a point x with f(x) = x.

**Everyday pictures.**

- Crumple a sheet of paper and drop it back onto a copy of itself lying on the table: some point of the crumpled sheet
  lies directly above the matching point of the flat one.
- Spread a map of a country on the floor inside that country: one point on the map is exactly where it depicts.
- Stir a drink gently (continuously) and let it settle: some point of the liquid ends up where it started.

**Why each assumption is needed.**

- *Same set in and out:* the function must map the set into itself.
- *Compactness (closed and bounded):* the shift f(x) = x + 1 on the whole real line has no fixed point.
- *Convexity, or at least being shaped like a disk:* rotating a circle by half a turn (x ↦ −x) moves every point,
  but once you fill in the disk, the centre stays put.

In one dimension the theorem is a consequence of the intermediate value theorem: a continuous map of [0, 1] into
itself must cross the diagonal.

**History.** The ideas came out of 19th-century work on differential equations and celestial mechanics, including
Poincaré's. Piers Bohl proved the three-dimensional case in 1904; L. E. J. Brouwer proved the general case in
1909–1910; Jacques Hadamard gave an independent proof in 1910. The theorem helped launch what is now algebraic
topology.
