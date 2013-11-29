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
