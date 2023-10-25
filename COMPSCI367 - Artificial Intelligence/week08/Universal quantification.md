>	#Example 
>	`cold(wellington). `
>	`rainy(auckland).`
>	`snowy(X):- rainy(X), cold(X).`

> ``snowy(X):- rainy(X), cold(X).`` 
> - this can be viewed as:
> - $\forall x$: (rainy(x) ∧ cold(x)) → snowy(x)