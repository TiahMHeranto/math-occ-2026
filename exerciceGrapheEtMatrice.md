# Exercices Corrigés — Théorie des Graphes

---

# Exercice 1 — Degré des sommets

On considère le graphe suivant :

* Sommets :
  [
  A,B,C,D
  ]

* Arêtes :
  [
  (A,B), (A,C), (B,C), (C,D)
  ]

---

## Questions

1. Donner le degré de chaque sommet.
2. Le graphe est-il connexe ?

---

# Correction

## 1. Calcul des degrés

### Sommet A

Relié à :

* B
* C

Donc :
[
deg(A)=2
]

---

### Sommet B

Relié à :

* A
* C

Donc :
[
deg(B)=2
]

---

### Sommet C

Relié à :

* A
* B
* D

Donc :
[
deg(C)=3
]

---

### Sommet D

Relié à :

* C

Donc :
[
deg(D)=1
]

---

## Réponse finale

| Sommet | Degré |
| ------ | ----- |
| A      | 2     |
| B      | 2     |
| C      | 3     |
| D      | 1     |

---

## 2. Graphe connexe ?

Oui.

Tous les sommets peuvent être atteints.

Donc :

* le graphe est connexe.

---

# Exercice 2 — Matrice d’adjacence

Considérons le graphe :

* Sommets :
  [
  A,B,C
  ]

* Arêtes :
  [
  (A,B), (B,C)
  ]

---

## Question

Construire la matrice d’adjacence.

---

# Correction

Ordre des sommets :
[
A,B,C
]

---

## Construction

* A relié à B
* B relié à A et C
* C relié à B

---

## Matrice

[
M=
\begin{pmatrix}
0 & 1 & 0\
1 & 0 & 1\
0 & 1 & 0
\end{pmatrix}
]

---

# Exercice 3 — Graphe orienté

On a les arcs :

[
A\to B
]
[
B\to C
]
[
C\to A
]

---

## Questions

1. Donner les degrés entrants.
2. Donner les degrés sortants.

---

# Correction

## Sommet A

* entrant :
  [
  C\to A
  ]

Donc :
[
deg^{-}(A)=1
]

* sortant :
  [
  A\to B
  ]

Donc :
[
deg^{+}(A)=1
]

---

## Sommet B

* entrant :
  [
  A\to B
  ]

* sortant :
  [
  B\to C
  ]

Donc :
[
deg^{-}(B)=1
]
[
deg^{+}(B)=1
]

---

## Sommet C

* entrant :
  [
  B\to C
  ]

* sortant :
  [
  C\to A
  ]

Donc :
[
deg^{-}(C)=1
]
[
deg^{+}(C)=1
]

---

# Exercice 4 — Cycle

Considérons :

[
A-B-C-D-A
]

---

## Question

Le graphe contient-il un cycle ?

---

# Correction

Oui.

Chemin fermé :
[
A\to B\to C\to D\to A
]

Donc :

* le graphe contient un cycle.

---

---

# Exercices Corrigés — Matrices

---

# Exercice 1 — Addition de matrices

Soient :

[
A=
\begin{pmatrix}
1 & 2\
3 & 4
\end{pmatrix}
]

[
B=
\begin{pmatrix}
5 & 6\
7 & 8
\end{pmatrix}
]

---

## Question

Calculer :
[
A+B
]

---

# Correction

Addition élément par élément :

[
A+B=
\begin{pmatrix}
1+5 & 2+6\
3+7 & 4+8
\end{pmatrix}
]

---

## Résultat

[
A+B=
\begin{pmatrix}
6 & 8\
10 & 12
\end{pmatrix}
]

---

# Exercice 2 — Multiplication de matrices

Soient :

[
A=
\begin{pmatrix}
1 & 2\
3 & 4
\end{pmatrix}
]

[
B=
\begin{pmatrix}
2 & 0\
1 & 2
\end{pmatrix}
]

---

## Question

Calculer :
[
AB
]

---

# Correction

## Élément (1,1)

[
1\times2 + 2\times1=4
]

## Élément (1,2)

[
1\times0 + 2\times2=4
]

## Élément (2,1)

[
3\times2 + 4\times1=10
]

## Élément (2,2)

[
3\times0 + 4\times2=8
]

---

## Résultat

[
AB=
\begin{pmatrix}
4 & 4\
10 & 8
\end{pmatrix}
]

---

# Exercice 3 — Déterminant

Soit :

[
A=
\begin{pmatrix}
3 & 2\
1 & 4
\end{pmatrix}
]

---

## Question

Calculer :
[
det(A)
]

---

# Correction

Formule :

\det\begin{pmatrix}a&b\c&d\end{pmatrix}=ad-bc

---

Application :

[
det(A)=3\times4-2\times1
]

[
det(A)=12-2
]

[
det(A)=10
]

---

# Exercice 4 — Résolution d’un système linéaire

Résoudre :

[
\begin{cases}
x+y=5\
x-y=1
\end{cases}
]

---

# Correction

Additionnons les deux équations :

[
(x+y)+(x-y)=5+1
]

[
2x=6
]

[
x=3
]

---

Substitution :

[
3+y=5
]

[
y=2
]

---

## Solution

[
(x,y)=(3,2)
]

---

# Exercice 5 — Méthode de Gauss

Résoudre :

[
\begin{cases}
x+y=2\
2x+3y=5
\end{cases}
]

---

# Correction

Matrice augmentée :

[
\left(
\begin{array}{cc|c}
1 & 1 & 2\
2 & 3 & 5
\end{array}
\right)
]

---

## Élimination

[
L_2\leftarrow L_2-2L_1
]

---

Nouvelle matrice :

[
\left(
\begin{array}{cc|c}
1 & 1 & 2\
0 & 1 & 1
\end{array}
\right)
]

---

Donc :

[
y=1
]

Puis :

[
x+1=2
]

[
x=1
]

---

## Solution finale

[
(x,y)=(1,1)
]

---

# Exercice 6 — Rang d’une matrice

Soit :

[
A=
\begin{pmatrix}
1 & 2\
2 & 4
\end{pmatrix}
]

---

## Question

Déterminer le rang.

---

# Correction

Deuxième ligne :

[
L_2=2L_1
]

Donc :

* lignes dépendantes.

Il n’y a qu’une ligne indépendante.

---

## Résultat

[
rg(A)=1
]

---

# Exercice 7 — Valeurs propres

Soit :

[
A=
\begin{pmatrix}
2 & 0\
0 & 5
\end{pmatrix}
]

---

## Question

Trouver les valeurs propres.

---

# Correction

Équation caractéristique :

\det(A-\lambda I)=0

---

Calcul :

[
\begin{vmatrix}
2-\lambda & 0\
0 & 5-\lambda
\end{vmatrix}=0
]

---

Donc :

[
(2-\lambda)(5-\lambda)=0
]

---

## Valeurs propres

[
\lambda_1=2
]

[
\lambda_2=5
]

---

# Exercice 8 — Vecteur propre

Soit :

[
A=
\begin{pmatrix}
3 & 0\
0 & 3
\end{pmatrix}
]

---

## Question

Trouver un vecteur propre.

---

# Correction

Comme :

[
A=3I
]

Tous les vecteurs non nuls sont vecteurs propres.

Exemple :

[
v=
\begin{pmatrix}
1\
0
\end{pmatrix}
]

---

Vérification :

[
Av=
\begin{pmatrix}
3\
0
\end{pmatrix}
=============

3
\begin{pmatrix}
1\
0
\end{pmatrix}
]

Donc :

* ( v ) est un vecteur propre.
