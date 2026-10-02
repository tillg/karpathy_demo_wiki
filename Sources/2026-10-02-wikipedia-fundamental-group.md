# Fundamental group (Wikipedia)

*Source: https://en.wikipedia.org/wiki/Fundamental_group (accessed 2026-10-02). Summarised in own words.*

The fundamental group turns loops in a space into algebra. Fix a **base point** in a space X and look at all loops
that start and end there. Two loops count as the same if one can be continuously deformed into the other while
keeping the base point fixed (they are *homotopic*). The set of these equivalence classes is written π₁(X).

It is a **group**: to "multiply" two loops, run through the first and then the second. The constant loop that never
leaves the base point is the identity, and running a loop backwards gives its inverse.

**Examples.**

- Euclidean space, a disk, or any contractible space: every loop shrinks to a point, so the group is trivial.
- The **circle**: π₁ is the integers ℤ. A loop is classified by its winding number — how many times it goes
  around, positive one way, negative the other. Joining loops adds the winding numbers.
- The **2-sphere**: trivial. Any loop on a ball's surface can be slid off and shrunk. A space with trivial
  fundamental group (and path-connected) is called **simply connected**.
- The **torus**: ℤ × ℤ, one integer for going around "the long way" and one for "through the hole".

**History.** Henri Poincaré introduced the fundamental group in 1895 (in *Analysis Situs*).

**Why it matters.** It is a *homotopy invariant*: spaces that are homotopy equivalent have isomorphic fundamental
groups. So if two spaces have different fundamental groups, they cannot be homeomorphic. That is how you prove,
for example, that a sphere and a torus are genuinely different.
