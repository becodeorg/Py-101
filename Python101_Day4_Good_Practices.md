# Python 101

# D4 Bonnes pratiques, exercices supplémentaires.

## DRY

Le premier commandement de la programmation est le DRY : ne vous répétez pas (Don't Repeat Yourself en anglais).

## Commentez votre code !

## Responsabilité unique

Chaque fonction a un but unique pour une meilleure lisibilité.

## [Bonne pratiques](https://docs.python-guide.org/writing/style/)

En python comme dans les autres langages, il existe des conventions sur la façon d'écrire du code. Vous n'êtes pas obligé de toutes les respecter, mais certaines d'entre elles sont devenues unanimement utilisées. Voyons ensemble un résumé des règles les plus importantes.

## [PEP8](https://pep8.readthedocs.io/en/release-1.7.x/intro.html) en résumé !

PEP 8 (pour Python Extension Proposal) est un ensemble de règles qui permet d'homogénéiser le code et d'appliquer les bonnes pratiques.

### L'indentation dans votre code doit être de 4 caractères. Plus c'est trop, moins c'est pas assez.

### Disposition des codes : 79 caractères par ligne, pas plus.

### Importation

Les importations sont déclarées au début du script. Cela semble évident, mais il est toujours bon de s'en souvenir. Vous pouvez en ajouter dans une fonction aussi (si vous ne pouvez pas faire autrement ou pour des raisons exceptionnelles) mais après la docstring. Séparer les importations. D'abord, vous devez mettre les modules internes à Python. Ensuite, vous devez importer les bibliothèques tierces comme bs4, numpy, etc. Puis vous importez vos propres modules.
Chaque partie des modules doit être séparée par une ligne qui les espace.

### Espaces : Les opérateurs doivent être entourés d'espaces.

Good 👍

```py
name = 'Batman'
```

Bad 👎

```py
name='Batman'
```

### Conventions d'appellation

Il existe quelques conventions de nommage qui doivent être suivies afin de rendre le programme moins complexe et plus lisible. En même temps, les conventions de nommage en Python sont un peu confuses, mais voici quelques conventions qui peuvent être suivies facilement

variable, function and module : utilisation du snake_case.

Good 👍

```py
my_variable = 'Hello'
```

Bad 👎

```py
myVariable = 'Hello'
MyVariable = 'Hello'

def myFunction(element):
    pass
```

class : Utiliser le PascalCase

Good 👍

```py
class MyClass:
```

Bad 👎

```py
class my_class:
```

## Exercices supplémentaires

### 1. Hello, World!

Ecrivez un programme qui salue l'utilisateur par son nom, ou en disant `Hello, World!` si aucun nom n'est donné.

### 2. Panagramme

Déterminez si une phrase est un pangramme. Un pangramme (grec : παν γράμμα, pan gramma, "chaque lettre") est une phrase utilisant chaque lettre de l'alphabet au moins une fois.

`Dans un wagon bleu, tout en mangeant cinq kiwis frais, vous jouez du xylophone`.

### 3. Transcription de l'ARN

Ecrivez un programme qui, étant donné un brin d'ADN, retourne son complément d'ARN (par transcription ARN).

### 4. Comptage de mots

Ecrivez un programme qui, étant donné une phrase, peut compter les occurrences de chaque mot dans cette phrase.

Par exemple, pour l'entrée `olly olly in come free` :

```py
olly : 2
in : 1
come : 1
free : 1
```

### 5. Gigaseconde

Écrivez un programme qui calculera la date à laquelle une personne fêtera son anniversaire d'une gigaseconde (un milliard de secondes).

### 6. Codage de la longueur d'exécution

Mettez en œuvre le codage et le décodage de la longueur d'exécution. Run-length encoding (RLE) est une forme simple de compression de données, où les courses (éléments de données consécutifs) sont remplacées par une seule valeur de données et un seul compte.

Par exemple, nous pouvons représenter les 53 caractères originaux par 13 seulement.

```py
"WWWWWWWWWWWWBWWWWWWWWWWBBBWWWWWWWWWWWWWWWWWWWWB" -> "12WB12W3B24WB"
```

RLE permet de reconstruire parfaitement les données originales à partir des données compressées, ce qui en fait une compression de données sans perte.

```py
"AABCCCDEEEE" -> "2AB3CD4E" -> "AABCCCDEEEE"
```

### 7. Différence de carrés

Trouvez la différence entre la somme des carrés et le carré des sommes des N premiers nombres naturels.

Le carré de la somme des dix premiers nombres naturels est,

`(1 + 2 + ... + 10)**2 = 55**2 = 3025`

La somme des carrés des dix premiers nombres naturels est,

`1**2 + 2**2 + ... + 10**2 = 385`

La différence entre le carré de la somme des dix premiers nombres naturels et la somme des carrés est donc de 2640 :

`3025 - 385 = 2640`

### 8. Allergies

Ecrivez un programme qui, étant donné le score d'allergie d'une personne, peut lui dire si elle est allergique ou non à un élément donné, et sa liste complète d'allergies.

Un test d'allergie produit un score numérique unique qui contient les informations sur toutes les allergies de la personne (pour lesquelles elle a été testée). La liste des éléments (et leur valeur) qui ont été testés est la suivante :

* œufs (1)
* cacahuètes (2)
* crustacés (4)
* fraises (8)
* tomates (16)
* chocolat (32)
* pollen (64)
* chats (128)

Donc, si Tom est allergique aux cacahuètes et au chocolat, il obtient un score de 34. Maintenant, étant donné ce score de 34, votre programme devrait être capable de dire :

* si Tom est allergique à l'un des allergènes listés ci-dessus.
* Tous les allergènes auxquels Tom est allergique.

### 9. Série

Écrivez un programme qui prendra une chaîne de chiffres et vous donnera toutes les sous-chaînes contiguës de longueur `n` dans cette chaîne.

Par exemple, la chaîne "49142" a les séries de 3 chiffres suivantes :

* 491
* 914
* 142

Et la série à 4 chiffres suivante :

* 4914
* 9142

Et si vous demandez une série de 6 chiffres à partir d'une chaîne de 5 chiffres, vous méritez ce que vous obtenez.

REMARQUE : ces séries doivent uniquement occuper des positions adjacentes dans l'entrée ; les chiffres ne doivent pas nécessairement être _numériquement consécutifs_.

### 10. Simulateur de robot

Ecrivez un simulateur de robot. L'installation de test d'une usine de robots a besoin d'un programme pour vérifier les mouvements des robots. Les robots ont trois mouvements possibles :

* tourner à droite
* tourner à gauche
* avancer

Les robots sont placés sur une hypothétique grille infinie, faisant face à une direction particulière `[nord, est, sud, ouest]` à un ensemble de coordonnées `{x,y}`, par exemple `{3,8}`, les coordonnées augmentant vers le nord et l'est.

Le robot reçoit ensuite un certain nombre d'instructions, et l'installation de test vérifie alors la nouvelle position du robot et la direction dans laquelle il pointe.

La chaîne de lettres "RAALAL" signifie :

* tourner à droite
* avancer deux fois
* tourner à gauche
* avancer une fois
* tourner à gauche encore une fois

Supposons qu'un robot démarre à {7, 3} face au nord. En exécutant ce flux d'instructions, il devrait se retrouver à {9, 4} face à l'ouest.
