Chapter One: Sets, Relations, and Languages
===========

## Special Types of Binary Relations

Since binary relations, and used over and again, it will be helpful to have convenient ways of representing them and develop/use some terminologies for discussing their properties. A completely "random" binary relation does not have any significant internal structure; but many relations arise out of specific contexts and therefore have important regularities. 

For example: the relation that holds between two districts if they belong to the same zone has certain "symmetries" and other properties, that are worth noting, discussing and exploiting. 

We will deal with relations that exhibits similar regularities. We will only deal with a special type of binary relation on a set and itself, i.e, a relation formed by `A × A` 


### Directed Graph

Let us suppose a set `A`, and `R ⊆ A × A` be a relation of `A`. Now the relation R can be represented by a **directed graph**. 

Suppose `A = {a,b,c,d}`

and let us suppose an arbitary relation `R = {(a,b),(b,a),(a,d),(d,c),(c,c),(c,a)}`

Now, we put an small circle for each element in A. The circles are called nodes.  After drawing the nodes, we then join the two nodes (if in R) by the use of arrows. The arrows are called edges. A node can also correspond to itself, `as in (c,c)` We also use arrows in that case. From one node to another,  there is either no edge (or arrows) or there is one edge. Parallel arrows are not allowed.



![Directed-Graph](http://imgur.com/qkZFt28.jpg?1 "Directed Graph")


There is no any formal distinction between binary relations on set A and directed graphs with nodes from A. Directed graphs makes easier to abstract complex systems.

An another example of directed graph can be shown on the following diagram, which is a less-than-or-equal-to relation ( <= ) defined on natural number.

[[Figure 1-2]]

<dl>
<dt>Reflexive Relation</dt>
<dd>A relation <code>R ⊆ A × A</code> is <strong>reflexive</strong> if <code>(a, a) ∈ R for each a ∈ A</code>. As we can guess, the directed graph of representing a reflexive relation has edges (or arrows) from a node to itself. The figure shown above represents a reflexive relation. (but the figure one does not)</dd>
</dl>

<dl>
<dt>Symmetric Relation</dt>
<dd>A relation <code>R ⊆ A × B</code> is <strong>symmetric</strong> if <code>(b, a) ∈ R whenever (a, b) ∈ R</code>. Again, the directed graph of representing a reflexive relation has edges (or arrows) from a node to another node in both direction. (See figure below). Representing in a Relation set, <code>R ⊆ A × A  =  {(a,b),(b,a),(a,c),(c,a),(c,d),(d,c)}</code> represent a symmetric relation for <code>A = {a,b,c,d}</code></dd>
</dl>

[[Figure 1-3]]

A symmetric relation may also contain pairs of the form `(a, a)`, but when the symmetric relation is purely symmetric (containing only symmetric relation), then it is represented as undirected graph ,or simply a graph which is drawn without arrowheads. To get some intution, we can assume the cancellation of arrowhead since they are in both direction

[[Figure 1-4]]

A relation R is <b>anti-symmetric</b> if if whenever `(a, b) ∈ R` and `a` and `b` are distinct, then `(b, a) ∉ R`.

A binary relation R is **transitive** if whenever `(a, b) ∈ R` and `(b, c) ∈ R` , then `(a, c) ∈ R`. The directed graph below will give the intution.

[[Figure 1-5]]

<dl>
<dt>Equivalence Relation</dt>
<dl>A relation that is reflexive, symmetric, and transitive is called and <strong>equivalence relation</strong>.</dl>
</dl>
