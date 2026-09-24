---
title: A quadratic through two given points is the chord plus $a(x-p)(x-q)$
area: algebra
tags: [quadratic, interpolation, remainder-theorem]
added: 2026-09-25
---

## Idea

Fixing two points on a parabola leaves one degree of freedom: how much of
$(x-p)(x-q)$ — zero at both points — is added to the straight line through
them. One more condition, of any kind, then pins the quadratic down.

## Definition

If $g$ is quadratic with $g(p)=P$ and $g(q)=Q$, then

$$g(x)=a(x-p)(x-q)+\ell(x),$$

where $\ell$ is the line through $(p,P)$ and $(q,Q)$ and $a \ne 0$ is the
leading coefficient.

## Why it holds

$g-\ell$ has degree at most 2 and vanishes at $p$ and $q$, so it is a constant
times $(x-p)(x-q)$. Through the remainder theorem (나머지정리), $\ell$ is the
remainder of $g$ divided by $(x-p)(x-q)$. Any degree works the same way: two
polynomials that agree at $x_1,\dots,x_k$ differ by a polynomial multiple of
$(x-x_1)\cdots(x-x_k)$.

At the midpoint $m$, with half-width $h=\tfrac{q-p}{2}$, the product equals
$-h^2$, so $g(m)=\ell(m)-ah^2$: a value there reads off $a$ directly.

## Example

Through $(0,1)$, $(2,5)$ and $(1,0)$: the chord is $\ell(x)=2x+1$, and $x=1$ is
the midpoint, so $0=\ell(1)-a=3-a$ gives $a=3$ and
$g(x)=3x(x-2)+2x+1=3x^2-4x+1$.

## Pitfalls

$a=0$ returns the chord itself, which is not a quadratic — discard it when the
problem demands degree 2.

Starting from $ax^2+bx+c$ also works, but spends two of the three equations
rediscovering the chord.

## See also

[A piecewise bijection fills each gap in the range exactly — in either direction](piecewise-bijection-fills-the-gap.md)
