# Python 101

# D3 Les fonctions

## Qu'est-ce qu'une fonction ?

Une fonction est un bloc de code nommé. Une fonction correspond à un ensemble d'instructions créées pour effectuer une tâche précise, regroupées ensemble et qu'on va pouvoir exécuter autant de fois qu'on le souhaite en “l'appelant” avec son nom.

Il existe deux grands “types” de fonctions en Python : les fonctions prédéfinies et les fonctions créées par l'utilisateur.

### Les fonctions prédéfinies Python

Les fonction prédéfinies sont des fonctions déjà créées et mises à notre disposition par Python. Dans ce cours, nous avons déjà utilisé des fonctions prédéfinies comme la fonction print() ou la fonction type() par exemple.

En fait, ces deux fonctions sont des fonctions complexes et qui contiennent de nombreuses lignes d'instructions leur permettant d'accomplir une tâche précise : l'affichage d'un résultat ou la détermination du type d'une valeur en l'occurence.

Cette complexité nous est cachée : nous n'avons qu'à appeler nos fonctions pour qu'elles fassent leur travail et n'avons pas à écrire la série d'instructions qu'elles contiennent à chaque fois et c'est tout l'intérêt des fonctions.

Python, dans sa version 3.7.4, met à notre disposition quasiment 70 [fonctions](https://docs.python.org/fr/3.7/library/functions.html?highlight=round#repr) prédéfinies.

### Les fonction Python définies par l'utilisateur

On va vouloir créer nos propres fonctions Python lorsque nos programmes utilisent de manière répétées une même série d'instructions : plutôt que de réécrire ces instructions à chaque fois, autant utiliser une fonction !

Pour définir une nouvelle fonction en Python, nous allons utiliser le mot clef def qui sert à introduire une définition de fonction. Ce mot clef doit être suivi du nom de la fonction, d'une paire de parenthèses au sein desquelles on pourra fournir une liste de paramètres et de : pour terminer la ligne comme ceci def ma_fonction():.

Notez que les noms de fonctions sont sensibles à la casse en Python.

```py

def bonjour(prenom):
    print('Bonjour',prenom,'!')

bonjour('Thomas')
```

### Préciser des valeurs par défaut pour les paramètres d'une fonction

```py

def bonjour(prenom, age=36, national='Belge'):
    print('Bonjour',prenom,'!','tu as',age, 'ans et tu est',national)

bonjour('Thomas')

bonjour('François', 39, 'Français')
```

### Passer un nombre arbitraire d'arguments avec *args

La syntaxe *args (remplacez “args” par ce que vous voulez) permet d'indiquer lors de la définition d'une fonction que notre fonction peut accepter un nombre variable d'arguments. Ces arguments sont intégrés dans un tuple.

```py

def somme(*args):
    s=0
    for i in args:
        s+=i
    print('Somme =',s)

somme(2,3,6)
```

En programmation, nous voudrons souvent récupérer le résultat d'une fonction afin de l'utiliser dans le reste de notre script. L'instruction return va terminer l'exécution d'une fonction, ce qui signifie qu'on placera généralement cette instruction en fin de fonction puisque le code suivant une instruction return dans une fonction ne sera jamais lu ni exécuté.

### Exemples d'utilisation de return en Python

retour une valeur

```py
def difference(a, b):
    return a - b

x = difference(8, 4)
print(x)
```

retourn plusieurs valeurs

```py
def ordre(a, b):
    if a <= b:
        return a, b
    else:
        return b, a

ordonne = ordre(50, 2)
print(ordonne)
```

### Les fonctions récursives

Les fonctions récursive sont des fonctions qui s'appelle elle même dans son exécution : c'est ce qu'on appelle la récursivité.
Exemple la factorielle de 4 par exemple est égale à 4 * 3 * 2 * 1.

```py
def factorielle(n):
    if n <=1:
        return 1
    else:
        return n * factorielle(n-1)

print(factorielle(4))
```

### Les fonctions de conversion

* La fonction str() retourne une chaine de caractères à partir d'une donnée qu'on va lui passer en argument
* La fonction int() retourne un entier à partir d'un nombre ou d'une chaine contenant un nombre qu'on va lui passer en argument
* La fonction float() retourne un nombre décimal à partir d'un nombre ou d'une chaine contenant un nombre qu'on va lui passer en argument
* La fonction complex() retourne un nombre complexe à partir d'un nombre ou d'une chaine contenant un nombre qu'on va lui passer en argument
* La fonction bool() retourne un booléen à partir d'une donnée qu'on va lui passer en argument
* La fonction list() retourne une liste à partir d'une donnée itérable (une donnée dont on peut parcourir les valeurs)
* La fonction tuple() retourne un tuple à partir d'une donnée itérable
* La fonction dict() crée un dictionnaire à partir d'un ensemble de paires clef = “valeur”
* La fonction set() retourne un ensemble (set) à partir d'une donnée itérable.

### Les fonctions mathématiques

La fonction *round()* permet d'arrondir un nombre spécifié en argument t à l'entier le plus proche avec un degré de précision (un nombre de décimales) éventuellement spécifié en deuxième argument.

Le nombre de décimales par défaut est 0, ce qui signifie que la fonction retournera l'entier le plus proche.

La fonction *sum()* permet de calculer une somme. On peut lui passer une liste de nombres en arguments par exemple. On peut également lui passer une valeur “de départ” en deuxième argument qui sera ajoutée à la somme calculée.

La fonction *max()* retourne la plus grande valeur d'une donnée itérable, c'est-à-dire d'une donnée dont on peut parcourir les différentes valeurs.

On peut lui passer autant d'arguments qu'on souhaite comparer de valeurs. Notez qu'on peut également comparer des chaines même si *max()* est peu souvent utilisée pour faire cela.

La fonction *min()*, au contraire, retourne la plus petite valeur d'une donnée itérable. Elle s'utilise exactement comme *max()*.

### Autres fonctions Python natives utiles

La fonction *len()*, tout d'abord, renvoie la longueur ou le nombre de valeurs d'une donnée de type séquence ou collection.

La fonction *input()* permet de dialoguer et d'échanger des données avec l'utilisateur.

# Les listes suite et les modules

## List Comprehensions

Les compréhensions de listes fournissent un moyen de construire des listes de manière très concise.

```py
vec = [-4, -2, 0, 2, 4]
# faire une nouvelle liste avec les valeurs doublées
[x*2 for x in vec]
[-8, -4, 0, 4, 8]
# filtrer la liste pour exclure les nombres négatifs
[x for x in vec if x >= 0]
[0, 2, 4]
# appliquer une fonction à tout les éléments
[abs(x) for x in vec]
[4, 2, 0, 2, 4]
```

d'autres exemples 👋

```py

no_integers = []

for x in semaine:
    if type(x) == int:
        lst.append(x)

print(no_integers)
```

==>

```py
no_integers = [x for x in semaine if isinstance(x, str)]  
print(no_integers)
```

## Définition et cas d'utilisation des modules Python

On appelle “module” tout fichier constitué de code Python (c'est-à-dire tout fichier avec l'extension .py) importé dans un autre fichier ou script.
Les modules permettent la séparation et donc une meilleure organisation du code.

En Python, on peut distinguer trois grandes catégories de module en les classant selon leur éditeur :

* Les modules standards qui ne font pas partie du langage en soi mais sont intégrés automatiquement par Python.
* Les modules développés par des développeurs externes qu'on va pouvoir utiliser.
* Les modules qu'on va développer nous mêmes.

## Importer un module

Pour importer un module, on utilise la syntaxe import nom-de-mon-module. Lorsque l'interprète rencontre une instruction import, il importe le module s'il est présent dans le path (le chemin de recherche). Pour rappel, le path ou chemin de recherche est une liste de répertoires dans lesquels l'interpréteur cherche avant d'importer un module.Pour être tout à fait précis, lorsqu'on importe un module, l'interpréteur Python le recherche dans différents répertoires selon l'ordre suivant :

* Le répertoire courant .
* Si le module est introuvable, Python recherche ensuite chaque répertoire listé dans la variable shell PYTHONPATH.
* Si tout échoue, Python vérifie le chemin par défaut. Sous UNIX, ce chemin par défaut est normalement /usr/local/lib/python/.

```py
from math import *
```

## Importer uniquement certains éléments d'un module

```py
from math import sqrt
```

## Créer un alias de nom pour un module

```py
import math as m
```

## Les modules Python standards

Il existe un grand nombre de [modules](https://docs.python.org/fr/3/library/index.html) préconçus et prêts à l'emploi qui sont fournis d'office avec Python. Ces modules vont étendre le langage et nous permettre de réaliser toutes sortes d'opérations notamment grâce aux fonctions qu'ils nous fournissent.

Pour importer un module Python, nous allons à nouveau tout simplement utiliser une instruction import comme si on importait l'un de nos modules.

Les modules Python standards à connaitre sont les suivants :

* Le module cgi (“Common Gateway Interface” ou “Interface de Passerelle Commune” en français) fournit des éléments permettant à des programmes Python de s'exécuter sur des serveurs HTTP
* Le module *datetime* fournit des classes pour manipuler de façon simple ou plus complexe des dates et des heures
* Le module *json* permet l'encodage et le décodage de données au format JSON
* Le module *math* fournit un ensemble de fonctions permettant de réaliser des calculs mathématiques complexes
* Le module *os* fournit une manière portable d'utiliser les fonctionnalités dépendantes du système d'exploitation
* Le module *pickle* permet de sérialiser des objets Python
* Le module *random* implémente des générateurs de nombres pseudo-aléatoires pour différentes distributions
* Le module *re* fournit des opérations sur les expressions rationnelles similaires à celles que l'on trouve dans Perl
* Le module *socket* fournit un accès à l'interface sockets qui correspond à un ensemble normalisé de fonctions de communication
* Le module *sys* fournit un accès à certaines variables système utilisées et maintenues par l'interpréteur, et à des fonctions interagissant fortement avec ce dernier
* Les modules *urllib.request* et *urllib.parse* permettent d'ouvrir, de lire et d'analyser des URLs.

## Exercices listes la suite

### 4.1 Ecrire un programme qui lit un entier n saisi au clavier et qui affiche :

* La liste des nombres de 1 à n.
* Les sous-listes de nombres impairs et pairs.

### 4.2 Ecrire un programme qui lit N nombres réels et qui les affiches d'abord dans l'ordre et ensuite dans l'ordre inverse.

### 4.3 Ecrire un programme qui lit N nombres réels et qui affiche leur minimum et maximum.

### 4.4 Ecrire un programme qui lit N nombres réels et qui affiche leur moyenne.

## Exercices Modularité

### 5.1 La distance entre deux points P1(x1,x2) et P2(x2,y2) dans le plan est définie par : d = racine carrée de ((X2-X1)²+(y2-y1)²).Ecrire une fonction qui calcule cette distance après la saisie des coordonnées.

### 5.2 Reprendre l'exercice précédent afin de calculer le périmètre d'un triangle formé par trois points non alignés.

### 5.3 Pour les anciens grecs, un nombre était trianguaire si l'on pouvait disposer ce nombre de cailloux en triangle. Tn = n(n+1)/2; Les 5 premiers nombres triangulaires sont : 1,3,6,10,15. Ecrire une fonction permettant de vérifier si un nombre saisi au clavier est triangulaire ou non.

### 5.4 Ecrire une fonction entourant d'étoiles une chaîne de caractères saisie au clavier.

```
*****************
* S A N G O K U *
*****************
```
