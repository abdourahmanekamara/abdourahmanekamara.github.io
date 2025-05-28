La variable qualitative
-
Une variable qualitative est différente d'une variable quantitative. Elle est composée de modalités ou items. Par exemple, dans le cadre d'une étude commerciale on peut chercher à étudier la caractère des clients selon qu'ils soient : Très bons, Assez bons, Bons, Mauvais, Très Mauvais.

Pour analyser ce type de variable, il faut faire au préalable une transformation de celle-ci qu'on appelle **codage**. Il permet de transformer cette variable composée d'items en une variable quantitative qu'on peut analyser. 
Pour ce faire, il faut créer des variable dites "dummy" à partir des modalités et retenir une modalité de référence qui est la modalité la plus représentée. Cette technique requiert deux exigences:


Cette transformation être déclinée en deux catégories:

- Lorsqu'on ne prend pas en compte le caractère ordonné de la variable

| Modalité      | X1 | X2 | X3 | X4 |
| --------------|----|----|----|----|
| Très Mauvais  | 0  | 0  | 0  | 0  |
| Mauvais       | 1  | 0  | 0  | 0  |
| Bons          | 0  | 1  | 0  | 0  |
| Assez Bons    | 0  | 0  | 1  | 0  |
| Très Bons     | 0  | 0  | 0  | 1  |

On retient ici la modalité "Très Mauvais" comme étant la modalité de référence parce que plus représentée.
Ce type de codage est toujours valable pour les variables non ordonnées mais pas toujours la meilleure pour les variables ordonnées

- Lorsqu'on prend en compte le caractère ordonné d'une variable

| Modalité      | X1'| X2'| X3'| X4'|
| --------------|----|----|----|----|
| Très Mauvais  | 0  | 0  | 0  | 0  |
| Mauvais       | 1  | 0  | 0  | 0  |
| Bons          | 1  | 1  | 0  | 0  |
| Assez Bons    | 1  | 1  | 1  | 0  |
| Très Bons     | 1  | 1  | 1  | 1  |

On obtient les relations linéaires suivantes:

	X1' = X1 + X2 + X3 + X4
	X2' = X1 + X2 + X3
	X3' = X1 + X2 
	X4' = X1 
