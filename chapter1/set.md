Chapter One: Sets, Relation and Languages
========


## Sets

Set is a collection of objects.  For example: `L = {a,b,c,d}` is a set.

Objects that make any set are its **elements** or **members** . In the above example, `a` is a member of set `L`. Similarly `c`  is also a member of set `L`. We denote these as `a ∈ L` *(read as: a 'belongs to' L)*. But since `z` is not a member or element of set `L` . We write `z` as `z ∉ L` *(read as: z 'does not belong to' L)*.

In sets, The repetition are not taken care. So set, `{orange, apple}` is same as `{orange, apple, apple}`.

Also, the order is also not taken care of. So set, `{pizza, burger}` is same as `{burger, pizza}`.

A set does not necessarily have to be a relation among their members. So, `{pizza, truck, apple, computer, star}` is also an set.

Likewise, a set can contain a set as element. For example `{apple, {toy, brick}, berry}` is a valid set.

A set that has only onle element is called singleton set. For example. `{1}`, `{apple}`  are singleton set.

> Question: Is `{{red,blue}}` a singleton set ?

A set that has no any element in it is called an empty set. For example. `{}` is an empty set. It is denoted by: `Ø`

Every set other than empty set are called non-empty


### Set Notation

There are differnt ways of representing a set. We listed all of its members upto now. We can call that `listing method`. As you already may have known. Listing method looks like this: `A = {1,2,3,4,5}` because we listed every member of the set.

Similarly, we can represent that in `set notation` method. Which looks likes this: `G = {x:x∈Z, x is greater than 2}`. *(read as: x 'such that' x belongs to Z, x is greater than 2)* Here G represents a set whose elements belongs to that of set Z *(Note that Z is generally represented as set of integers)* and whose elements are greater than 2.

### Subsets

We can create another set from a parent set, called subset.

For example,

Consider a parent set, `P = {x:x∈N}` (a set of all natural numbers)

and another set, `C = {x:x∈P, x is even number}`  (a set whose elements belong to P, and is even) 

Here set C is made by elements of set P, so C is a subset of P, denoted by `C ⊆ P`

Technically, the set itself is a subject of it. i.e, P is a subset of P.

Except P, all the other subsets of P are known as `proper subset` or `strict subset` (denoted by, `⊂`)

### Operation on Sets

There are different operations on sets, mainly `Union`, `Intersection` and `Difference`

1. Union : A Union of two sets is a set which conatins all the element of both sets. For example. Consider sets `A = {1, 2, 3}, and B={3, 4, 5}`. Now `A ∪ B` is `{1,2,3,3,4,5}` and since repetation does not mean anything on sets, we can rewrite the result as `{1,2,3,4,5}`.
2. Intersection: A Intersection of two sets gives the common elements of two sets. For example. On the previous example, we have a common element: `{3}` which is called the intersection of two sets. It is denoted by `∩`. 
3. Difference: Difference of two sets `A` and `B` is defined as set of all elements of A that are not elements of B. and denoted by `A-B`


#### Properties of Sets

Set follow Idempotency, Commutativity, Associativity, Distributivity, Absportion, and De-Morgan laws. More of this on the appendix.


### Multiple Union and Intersection

Union of set can also be defined on more than two sets. Let us consider a set, `A = {{a,b,c}, {c,d,e}, {e,f,g}}` which is a set of different Sets. Now the union of sets that are elements of set A is defined as: `∪ A = {a,b,c,d,e,f,g}`. Similar rule is followed by the intersection

### Overlapping and Disjoint sets

As the name says, if a number of sets have something in common, they are called overlapping sets, and the vice versa is disjoint.

### Power Set

The collection of all subjects of set A is called `power set`. And is denoted by 2<sup>A</sup>. For example. Consider a set, `A = {c,d}`.. Now `2`<sup>`A`</sup>` = {{c,d}, {c}, {d}, Ø}`

### Partition

A partition of a non empty set A is a subset C of 2<sup>A</sup> such that Ø is not an element of C and each element of A is in one and only one set in C. To summarize,
- each element of C is nonempty
- distinct members of C are disjoint.
- ∪ C = A



    
    
    
    
    
