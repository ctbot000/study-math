---
title: An absolute-value equation solved by cases keeps only the roots inside each case
area: algebra
tags: [absolute-value, equation, case-analysis]
added: 2026-09-28
---

## Idea

![y = |x − 1| with both branches extended as dashed lines; y = 2x meets the V at x = 1/3 and the dashed extension at x = −1](absolute-value-cases-keep-their-own-roots.svg)

Splitting $|x - c|$ into cases swaps the V for one straight branch at a time,
but each case equation solves against that branch's whole line, not just its
half. A root on the wrong half is where the other curve meets the dashed
extension, not the graph, and it has to be thrown out.

## Definition

To solve an equation containing $|x - c|$:

- Case $x \ge c$: replace $|x - c|$ by $x - c$, solve, keep only roots with $x \ge c$.
- Case $x < c$: replace $|x - c|$ by $c - x$, solve, keep only roots with $x < c$.

The solution set is the union of what the two cases keep.

## Example

$|x - 1| = 2x$. Case $x \ge 1$: $x - 1 = 2x$ gives $x = -1$, which is not
$\ge 1$, so it is rejected. Case $x < 1$: $1 - x = 2x$ gives $x = \tfrac13$,
kept. One solution, $x = \tfrac13$.

## Pitfalls

Test each root against its own case, not the other one. A root rejected in one
case is not a solution at all — it does not move over to the other case.

## See also

[Two functions are equal when they agree at every point of their domain](equal-functions-agree-pointwise.md)
