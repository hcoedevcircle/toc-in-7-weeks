Chapter One: Sets, Relations, and Languages
===============


## Relations and Functions

Mathematics deals with statements about objects and the realtions between them. There exists natural relation, between any two objects of a certain kind, say for 9 and 6 . It is obvious that a relation "greater than" holds true between 9 and 6 (i.e., 9 is greater than 6) but does not hold true between 6 and 9. 

But that is mathematics. The major question that arise now is, How can we express those type of relations on the language of sets? Is it possible to just say that set A "is greater than" set B ?


> Is it possible to just say that set A "is greater than" set B ?

When we think about the above question, we can do a nice litle trick. We can think of a "greater than" relation on each and every member of two set. 

For example:

Consider sets `A = {1,2,3,4} and B = {1,9,10,2}`. Now we think the relation "greater than" as a set of relation that applies to each and every element... So, `A > B ?` will be equal to a set `{no, no, no, yes}` . What did just happen here? We took a pair and applied the relation to it and got an output. We took `1` and `1`and applied the relation. 

But there is a problem here. As we discussed previously, the order is not cared. So, Technically, `A = {1,2,3,4}` and `A = {4,3,2,1}` is same. But when we use `A = {4,3,2,1}` in the above example, the output will differ, which is what we do not want. We need to be able to  distinguish the two parts of a pair in order to relate them. So, we introduced a new device for grouping objects, which we called **ordered pair**


### Ordered Pair
  
An ordered pair is a pair of two objects `a`, and `b` denoted by `(a,b)`, where `a` and `b` are the components of ordered pair.  As the definition, the order plays a vital role (unlinke sets). So, `(b,a) <> (a,b)` . And unlike sets, `(7,7)`is perfectly valid. (In sets, {7,7} used to be treated like {7}, which is not the case in ordered pair).

Any two ordered pairs `(a,b) and (c,d)` are considered equal if and only if `a = c and b = d`.

-------------------
*Note: A true fundamentalist will see ordered pair (a,b) as {a, {a,b}}.*

-------------------


### Cartesian Product

We can define Cartesian Product of two sets *A* and *B* denoted by `A × B` is the set of all ordered pairs `(a,b)` with `a ∈ A` and `b ∈ B` . 

An example.

Consider sets, `A = {2,4} and B = {b, i, n}` Now,

`A × B = {(2,b), (2,i), (2,n), (4,b), (4,i), (4,n)}`

[Note: You can write the sets in any order. for example. writing `A ={4,2}` does not affect the result] 

And `B × A  <> A × B`

### Relations

Now, we can better define relation on two sets. As in the previous example, A binary relation on two sets A and B is a subset of `A × B`. To be more clear, only the subsets of `A × B` can be realted through a binary relation. For example: `{(2,b),(4,b)}` is a binary relation on `{2,4} × {b,i,n}`. 

For a more clear example, consider a set of natural numbers `N`, now `{(i,j): i ∈ N, j ∈ N, i < j }` is a typical less than relation, which is a subset of `N × N`

### Generalizing Ordered Pairs

We introduced ordered pair as a pair of two objects `a` and `b` denoted by `(a,b)`. Generalizing the concept, let us assume, `n` as any natural number. Then if <code>a<sub>1</sub>,...,a<sub>n</sub></code> are any *n* objects (not necessarily distinct), then <code>(a<sub>1</sub>,...,a<sub>n</sub>)</code> is an ordered tuple.  

As we took the cartesian product of two sets to obtain an ordered pair. We can take n-fold Cartesian product <code>A<sub>1</sub>×...×A<sub>n</sub></code> to obtain an Ordered-n tuple <code>(a<sub>1</sub>,...,a<sub>n</sub>)</code>

#### Equality of ordered tuples
As any two ordered pairs `(a,b) and (c,d)` are considered equal if and only if `a = c and b = d`. There exists a similar relation on ordered tuples..

Consider an ordered-n tuple <code>(a<sub>1</sub>,...,a<sub>n</sub>)</code>.
And another ordered-m tuple <code>(b<sub>1</sub>,...,b<sub>m</sub>)</code>.

let us consider for each i = 1....n , a<sub>i</sub> represents the element of first (ordered-n) tuple
and for each j = 1.....m ,  b<sub>j</sub> represents the element of second (ordered-m) tuple

Now, Those two tuples are equal if and only if
- `m = n`  (which automatically means `i = j`), and
-  <code>a<sub>i</sub> = b<sub>i</code> for all `i = 1......n` 


We can also name  the tuples like:
+ Ordered 2-tuples > Ordered Pairs
+ Ordered 3-tuples > Ordered Triples
+ Ordered 4-tuples > Ordered Quadruples
+ Ordered 5-tuples > Ordered Quintuples
+ Ordered 6-tuples > Ordered Sextuples


<dl>
<dt> Sequence </dt>
<dd>
A Sequence is an ordered n-tuple for some unspecified <em>n</em> (the length of sequence). 
</dd>
</dl>


#### Relations of Ordered Tuples

As Ordered pairs had binary relations, Ordered-n tuples has n-ary relations.  

--------

### Functions

Simply said, a function is an association of each object of one kind with a unique object of another kind. It is a special kind of relation.  We can give a complex and concrete definition of functions using our knowledge of binary relation. 

<dl>
<dt> Function </dt>
<dd> A <strong>function</strong> from a set A to set B is a binary relation R on A and B with the following special property: for each element <code>a ∈ A</code>, there is <em>exactly one</em> ordered pair in R with the first component <code>a</code> </dd>
</dl>

For an example, let us consider a set Zn which is a set of Zones in Nepal and D which is a set of Districts in a specific zone. Now let us consider two relations as in:

<code>R<sub>1</sub> =  {(x,y): x ∈ D , y ∈ Zn, x is a district in zone y }</code>

<code>R<sub>2</sub> =  {(x,y): x ∈ Zn , y ∈ D, y is a district in zone x }</code>

Now, R<sub>1</sub> is a function since each district is in one and only one zone. For example, Kathmandu is only in Bagmati Zone. Some ordered pairs for R<sub>1</sub> are: `{(Kathmandu, Bagmati), (Lalitpur, Bagmati), (Banke, Bheri)}`

But R<sub>2</sub> is not be a function since  zones have more than one district. Some ordered pair for R<sub>2 is like `{(Bagmati, Kathmandu), (Bagmati, Lalitpur), (Bheri, Banke)}`

What happens in R<sub>1</sub> is you cannot have any other pair with its `x = Kathmandu` . But in R<sub>2</sub> you can have multiple ordered pairs with `x = Bagmati`. Therefore R<sub>1</sub> is a function but R<sub>2</sub> is not a function. 


#### Domain, Range, and Function Notations

Generally, the letters `f`, `g`, `h` are used for functions and we write  `f : A -> B` to indicate that a function f is a function from A to B. A is called the *domain*. If `x` is any element of domain, then we write `f(x)` for the unique element in B that the function corresponds to. `f(x)` denotes and unique object, which is called the **image of *a* under f** . The *range*  of a function  `f` is the *image* of its *domain*.

**Self Study parts: One-to-One, One-to-Many, Into, Onto, Bijection, Inverse**

**Book: Page Number 11-12 gives a clear understanding**

----------------

*****
