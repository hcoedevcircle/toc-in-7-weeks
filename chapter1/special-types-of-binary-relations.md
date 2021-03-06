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
<dt>Equivalence Relation and Equivalence class</dt>
<dd>A relation that is reflexive, symmetric, and transitive is called and <strong>equivalence relation</strong>. The equivalence relation are represented by undirected graph which consits of a number of <em>clusters</em>; and within each cluster, each pair of nodes is connected by a line. Those <em>Clusters</em> are called <strong>equivalence classes</strong>. Normally equivalence class is denoted by <code>[a]</code>. Equivalence class can also be defined as <code>[a] = {b:(a,b) ∈ R}</code>, or <code>[a]={b: (b,a) ∈ R</code> (since R is symmetric). As shown in the figure below, there are three equivalence classes, one with four elements, one with three, and one with a single element.</dd>
</dl>


[[Figure 1-6]]


<strong>Some problems and theorems on equivalence relation is to be done from the book</strong>


<dl>
<dt>Partial Order</dt>
<dd>
A relation that is <em>reflexive</em>, <em>anti-symmetric</em>, and <em>transitive</em> is acalled a <strong>partial order</strong>
</dd>
</dl>

<dl>
<dt>Total Order</dt>
<dd>
A partial order <code>R ⊆ A × A</code> is a <strong>total order</strong> if, for all <code>a, b ∈ R </code>, either <code>(a,b) ∈ R</code> or <code>(b,a) ∈ R</code>
</dd>
</dl>

<dl>
<dt>Path</dt>
<dd>
A path in a binary relation R is a sequence <code>(a<sub>1</sub>.....a<sub>n</sub>)</code> for some <code> n >= 1 </code> such that <code>(a<sub>i</sub>, a<sub>i+1</sub>) ∈ R for i = 1.....n-1</code>; this path is said to be from a<sub>1</sub> to a<sub>n></sub>. The <strong>length</strong> of that path is n. The path is called <strong>cycle</strong> if all the a<sub>i</sub>'s are distinct and <code>(a<sub>n</sub>, a<sub>1</sub>) ∈ R</code>
</dd>
</dl>
