Le modèle Linéaire et la nécessité de son dépassement
======

# Rappels sur le modèle linéaire

## Représentations
### Première écriture
Ecriture matricielle
$$
Y = Xa + \epsilon
$$

- Y contient l'ensemble des valeurs observées, c'est la variable expliquée. On peut noter que Y est une variable aléatoire parce que $\epsilon$ est une variable aléatoire.

- X est la matrice des variables explicatives de taile n lignes ( nombre d'observations) et k+1 colonnes ( avec k le nombre de variables explicatives et +1 pour modéliser le terme constant)

$$
X = \begin{bmatrix}
	1&x_{1,1}&...&x_{1,k}\\
	1&x_{2,1}&...&x_{2,k}\\
	&\ddots\\
	1&x_{n,1}&...&x_{n,k}
	\end{bmatrix} = [X_{0},X_{1},...,X_{k}]
$$

- $\epsilon$ est le terme aléatoire
$$
\epsilon = \begin{pmatrix}
\epsilon_{1}\\\
\vdots\\\
\epsilon_{n}
\end{pmatrix}
$$
- $a$ est le vecteur des coéfficients du modèle, c'est un vecteur colonne
$$
a = \begin{pmatrix}
a_{0}\\
\vdots\\
a_{k}
\end{pmatrix}
$$
### Deuxième écriture
Ecriture vectorielle
$$
\forall i\ y_{i} = x_{i}a + \epsilon_{i}  
$$
- $y_{i}$ est la valeur observée pour l'individu i
- $x_{i}$ est le vecteur des variables explicatives pour l'individu i
$$
x_{i} = (1,x_{i,1},x_{i,1},\cdots,x_{i,k} )
$$

### Troisième écriture
Sous forme de combinaison linéaire

$$
\forall i\ y_{i} = a_{0} + x_{i,1}a_{1}+ \cdots + + x_{i,k}a_{k} + \epsilon_{i}
$$

### Quatrième écriture
Sous forme d'espérance

$\forall i$ on suppose que $ E(\epsilon_{i})=0$

$$
 E(y_{i}) = a_{0} + x_{i,1}a_{1}+ \cdots + x_{i,k}a_{k}
$$

Lorsque toutes les variables explicatives sont nulles alors $E(y_{i}) = a_{0}$. Ce qui signifie que $a_{0}$ est la valeur espérée de Y dans la situation de référence. Cette affirmation est à nuancer dans le sens où il faudrait que toutes des variables explicatives soient des dummys codés. $a_{0}$ peut perdre son sens donc il est nécéssaire de ré-encoder de sorte à ce que le resultat soit plus intelligible.
## Hypothèses de la méthode des moindres carrés ordinaires(MCO)
