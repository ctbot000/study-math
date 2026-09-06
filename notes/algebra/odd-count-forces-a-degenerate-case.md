---
title: An odd solution count across two quadratics pins the parameter at a degenerate case
area: algebra
tags: [quadratic, discriminant, counting]
added: 2026-09-06
---

## Idea

When a problem splits into two quadratics in a parameter and asks for an *odd*
total number of solutions, the parameter is forced: quadratics hand out roots two
at a time, so an odd count can only come from a double root or from a root the
problem throws away.

## Definition

For $f_1(x)=0$ and $f_2(x)=0$ quadratic in $x$ with parameter $k$, the total count
is $n_1+n_2$ where $n_i \in \{0,1,2\}$. An odd total needs exactly one of:

- some $D_i = 0$ (double root — counts once), or
- a root that fails a side condition and is discarded.

Both are equations in $k$, not inequalities, so each gives finitely many
candidates — then verify the other quadratic supplies the rest of the count.

## Example

Circles tangent to both axes with center on $y=(x-1)^2+k$. The center is
$(a,\pm a)$, so
$$a^2-3a+1+k=0 \quad (y=x), \qquad a^2-a+1+k=0 \quad (y=-x)$$
with $D_1=5-4k$, $D_2=-3-4k$, and $a=0$ discarded (radius $0$).

Exactly three circles $\Rightarrow$ $D_2=0$, i.e. $k=-\tfrac34$, which leaves
$D_1=8>0$. The discarded-root route $k=-1$ kills one root in *each* quadratic and
gives two, not three.

## Pitfalls

Enumerate every candidate before picking one. $D_1=0$ gives $k=\tfrac54$, but then
$D_2<0$ and the total is $1$ — a discriminant vanishing is necessary for an odd
count, not sufficient for the count you want.

Sum the squares with Vieta's formulas (근과 계수의 관계) rather than the roots
themselves:
$a_1^2+a_2^2=(a_1+a_2)^2-2a_1a_2 = 9-\tfrac12=\tfrac{17}{2}$ beats squaring
$\tfrac{3\pm2\sqrt2}{2}$ by hand.

## See also

[A circle tangent to both coordinate axes has center $(\pm r, \pm r)$](../geometry/circle-tangent-to-both-axes.md)
