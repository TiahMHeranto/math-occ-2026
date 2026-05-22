# Cours Complet — Outils Mathématiques

## 1. Ensembles

### Définition

Un ensemble est une collection d’éléments.

Exemple :

* ( A = {1,2,3} )
* ( B = {a,b,c} )

---

## 1.1 Notations importantes

| Symbole           | Signification          |
| ----------------- | ---------------------- |
| ( x \in A )       | x appartient à A       |
| ( x \notin A )    | x n’appartient pas à A |
| ( A \subset B )   | A est inclus dans B    |
| ( A \cup B )      | Union                  |
| ( A \cap B )      | Intersection           |
| ( A \setminus B ) | Différence             |
| ( \emptyset )     | Ensemble vide          |

---

## 1.2 Propriétés des ensembles

### Commutativité

[
A \cup B = B \cup A
]
[
A \cap B = B \cap A
]

### Associativité

[
(A \cup B)\cup C = A \cup (B \cup C)
]

### Distributivité

[
A \cap (B \cup C) = (A \cap B)\cup(A \cap C)
]

---

# 1.3 Applications (Fonctions)

Une application associe chaque élément d’un ensemble à un unique élément d’un autre ensemble.

[
f : A \to B
]

Exemple :
[
f(x)=2x+1
]

---

## Domaine, Codomaine, Image

* Domaine : ensemble de départ
* Codomaine : ensemble d’arrivée
* Image :
  [
  Im(f)={f(x)}
  ]

---

## Types d’applications

### Injection

Chaque élément a une image différente.

[
f(x_1)=f(x_2)\Rightarrow x_1=x_2
]

### Surjection

Tous les éléments du codomaine sont atteints.

### Bijection

Injection + Surjection.

---

# 1.4 Composition d’applications

Si :
[
f:A\to B
]
[
g:B\to C
]

Alors :
[
(g\circ f)(x)=g(f(x))
]

Exemple :
[
f(x)=2x
]
[
g(x)=x+3
]

Alors :
[
(g\circ f)(x)=2x+3
]

---

# 2. Théorie des nombres

## 2.1 Nombre premier

Un nombre premier possède exactement deux diviseurs :

* 1
* lui-même

Exemples :
[
2,3,5,7,11
]

---

## Test de primalité

Pour tester si ( n ) est premier :

* vérifier les diviseurs jusqu’à :
  [
  \sqrt{n}
  ]

---

# 2.2 PGCD

Le Plus Grand Commun Diviseur.

Exemple :
[
PGCD(18,24)=6
]

---

## Algorithme d’Euclide

[
a=bq+r
]

Puis :
[
PGCD(a,b)=PGCD(b,r)
]

Exemple :
[
24=18\times1+6
]
[
18=6\times3+0
]

Donc :
[
PGCD(24,18)=6
]

---

# 2.3 PPCM

Plus Petit Commun Multiple.

Relation importante :
[
PPCM(a,b)\times PGCD(a,b)=a\times b
]

Exemple :
[
PPCM(12,18)=36
]

---

# 3. Relations

Une relation relie les éléments d’un ensemble.

Exemple :
[
xRy \iff x<y
]

---

# 3.1 Relation d’équivalence

Une relation d’équivalence doit être :

### Réflexive

[
xRx
]

### Symétrique

[
xRy \Rightarrow yRx
]

### Transitive

[
xRy \text{ et } yRz \Rightarrow xRz
]

---

## Exemple

[
xRy \iff x-y \text{ est pair}
]

---

# 3.2 Relation d’ordre

Une relation d’ordre doit être :

### Réflexive

### Antisymétrique

[
xRy \text{ et } yRx \Rightarrow x=y
]

### Transitive

Exemple :
[
\le
]

---

# 3.3 Inclusion

[
A\subseteq B
]

Signifie :
Tous les éléments de A sont dans B.

---

# 4. Théorie des graphes

Un graphe est composé :

* de sommets
* d’arêtes

---

## Types de graphes

### Graphe orienté

Les arêtes ont une direction.

### Graphe non orienté

Pas de direction.

---

# 4.1 Degré d’un sommet

Nombre d’arêtes reliées au sommet.

---

# 4.2 Chaîne et cycle

### Chaîne

Suite de sommets reliés.

### Cycle

Chaîne fermée.

---

# 4.3 Matrice d’adjacence

Pour représenter un graphe.

Si un sommet est relié :
[
a_{ij}=1
]

Sinon :
[
a_{ij}=0
]

---

# 4.4 Graphe connexe

Tous les sommets sont accessibles.

---

# 5. Matrices

## Définition

Tableau de nombres.

[
A=
\begin{pmatrix}
1 & 2\
3 & 4
\end{pmatrix}
]

---

# 5.1 Opérations sur les matrices

## Addition

Même dimension.

## Multiplication

[
AB
]

Le nombre de colonnes de A doit être égal au nombre de lignes de B.

---

# 5.2 Déterminant

Seulement pour matrices carrées.

Pour :
[
A=
\begin{pmatrix}
a & b\
c & d
\end{pmatrix}
]

[
det(A)=ad-bc
]

---

## Importance du déterminant

Si :
[
det(A)\neq0
]

Alors :

* matrice inversible
* système possède une solution unique

---

# 5.3 Vecteur et Scalaire

## Scalaire

Nombre simple :
[
5,\ 3.2
]

## Vecteur

Liste ordonnée :
[
\begin{pmatrix}
1\
2
\end{pmatrix}
]

---

## Différence

| Scalaire         | Vecteur               |
| ---------------- | --------------------- |
| Une valeur       | Plusieurs composantes |
| Taille seulement | Taille + direction    |

---

# 5.4 Système linéaire

Exemple :
[
\begin{cases}
2x+y=5\
x-y=1
\end{cases}
]

---

## Méthodes de résolution

### Substitution

### Élimination de Gauss

---

# 5.5 Méthode de Gauss

Transformer la matrice en forme triangulaire.

Exemple :

[
\begin{pmatrix}
1 & 2\
2 & 4
\end{pmatrix}
]

La deuxième ligne devient :
[
L_2-2L_1
]

---

# 5.6 Rang d’une matrice

Nombre de lignes indépendantes.

Noté :
[
rg(A)
]

---

## Importance

Le rang permet de savoir :

* nombre de solutions
* indépendance linéaire

---

# 5.7 Valeur propre

Pour une matrice ( A ).

Un scalaire ( \lambda ) est valeur propre si :

[
A\vec v=\lambda \vec v
]

avec :

* ( \lambda ) : valeur propre
* ( \vec v ) : vecteur propre

---

# 5.8 Vecteur propre

Vecteur qui garde sa direction après transformation.

---

## Calcul des valeurs propres

On résout :

[
det(A-\lambda I)=0
]

où :
[
I=
\begin{pmatrix}
1&0\
0&1
\end{pmatrix}
]

---

## Exemple

[
A=
\begin{pmatrix}
2&0\
0&3
\end{pmatrix}
]

Valeurs propres :
[
\lambda_1=2
]
[
\lambda_2=3
]

---

# 5.9 Décomposition matricielle

Décomposer une matrice en plusieurs matrices simples.

---

## Décomposition LU

[
A=LU
]

* L : triangulaire inférieure
* U : triangulaire supérieure

---

## Diagonalisation

[
A=PDP^{-1}
]

* D : diagonale
* P : matrice des vecteurs propres

---

# 5.10 Distribution gaussienne en dimension 2

Distribution de probabilité sur deux variables.

---

## Forme générale

Variables :
[
X=(X_1,X_2)
]

---

## Paramètres

### Moyenne

[
\mu=
\begin{pmatrix}
\mu_1\
\mu_2
\end{pmatrix}
]

### Matrice de covariance

[
\Sigma
]

---

## Utilisation

Très utilisée en :

* IA
* Machine Learning
* Statistiques
* Vision par ordinateur

---

# Résumé Ultra Important pour l’Examen

## À retenir absolument

### Ensembles

* union
* intersection
* inclusion
* application
* composition

### Théorie des nombres

* nombre premier
* PGCD : Euclide
* PPCM

### Relations

* équivalence
* ordre
* inclusion

### Graphes

* sommet
* arête
* matrice d’adjacence
* degré
* cycle

### Matrices

* déterminant
* rang
* Gauss
* systèmes linéaires
* valeurs propres
* vecteurs propres
* diagonalisation

---

# Formules essentielles

## Déterminant 2×2

\det\begin{pmatrix}a&b\c&d\end{pmatrix}=ad-bc

## Relation PGCD/PPCM

PPCM(a,b)\times PGCD(a,b)=a\times b

## Valeur propre

A\vec v=\lambda \vec v

## Équation caractéristique

\det(A-\lambda I)=0
