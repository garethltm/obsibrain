``in(auckland, northIs).``
``in(wellington, northIs).``
``samelsland(X, Z):- in(X, Y), in(Z, Y).``

> >`samelsland(X, Z):- in(X, Y), in(Z, Y).`
> >- this can be viewed as :
> >- $\forall x,z$: ($\exists y$: in(x, y) ∧ in(z, y)) → `sameIsland(x, z)`
