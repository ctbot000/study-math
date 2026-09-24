---
title: A piecewise bijection fills each gap in the range exactly — in either direction
area: algebra
tags: [function, bijection, piecewise]
added: 2026-09-25
---

## Idea

When the outer pieces of a function already cover most of $\mathbb{R}$, a middle
piece makes the whole a bijection (일대일대응) only by hitting the leftover gap
exactly, each value once. A continuous piece does that by running monotonically
from one end of the gap to the other — and backwards works as well as forwards,
so the bijection need not be monotone.

## Definition

Let $f=h$ outside $(p,q)$, where $h$ is one-to-one with values exactly
$\mathbb{R} \setminus (A,B)$, and let $f=g$ on $(p,q)$ with $g$ continuous on
$[p,q]$. Then $f$ is a bijection if and only if $g$ is strictly monotone on
$(p,q)$ and $g(p)$, $g(q)$ are $A$ and $B$ — in either order.

For a quadratic $g$ with axis $x=v$, monotone on $(p,q)$ means $v \le p$ or
$v \ge q$.

## Why it holds

Bijective means the pieces' images are disjoint and together cover
$\mathbb{R}$, so $g$ must send $(p,q)$ onto exactly $(A,B)$, one-to-one. A
continuous one-to-one function on an interval is strictly monotone — a turn
would repeat a value by the intermediate value theorem — so its image is the
open interval between $g(p)$ and $g(q)$.

## Example

$f(x)=x$ for $x \le 0$ or $x \ge 1$, and $f(x)=1-x$ for $0 < x < 1$. The outer
pieces leave the gap $(0,1)$ and the middle piece covers it backwards: $f$ is a
bijection, yet it is not monotone and jumps at both joins.

## Pitfalls

Trying only the filler that runs the same way as the outer pieces finds half
the candidates. When the question asks for a maximum or minimum, the reversed
one is often the answer.

The vertex condition keeps its equality: a parabola is strictly monotone on
each side of its axis, axis included. Writing $v < p$ drops the boundary case,
and a quadratic pinned by three conditions can land exactly there.

"One-to-one implies monotone" needs continuity on an interval; a piecewise $f$
that jumps at the joins escapes it.

## See also

[A quadratic through two given points is the chord plus $a(x-p)(x-q)$](quadratic-is-chord-plus-product.md)
