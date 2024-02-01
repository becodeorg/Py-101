# Python 101

# D2 Les structures de contrôle python

Une structure de contrôle est un ensemble d'instructions qui permet de contrôler l'exécution du code.

Les deux types de structures les plus communément utilisées sont les structures de contrôle conditionnelles qui permettent d'exécuter un bloc de code si une certaine condition est vérifiée et les structures de contrôle de boucle qui permettent d'exécuter un bloc de code en boucle tant qu'une condition est vérifiée.

## Les conditions Python

Selon la valeur stockée dans une variable, nous allons vouloir exécuter un bloc de code plutôt qu'un autre.

Python nous fournit les structures conditionnelles suivantes :

* La condition if (“si”) ;
* La condition if…else (“si…sinon”) ;
* La condition if…elif…else (“si…sinon si… sinon”) .

## Les opérateurs de comparaison

Pour comparer des valeurs, nous allons devoir utiliser des opérateurs de comparaison et exécuter un bloc de code ou pas.

| Opérateur | Définition                                                             |
| ---------- | ----------------------------------------------------------------------- |
| ==         | Permet de tester l'égalité en valeur et en type                      |
| !=         | Permet de tester la différence en valeur ou en type                    |
| <          | Permet de tester si une valeur est strictement inférieure à une autre |
| >          | Permet de tester si une valeur est strictement supérieure à une autre |
| <=         | Permet de tester si une valeur est inférieure ou égale à une autre   |
| >=         | Permet de tester si une valeur est supérieure ou égale à une autre   |

Lorsqu'on utilise un opérateur de comparaison, on demande à Python de tester si telle valeur est supérieure, égale, inférieur ou différente à telle autre valeur. Python va donc comparer les deux valeurs et toujours renvoyer un booléen : True si la comparaison est vérifiée ou False dans le cas contraire.

```py
4 < 5
True

4 != 5
True

4 == 4
True

4 =='4'
False
```

## La condition if en Python

Cette condition va nous permettre d'exécuter un code si (et seulement si) une certaine condition est vérifiée.

Si Python évalue l'expression passée à True, le code dans la condition if sera exécuté. Dans le cas contraire, le code dans if sera ignoré.

```py
x = int(input('Entrer une valeur pour x : '))
y = int(input('Entrer une valeur pour y : '))

if x == 5:
    print('X contient l\'entier 5')

if x > y:
    print("x contient une valeur strictement supérieur à y")
```

Au final, vous pouvez retenir que toute expression qui suit un if va être évaluée par Python et que Python renverra toujours soit True, soit False. Nous n'avons donc pas nécessairement besoin d'une comparaison explicite pour faire fonctionner un if.

Pour comprendre cela vous devez savoir qu'en dehors des comparaisons Python évaluera à True toute valeur passée après if à l'exception des valeurs suivantes qui seront évaluées à False :

* La valeur 0 (et 0.0) ;
* La valeur None ;
* Les valeurs chaine de caractères vide ””, liste vide [], dictionnaire vide {} et tuile vide ().

## La condition if… else en Python

La structure conditionnelle if…else (« si… sinon » en français) est plus complète que la condition if puisqu'elle nous permet d'exécuter un premier bloc de code si un test renvoie True ou un autre bloc de code dans le cas contraire.

```py
x = 6

if x == 5:
    print('X contient l\'entier 5')
else:
    print('X ne contient pas  l\'entier 5' )
```

## La condition if… elif… else en Python

La condition if…elif…else (« si…sinon si…sinon ») est une structure conditionnelle encore plus complète que la condition if…else qui vannons permettre cette fois-ci d'effectuer autant de tests que l'on souhaite et ainsi de prendre en compte le nombre de cas souhaité.

Il faut cependant faire attention à un point en particulier lorsqu'on utilise une structure Python if… elif… else : le cas où plusieurs elif possèdent un test évalué à True par Python.

```py
x = int(input('Entrer une valeur pour x : '))

if x == 5:
    print('X contient l\'entier 5')
elif x == 6:
    print('X contient l\'entier 6')
elif x == 6:
    print('X contient l\'entier 7')
else:
    print('x contient un autre entier' )
```

## Imbriquer des conditions

```py
x = int(input('Entrer une valeur pour x : '))
y = int(input('Entrer une valeur pour y : '))

if x == 5:
    print('x contient l\'entier 5')
    if y ==4:
        print('x contient l\'entier 5 et y contient l\'entier 4')
else:
    print('x ne contient pas l\'entier 5 et y ne contient l\'entier 4')
```

## Utiliser les opérateurs logiques avec les conditions

Les opérateurs logiques vont être principalement utilisés avec les conditions puisqu'ils vont nous permettre d'écrire plusieurs comparaisons au sein d'une même condition ou encore d'inverser la valeur logique d'un test.

| Opérateur | Définition                                                         |
| ---------- | ------------------------------------------------------------------- |
| and        | Renvoie True si toutes les deux expressions sont évaluées à True |
| or         | Renvoie True si une des comparaisons vaut True                      |
| not        | Renvoie True si la comparaison vaut False (et inversement)          |

```py
x = int(input('Entrer une valeur pour x : '))
y = int(input('Entrer une valeur pour y : '))

if x == 5 and  y ==4:
    print('x contient l\'entier 5 et y contient l\'entier 4')
else:
    print('x ne contient pas l\'entier 5 et y ne contient l\'entier 4')
```

l'opérateur logique not est très particulier puisqu'il nous permet d'inverser la valeur logique d'un test : si Python renvoie False à l'issue d'une évaluation par exemple et qu'on utilise l'opérateur not sur cette expression l'opérateur inversera la valeur renvoyée par Python et la valeur finale passée à la condition sera True.

## Opérateurs d'appartenance ou d'adhésion

L'opérateur in permet de tester si une certaine séquence de caractères ou de valeurs est présente dans une valeur d'origine et renvoie True si c'est le cas.

```py
semaine = ["lundi", "Mardi", "Mercredi",
           "Jeudi", "Vendredi", "Samedi", "Dimanche"]

if "Mardi" in semaine:
    print('Mardi est le deuxième jour de la semaine')
```

## Exercices instructions conditionelles

### 2.1 Ecrire un programme qui lit l'âge de l'utilisateur et qui affiche "Junior" pour les moins de 18 ans, "Adulte" à partir de 18 ans et "Senior" à parti de 65 ans.

### 2.2 Ecrire un programme qui lit deux nombres entiers entré au clavier et qui affiche si l'un des nombres est multiple de l'autre.

### 2.3 Ecrire un programme qui lit quatres nombres entiers  entré au clavier puis affiche le plus petit et le plus grand de ces nombres.

### 2.4 Ecrire un programme qui lit deux nombres et un caractère +,-,* ou /  entré au clavier. Suivant le caractère, le programme affiche l'opération correspondante.

### 2.5 Ecrire un programme qui vérifie si une année entré au clavier est bissextile. Ce sont les années divisibles par 4 mais pas par 100 ou les années divisible par 400.

### 2.6 Ecrire un programme qui lit une côte sur 10, et qui affiche :

* "Exellent" si la côte vaut 9 ou 10.
* "Très bien" si la côte vaut 8.
* "Bien" si la côte vaut 6 ou 7.
* "Faible" si la côte vaut 5.
* "Médiocre" si la côte vaut 3,4.
* "Mauvais" si la côte vaut 0,1,2.

# Instructions répétitives

Les boucles vont nous permettre d'exécuter plusieurs fois un bloc de code, c'est-à-dire d'exécuter un code « en boucle » tant qu'une condition donnée est vérifiée.

* La boucle while (“tant que…”)
* La boucle for (“pour…”)

Le fonctionnement général des boucles sera toujours le même : on pose une condition qui sera généralement liée à la valeur d'une variable et on exécute le code de la boucle « en boucle » tant que la condition est vérifiée.

## La boucle Python while

La boucle while va nous permettre d'exécuter un certain bloc de code « tant qu'une » condition donnée est vérifiée.

```py
x = 1

while x < 10:
    print(x)
    x += 1
```

Note : Lorsqu'on ajoute 1 à une variable, on dit qu'on l'incrémente. À l'inverse, lorsqu'on enlève 1 à la valeur d'une variable, on dit qu'on la décrémente. Les opérations d'incrémentation et de décrémentation sont très fréquentes au sein des boucles.

## La boucle Python for

La boucle Python for possède une logique et une syntaxe différente de celles des boucle for généralement rencontrées dans d'autres langages.

En effet, la boucle for Python va nous permettre d'itérer sur les éléments d'une séquence (liste, chaine de caractères, etc.) selon leur ordre dans la séquence.

La condition de sortie dans cette boucle va être implicite : on sortira de la boucle après avoir parcouru le dernier élément de la séquence.

```py
semaine = ["lundi", "Mardi", "Mercredi",
           "Jeudi", "Vendredi", "Samedi", "Dimanche"
           ]

for jour in semaine:
    print(jour)
```

## La fonction range()

On va pouvoir utiliser la fonction range() pour itérer sur une suite de nombres avec une boucle for.
Dans son utilisation la plus simple, nous allons nous contenter de passer un nombre en argument (entre les parenthèses) de range().

Si on précise deux nombres en arguments de cette fonction, le premier nombre servira de point de départ pour la génération de nombres tandis que le second servira de point d'arrivée (en étant exclus).

Finalement, on peut préciser un troisième et dernier nombre en argument de range() qui nous permet de préciser son pas, c'est-à-dire l'écart entre deux nombres générés.

```py
for n in range(10):
    print(n+1)

for n in range(10, 15):
    print(n+1)

for n in range(10,15,2):
    print(n)
```

## La fonction Enumerate ()

Ajoute un compteur à un itérable et le renvoie sous la forme d'un objet enumerate.
Cet objet enumerate peut ensuite être utilisé directement dans les boucles for ou être converti en une liste de tuples à l'aide de la méthode list ().
enumerate prend en paramètre une liste et renvoie un objet qui peut être associé à une liste contenant deux valeurs par élément : l'indice et l'élément de la liste parcourue.

```py
semaine = ["lundi", "Mardi", "Mercredi","Jeudi", "Vendredi", "Samedi", "Dimanche"]

for index, value in enumerate(semaine):
    print(index,value)
```

## Les instructions break et continue

Les instructions break et continue sont deux instructions qu'on retrouve dans de nombreux langages et qui sont souvent utilisées avec les boucles mais qui peuvent être utilisées dans d'autres contextes.

L'instruction break permet de stopper l'exécution d'une boucle lorsqu'une certaine condition est vérifiée. On l'inclura souvent dans une condition de type if.

```py
for val in "string":
    if val == "i":
        break
    print(val)

print("The end")
```

L'instruction continue permet elle d'ignorer l'itération actuelle de la boucle et de passer directement à l'itération suivante. Cette instruction va donc nous permettre d'ignorer toute ou partie de notre boucle dans certaines conditions et donc de personnaliser le comportement de notre boucle.

```py
for i in range(9):
    if i % 2 == 0:
        continue
    else:
        print(i)
```

## Exercices instructions répétitives

### 3.1 Pour afficher un carractère du code ASCII, il suffit d'utiliser la fonction chr(i), où i représente le numéro de caractère. Ecrire un programme qui affiche les 128 premiers caractères, précédés de leur numéro.

### 3.2 Ecrire un programme qui lit le nombre de ligne d'étoiles, et qui affiche un triangle rectangle en accroissant de un le nombre d'étoiles par ligne.

Exemple : nombre de lignes d'étoiles = 4

```
*
**
***
****
```

### 3.2 Même exercice que le précédent, mais avec l'affichage d'un sapin (triangle isocèle).

Exemple : nombre de lignes d'étoiles = 4

```
   *
  ***
 *****
*******
```

### 3.4 Selon une légende hindoue, l'inventeur du jeu d'échec demande au prince que l'on place un grain de riz sur la première case, 2 sur la deuxième , 4 sur la troisième, 8 sur la quatrième... et ainsi de suite jusqu'à la soixante-quatrième case. Ecrire un programme qui calcule le nombre total de grains de riz.

### 3.5 Ecrire un programme qui lit votre prénom et qui affiche à l'envers avec chaque caractère suivi d'une étoile *. Utiliser la fonction prédéfinie len().

Exemple : sangoku devient `u*k*o*g*n*a*s`

