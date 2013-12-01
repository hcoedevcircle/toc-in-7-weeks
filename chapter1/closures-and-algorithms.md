Chapter One: Sets, Relations, and Languages
---------------

## Closures and Algorithms


### Reflexive Transitive Closure

Consider two directed graphs R and R\* as shown in figure below. R\* contains R; also R\* is `reflexive` and `transitive` (R is neither). So R\* is called `reflexive transitive closure of R`

Formally,

If <code>R ⊆ A<sup>2</sup></code> be a directed graph defined on set A, the **reflixive transitive closure** of R is the relation:  `R* = {(a,b): a,b ∈ A and there is path from a to b in R.}` 

### Algorithms

The above defnition immediately suggests an algorithm for computing the reflexive transitive closure R* of any given binary relation R over a finite set <code>A = {a<sub>1</sub>, a<sub>3</sub>,..., a<sub>n</sub>}</code>

``` 
Initially R* = Ø
for i = 1,...,n do:
  for each i-tuple (b₁,...,bᵢ) ∈ Aⁱ do
    if (b₁,...,bᵢ) is a path in R then add (b₁,bᵢ) to R*
```

The above algorithm is pretty straightforward. When we follow these steps, there is no doubt that we will have a complete set of R* at the end. 

But the important indication that we need here is an indication of *time*. When does the algorithm terminate? This largely depend upon the inputs. It's reasonable to expect that the algorithm will take more time on larger input relations, so as said, the *time* it takes depends upon how large is input. For example, if a function is defined as `f: N -> N` 

.....
