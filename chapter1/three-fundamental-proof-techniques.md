Chapter One: Sets, Relationss, and Languages
-----------

## Three Fundamental Proof Techniques

Each and every proof is different, because every prrof is designed to establish a different result. But there are different ways, patterns, rules, tricks, that can be utilized again and again to make things easier. Similarly, we introduce some of those ways, or rules, or tricks that will help us prove many proofs.

There are three such techniques that we will cover:
1. The Principle of Mathematical Induction
2. The Pigeonhole Principle
3. The Diagonalization


### The Principle of Mathematical Induction

Let A be a set of natural numbers such that: 
- 0 ∈ A, and
- for each natural number n, if {0,1,...,n} ⊆ A, then n + 1 ∈ A

Then A = N.

For a more practical approach, we use mathematical induction to prove assertions of the following form: "For all natural numbers n, property P is true". (i.e, `say A =  {n : P is true for n}` When we apply mathematical induction to prove that. 

1. We first show that A ∈ 0. (i.e, P is true for 0)
2. Then we assume that the property P holds true for any fixed but arbitary n.
3. Then we modify our hypothesis and show tht P holds true for n+1

If these conditions are satisfied , then using Mathematical Induction, we can prove that A = N

### The Pegionhole Prinicple

It says that if A and B are finite sets, |A| > |B|, then there is no one-to-one function from A to B. 

In fancy way, let us consider A as the set of pegions, and B is the set of pegionholes. Now, |A| > |B| will mean that there are more pegions than the pegionhole. So, we may have to fit other pegions in one pegionholes, which eventually will it impossible to have bijection between A and B.

Proof using Pegionhole Principle: 
1. Suppose |B| = 0, that is B = Ø . Then there is no function f : A -> B whatsover, let alone a one-to-one function.

.................

More on this chapter later.
