---
title: A circle tangent to both coordinate axes has center $(\pm r, \pm r)$
area: geometry
tags: [circle, tangency, coordinate-geometry]
added: 2026-09-06
---

## Idea

A line is tangent to a circle exactly when the distance from the center to the
line equals the radius. For the coordinate axes those distances are just $|y|$
and $|x|$, so "tangent to both axes" collapses three unknowns into one.

## Definition

A circle of radius $r>0$ touches both axes if and only if its center $(a,b)$
satisfies $|a|=|b|=r$. The quadrant fixes the signs:

$$\text{I}:(r,r)\quad \text{II}:(-r,r)\quad \text{III}:(-r,-r)\quad \text{IV}:(r,-r)$$

## Why it holds

Distance from $(a,b)$ to the $y$-axis ($x=0$) is $|a|$; to the $x$-axis is $|b|$.
Tangency to each forces both to equal $r$.

## Example

Centers constrained to lie on $(x-1)^2+(y-1)^2=18$:

- Quadrant III, center $(-r,-r)$: $2(r+1)^2=18 \Rightarrow r=2$.
- Quadrant II, center $(-r,r)$: $(r+1)^2+(r-1)^2=2r^2+2=18 \Rightarrow r=2\sqrt2$.

The cross terms cancel in II and reinforce in III, so the two quadrants give
genuinely different equations — not the same answer with a sign flipped.

## Pitfalls

The center sits on $y=x$ (quadrants I, III) or on $y=-x$ (II, IV), never both,
so each quadrant needs its own equation.

Discard roots with $r\le 0$ instead of taking $|r|$: in the example
$r+1=-3$ gives $r=-4$, which is not a radius-4 circle somewhere else — it is no
circle at all.

## See also

[An odd solution count across two quadratics pins the parameter at a degenerate case](../algebra/odd-count-forces-a-degenerate-case.md)
