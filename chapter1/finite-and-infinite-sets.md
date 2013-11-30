Chapter One: Sets, Relations, and Languages
-----------

## Finite and Infinite Sets

We discuss about our intution of finite and infinite set in this topic. A question.

> What is a finite set?

We generally percieve that a finite set is a set that has finite <em>size</em>. Yes, ***size*** is the baisc property of set when we categorize it as finite or infinite. And the our definition is so obvious and natural that it hardly needs proof. 


However, there are situations where our notion of *size* leads to difficultiies. Put forward an example:

Do you consider size of set of prime numbers more than that of perfect squares? Definately we cannot get to any satisfactory conclusion, but experience in the field has shown that the only satisfactory explaination is to regard these two sets having the same size. 


### Equinumerous Set

Two sets A and B are called **equinumerous** if there is a bijection `f: A -> B`. 

With the concept of Equinumerous set, we can define a set as **finite**  set if, it is equinumerous with `{1,2,....,n}` for some natural number `n`. 

A set is **infinite** if it is not finite. For an obvious example, the set of natural numbers are infinite. However infinite set also can be equinumerous. (As in our first example of prime numbers and perfect squares)

A set is said to be **countably infinite** if it is equinumerous with N, and **countable** if it is finite, or countably infinite.  A set that is not countable is called **uncountable**

So, to show that a set `say A` is *countably infinite* we need to exhibit a bijection (or a one-to-one relation) between `A` and `N`, that is: we need only suggest a way in which `A` can be written as 

<code>A = {a<sub>0</sub>, a<sub>1</sub>, a<sub>2</sub>,...}</code>

which would mean a bijection with `N`, because, <code>f(0)=a<sub>0</sub> , f(1)=a<sub>1</sub>.....</code> (which suggests bijection)


### Union of two countably infinite sets

We can show that the union of two countably infinite sets is countably infinite. Consider three sets A, B and C, which are disjoint, and conuntably infinite. 

Let, <code>A = {a<sub>0</sub>, a<sub>1</sub>,...}, B = {b<sub>0</sub>, b<sub>1</sub>,...}, C = {c<sub>0</sub>, c<sub>1</sub>,...}`


Now their Union can be represented by: <code>A ∪ B ∪ C = {a<sub>0</sub>, b<sub>0</sub>,c<sub>0</sub>, a<sub>1</sub>,b<sub>1</sub>, c<sub>1</sub>,...}</code>

which is countably infinite. The elements of the union can also be represented as in the graph below. This technique of interweaving the enumeration of several sets is called "dovetailing"

[[Figure 1-7]]

### Going a little bit complex

We can use the similar idas to show that union of coutnably infinite set of countably infinte set is countable infinite! ( Yeah, read it again :P )

Consider that a set formed by `N X N` is countably infinte. (You must note that `N X N` is the union of `{0} X N, {1} X N, ... `) Dovtailing here must be done on a subtle way than in the figure above. So, instead of visiting one element from each set before visiting the second element of the first set (Note that we do not follow the simple way because, there are infintely many sets to visit before we could even start with the second element of the first set), we proceed as follows: 

1. In the first round, we visit one element from the first set: `(0,0)`
2. In the second round, we visit the next element from the first set: `(0,1)`, and also the first element from second set: `(1,0)`
3. In the third round, we visit the next unvisited element from the first and second set: `(0,2)` and `(1,1)`, but also the first element of third set: `(2,0)`
4. Generalzing, In the nth round, we visit the nth element from first set, (n-1)th element from second set, .... and the first element of the nth set.


This can be better understood by the figure below:

[[Figure 1-8]]


