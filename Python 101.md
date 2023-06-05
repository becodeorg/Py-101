# Python 101

## Introduction

* Presentez vous (prenom , parcours , connaissance informatique, objectif )

* Ce qui vous a amener a cette formation ( actiris , un ami , pub )

* Quels sont vos attente pour cette formation et quels sont vos "a priori" 


### Installer visual studio [code](https://code.visualstudio.com/)

### Installer l'interpreteur [python]( https://www.python.org/downloads/) 

### Résumer de théorie du site de [Pierre Giraud](https://www.pierre-giraud.com/) 

### S'entrainer à l'algorithmique sur [CodeWars](https://www.codewars.com/)

## Pourquoi apprendre python en 2022 ?

*  Python est adapté aux débutants
*  Python est polyvalent 
*  Les postes de développeurs Python sont très demandés. 
*  Python bénéficie d'une communauté solidaire
*  Python est le langage de programmation qui connaît la plus forte croissance

C'est un language présent dans de nombreux domaines :+1: 

* Data Science
* Machine Learning
* Web Development ([Flask](https://flask.palletsprojects.com/en/2.1.x/), [Django](https://www.djangoproject.com/))
* Automation

# D1 les variables  

## Syntaxe de base de Python : indentation, commentaires et print()

En Python, on utilise le signe # pour écrire un commentaire dans notre code.

L’indentation Python correspond au fait de créer des retraits au niveau de certaines lignes de code. Elle est utilisée par Python pour définir des blocs de code.Si on indente mal notre code Python, celui-ci ne s’exécutera tout simplement pas et Python renverra une erreur. dès qu’il y a une relation de dépendance, il faudra ajouter un retrait (une fabulation).

La fonction print() permet tout simplement d’afficher le message qu’on va lui passer entre ses parenthèses. A première vue, la fonction print() ne parait pas très utile, et c’est pourtant l’une des fonctions qu’on utilisera le plus.

La fonction print() de Python est fournie avec un paramètre appelé "end". Par défaut, la valeur de ce paramètre est '\n', c'est-à-dire le caractère de nouvelle ligne. 

Vous pouvez terminer une instruction d'impression avec n'importe quel caractère ou chaîne de caractères en utilisant ce paramètre.


## Qu’est-ce qu’une variable ?

Une variable, dans le domaine de la programmation informatique, est un conteneur qui sert à stocker une valeur. Les variables possèdent deux caractéristiques fondamentales :

* Les variables ont une durée de vie limitée, ce qui signifie qu’on ne va pas pouvoir utiliser les variables pour stocker des données de manière pérenne ;

* La valeur d’une variable peut varier : les variables peuvent peuvent stocker différentes valeurs (la nouvelle valeur remplaçant l’ancienne).

Les variables Python sont automatiquement créées au moment où on leur assigne une valeur.

Le choix du nom pour nos variables est libre en Python. Il faut cependant respecter les règles usuelles suivantes :

* Le nom doit commencer par une lettre ou par un underscore ;

* Pas d’espace dans le nom d’une variable si de caractères spéciaux comme des caractères accentués ou tout autre signe;

* On ne peut pas utiliser certains mots qui possèdent déjà une signification spéciale pour le langage.

Les noms de variables en Python sont sensibles à la casse, ce qui signifie qu’on va faire une différence entre l’emploi de majuscules et de minuscules.

```py
    prenom="Thomas"
    age=23
```

## Qu’est-ce qu’un type de données ?

Python définit de nombreux types de données qu’on va pouvoir stocker dans nos variables et manipuler à loisir ensuite : nombres entiers, décimaux, complexes, chaines de caractères, booléens, listes, tuples, dictionnaires, etc.

### Les types numériques int, float et complex

* Le type int qui représente tout entier positif ou négatif ;

* Le type float qui représente les nombres décimaux et certaines expressions scientifiques comme le e pour désigner une exponentielle par exemple;

* Le type complex qui représente les nombres complexes ou nombres imaginaires et qui se sert de la lettre j pour représenter la partie imaginaire d’un nombre.

Notez que pour réaliser une division entière, on utilise l’opérateur //. On peut également utiliser l’opérateur / pour réaliser une division “classique” mais dans ce cas le résultat sera toujours considéré comme étant de type float (nombre décimal). Finalement, on utilise l’opérateur ** pour élever un nombre à la puissance.

* Toute opération arithmétique entre nombres de type float donne un résultat de type float ;

* Toute opération arithmétique entre nombres de types int et float donne un résultat de type float ;

* La division classique donne toujours un résultat de type float.


### Le type str ou chaine de caractères

Le caractère d’échappement en Python est l’antislash \.

### Le type de valeurs booléen

Le type de valeur booléen est un type qui ne contient que deux valeurs qui servent à représenter deux états. Les deux valeurs sont True (vrai) et False (faux).

**Attention en Python à bien indiquer des majuscules car dans le cas contraire Python ne reconnaitra pas ces booléens.**

### Utiliser la fonction type() pour connaitre le type d’une valeur

Pour connaitre le type de valeur stockée dans une variable, on peut utiliser la fonction Python type(). On va passer la variable à tester en argument de cette fonction

## Définition et liste des opérateurs Python

Un opérateur est un signe ou un symbole qui va nous permettre de réaliser une opération. Le signe = par exemple est en Python l’opérateur d’affectation simple : il permet d’affecter une valeur à une variable.

Python dispose de nombreux opérateurs qui peuvent être classés selon les catégories suivantes :

* Les opérateurs arithmétiques ;
* Les opérateurs d’affectation ou d’assignation ;
* Les opérateurs de chaines ;
* Les opérateurs de comparaison ;
* Les opérateurs logiques ;
* Les opérateurs d’identité ;
* Les opérateurs d’appartenance ;
* Les opérateurs binaires.

### Les opérateurs arithmétiques


|Opérateur | Nom              | 
| -------- | --------         | 
|        + | Addition         | 
|        – |	Soustraction  |
|        * |	Multiplication|
|        / |    Division      |
|        % |    Modulo        |
|        **|	Puissance     |
|        //|  Division entière|


Le modulo correspond au reste d’une division Euclidienne (division entière) tandis que l’opérateur // permet d’obtenir le résultat entier d’une division

### Les opérateurs de chaines

Les opérateurs de chaines vont nous permettre de manipuler des données de type str.

Python met à notre disposition deux opérateurs de chaine : l’opérateur de concaténation + et l’opérateur de répétition *.

L’opérateur de concaténation va nous permettre de mettre bout à bout deux chaines de caractères afin d’en former une troisième, nouvelle.

L’opérateur de répétition va nous permettre de répéter une chaine un certain nombre de fois.

### Les opérateurs d’affection simple et composés Python


|Opérateur | Exemple  | Equivalent à|
| -------- | -------- | --------    |
| =        | x = 1    | 	x = 1   |      
| +=       | x += 1   | x = x + 1   |           
| -=       |x -= 1    | x = x – 1   |
| *=       | x *= 2   |  x = x * 2  |           
| /=       |x /= 2    | x = x / 2    |
| %=       |x %= 2    |x = x % 2    |
| //=      |x //= 2   |	x = x // 2  |
| **=      | x **= 4  |x = x ** 4    |

## Exercices Valeurs, types, variables

### 1.1 Afficher les chaînes suivantes 
* Coucou !
* L'étoile du Nord
* C'est "génial !!!"
* `^0\/0^`
* affichez la valeur d'une variable

### 1.2 Déterminer le type des expressions suivantes:

* 10-12
* 2+3.14
* '3'
* 10²
* 10.0/3.0

### 1.3 Evaluer chacune des expressions suivantes:

* 40//3
* 40/3
* 37-5-2
* 37/(5*2)
* 37/5/2
* 37%(5%2)
* 37%5%2

### 1.4 Evaluer chacune des expressions suivantes en supposant que m=24 et que n=7 : 

* m-n-8
* m%n
* m=m+1
* m+=1
* n-=2
* m+=n
* m=n=3

### 1.5 Assignez une chaine de charactere a deux variable : a = "Hello" ,b = "world" et affichez leur **concatenation**

### 1.6 Ecrire un programme qui demande vos nom/prenoms, adresses et qui affiche "Bonjour *votre nom*, votre adresse est *votre adresse*"

### 1.7 Ecrire un programme qui affiche la lettre majuscule "P" dans grille 7x7:

```py
******
*     *
*     *
******
*
*
*
```

### 1.8 Ecrire un programme qui affiche la somme, la différence, le produit, le quotient et le reste de deux entiers lus ou clavier. Testez avec les valeurs 60 et 7 !


## Listes 
 
Jusqu’à présent, nous n’avons stocké qu’une seule valeur à la fois dans nos variables. Les listes sont un type de données très particulier au sens où elles représentent des données composées ou combinées. Une liste est en effet par définition composée d’une suite de valeur ou d’éléments. 

Pour définir une nouvelle liste en Python, on va devoir utiliser une paire de crochets [ ].

```py
python=prenoms= ['Michel', 'Moustafa', 'Kevin']
```

On va pouvoir stocker tous types de valeurs dans une liste. 

```py
python=infos= ['Michel', 33, True]
```

Note : Si vous avez déjà étudié un autre langage de programmation par le passé, les liste doivent vous faire penser à ce qu’on appelle communément dans ces autres langages des tableaux. En effet, les listes Python sont très proches des tableaux qu’on peut retrouver dans de nombreux autres langages.


### Récupérer une ou plusieurs valeurs dans une liste


Les listes Python sont par défaut indexées. Cela signifie que chaque valeur d’une liste est lié à un indice qu’on va pouvoir utiliser pour récupérer cette valeur en particulier.

Les listes possèdent des indices numériques qui commencent à 0.

Pour récupérer une valeur en particulier dans une liste, on va devoir préciser le nom de la liste suivi de l’indice de cette valeur entre crochets. 

Notez que les indices négatifs sont acceptés.


```py
infos= ['Michel', 33, True]

>>> infos[0]

Michel

>>> infos[-1]

True
```

On va également pouvoir récupérer une tranche de valeurs dans une liste.

```py
infos= ['Michel', 33, True]

>>> infos[:]

['Michel', 33, True]

>>> infos[0:1]

['Michel', 33,]

>>> infos[:1]

['Michel', 33,]

```

Ce qu’on a vu jusqu’ici sur les listes s’applique également aux chaines de caractères. Les chaînes de caractères peuvent en effet également être indexées.

```py
intro = 'Salut, ça va bien ?'
>>> intro[2]
l
>>>intro[5]
,
>>> intro[13:17]
bien
```

A la différence des types de données simples comme les chaines qui sont immuables, les listes sont un type de données altérable ce qui signifie qu’on va pouvoir altérer leur structure ou modifier leur contenu en ajoutant, supprimant ou remplaçant des valeurs.

```py
prenoms= ['Michel', 'Moustafa', 'Kevin', 'Tintin', 'Sangoku']
>>>prenoms[2]
Kevin

prenoms[2] = "Jean-Michel"
>>>prenoms
['Michel', 'Moustafa', 'Jean-Michel', 'Tintin', 'Sangoku']

prenoms[:]=[]
>>>prenoms 
[]
```
on va aussi pouvoir utiliser les opérateurs de concaténation

```py
prenoms=['Michel', 'Moustafa']
ages=[27,56]

infos= prenoms +ages

>>>infos

['Michel', 'Moustafa',27,56]
```

### Exercice liste

Écrire un programme python qui créé une liste semaine qui comprend les jours de la semaine, puis à l’aide de parcours successifs de la liste effectuer les actions suivantes :

* Afficher la liste semaine
* Afficher la valeur de semaine[4]
* Échanger les valeurs de la première et de la dernière case de cette liste
* Afficher 12 fois la valeur du dernier élément de la liste

## Tuples 

Les chaines de caractères et les listes sont deux types séquentiels de données : ce sont des données qui sont organisées sous la forme de séquence de caractères ou de valeurs. Les tuples sont un autre type séquentiel de données.

Les tuples ressemblent aux listes : un tuple consiste en différentes valeurs entourées par des virgules. Notez qu’on encadre généralement les valeurs d’un tuple avec un couple de parenthèses même si cela n’est pas obligatoire.

Les tuples peuvent contenir différents types de valeurs comme des nombres, des chaines, des listes etc. et même d’autres tuples imbriqués. 

```py
t1 = 'un', 'deux', 'trois'
print(t1[1])

deux

t2 = ('un', 2, True)
print(t2[1])

2

t3 = ('un', 2, True, ['quatre', 5])
print(t3[3])

['quatre', 5]

t3 = ('un', 2, True, ('quatre', 5))
print(t3[3])

('quatre', 5)
```

Notez que dans le cas où on souhaite créer un tuple vide, on utilisera une paire de parenthèses vides.


### Le déballage de séquence


Une fonctionnalité intéressante des tuples est le “déballage de séquence”. Un déballage de séquence correspond à une façon rapide d’affecter les différentes valeurs d’un tuple dans des variables séparées.


```py
personnage = ('Vladimir', 73, ['pêche', 'équitation'])

nom, age, sport = personnage

print(sport[0])

pêche
```


Attention ici : il faut bien faire attention à écrire les variables qui vont recevoir les valeurs du tuple avant le tuple car dans le cas contraire cela ne fonctionnerait pas.


### Exercice tuple

Écrire un programme python qui créé un tuple personnage qui comprend un non, un age et deux passions puis à l’aide de parcours successifs du tuple effectuer les actions suivantes :

* Afficher le tuple
* Afficher la valeur de passions[0]
* Échanger les valeurs de la première et de la dernière case de ce tuple

Si vous devez traiter une collection qui ne changera pas, utilisez les tuples. En revanche, si vous savez que cette collection devra être modifiée, alors utilisez les listes.

## Les Dictionnaires Python

Les dictionnaires (tableaux associatifs) sont un type de données Python. 
La grande différence entre les données séquentielles (listes, tuples) et les dictionnaires se situe dans la façon d’indexer les valeurs et dans la nature de l’index. Dans le cas des séquences, les différentes valeurs dont associées à des index numériques commençant à 0. Pour les dictionnaires on va pouvoir déterminer un index "key:value".

Dans les dictionnaires, les index seront des chaînes de caractères, contrairement aux listes.

```py
personnage = {"nom":"Pierre", "age": 29, "sport" : ["Trail","Triathlon"]}
personnage["nom"]
personnage["sport"]
```
Le type dictionnaire étant un type modifiable, on peut commencer par créer un dictionnaire vide, puis le remplir petit à petit.

```py
heroes = {}
heroes["Batman"]= "Bruce Wayne"
heroes["Superman"]= " Clark Kent"

```
Pour supprimer une paire clef : valeur d’un dictionnaire, nous allons utiliser l’instruction del.

```py
del heroes["batman"]
```
## Ensembles

Les ensemble ou sets forment un autre type de données composites Python. Un ensemble est une collection d’éléments non ordonnée, sans index et qui ne peut pas posséder l’élément dupliqué.

Une des utilisation les plus courantes des ensembles est de les utiliser pour supprimer des valeurs doublons à partir d’un autre type de données.

```py
l2 = {"Mathile", 27, "Tennis", 27, "Tennis"}
print(l2)
>>> {"Mathile", 27, "Tennis"}
```

* Les listes sont des collections d’éléments ordonnés et altérables qui peuvent contenir plusieurs fois la même valeur ;
* Les tuples sont des collections d’éléments ordonnés et immuables qui peuvent contenir plusieurs fois la même valeur ;
* Les dictionnaires sont des collection d’éléments non ordonnés mais indexés avec des clefs de notre choix et altérables qui n’acceptent pas de contenir plusieurs fois le même élément ;
* Les ensembles sont des collections d’éléments non ordonnées, non indexés et non modifiables qui n’acceptent pas de contenir plusieurs fois le même élément.


# D2 Les structures de contrôle python

Une structure de contrôle est un ensemble d’instructions qui permet de contrôler l’exécution du code.

Les deux types de structures les plus communément utilisées sont les structures de contrôle conditionnelles qui permettent d’exécuter un bloc de code si une certaine condition est vérifiée et les structures de contrôle de boucle qui permettent d’exécuter un bloc de code en boucle tant qu’une condition est vérifiée.


## Les conditions Python

Selon la valeur stockée dans une variable, nous allons vouloir exécuter un bloc de code plutôt qu’un autre.

Python nous fournit les structures conditionnelles suivantes :

* La condition if (“si”) ;
* La condition if…else (“si…sinon”) ;
* La condition if…elif…else (“si…sinon si… sinon”) .

## Les opérateurs de comparaison

Pour comparer des valeurs, nous allons devoir utiliser des opérateurs de comparaison et exécuter un bloc de code ou pas.

| Opérateur |Définition                                             |
| -------- | --------                                               |
|==    | Permet de tester l’égalité en valeur et en type            |
| !=     |Permet de tester la différence en valeur ou en type             |
| <    | Permet de tester si une valeur est strictement inférieure à une autre  |
| >     | 	Permet de tester si une valeur est strictement supérieure à une autre |
| <=    |Permet de tester si une valeur est inférieure ou égale à une autre           |
|>=    |Permet de tester si une valeur est supérieure ou égale à une autre  |

Lorsqu’on utilise un opérateur de comparaison, on demande à Python de tester si telle valeur est supérieure, égale, inférieur ou différente à telle autre valeur. Python va donc comparer les deux valeurs et toujours renvoyer un booléen : True si la comparaison est vérifiée ou False dans le cas contraire.

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

Cette condition va nous permettre d’exécuter un code si (et seulement si) une certaine condition est vérifiée.

Si Python évalue l’expression passée à True, le code dans la condition if sera exécuté. Dans le cas contraire, le code dans if sera ignoré.


```py
x = int(input('Entrer une valeur pour x : '))
y = int(input('Entrer une valeur pour y : '))

if x == 5:
    print('X contient l\'entier 5')

if x > y:
    print("x contient une valeur strictement supérieur à y")
```

Au final, vous pouvez retenir que toute expression qui suit un if va être évaluée par Python et que Python renverra toujours soit True, soit False. Nous n’avons donc pas nécessairement besoin d’une comparaison explicite pour faire fonctionner un if.

Pour comprendre cela vous devez savoir qu’en dehors des comparaisons Python évaluera à True toute valeur passée après if à l’exception des valeurs suivantes qui seront évaluées à False :

* La valeur 0 (et 0.0) ;
* La valeur None ;
* Les valeurs chaine de caractères vide ””, liste vide [], dictionnaire vide {} et tuile vide ().


## La condition if… else en Python

La structure conditionnelle if…else (« si… sinon » en français) est plus complète que la condition if puisqu’elle nous permet d’exécuter un premier bloc de code si un test renvoie True ou un autre bloc de code dans le cas contraire.

```py
x = 6

if x == 5:
    print('X contient l\'entier 5')
else:
    print('X ne contient pas  l\'entier 5' )
```

## La condition if… elif… else en Python

La condition if…elif…else (« si…sinon si…sinon ») est une structure conditionnelle encore plus complète que la condition if…else qui vannons permettre cette fois-ci d’effectuer autant de tests que l’on souhaite et ainsi de prendre en compte le nombre de cas souhaité.

Il faut cependant faire attention à un point en particulier lorsqu’on utilise une structure Python if… elif… else : le cas où plusieurs elif possèdent un test évalué à True par Python.

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

Les opérateurs logiques vont être principalement utilisés avec les conditions puisqu’ils vont nous permettre d’écrire plusieurs comparaisons au sein d’une même condition ou encore d’inverser la valeur logique d’un test.


| Opérateur| 	Définition |
| -------- | -------- |
| and	   | Renvoie True si toutes les deux expressions sont évaluées à True     | 
|  or      | Renvoie True si une des comparaisons vaut True    | 
| not      | Renvoie True si la comparaison vaut False (et inversement)   | 


```py
x = int(input('Entrer une valeur pour x : '))
y = int(input('Entrer une valeur pour y : '))

if x == 5 and  y ==4:
    print('x contient l\'entier 5 et y contient l\'entier 4')
else:
    print('x ne contient pas l\'entier 5 et y ne contient l\'entier 4')
```

l’opérateur logique not est très particulier puisqu’il nous permet d’inverser la valeur logique d’un test : si Python renvoie False à l’issue d’une évaluation par exemple et qu’on utilise l’opérateur not sur cette expression l’opérateur inversera la valeur renvoyée par Python et la valeur finale passée à la condition sera True.

## Opérateurs d’appartenance ou d’adhésion

L’opérateur in permet de tester si une certaine séquence de caractères ou de valeurs est présente dans une valeur d’origine et renvoie True si c’est le cas.

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
Les boucles vont nous permettre d’exécuter plusieurs fois un bloc de code, c’est-à-dire d’exécuter un code « en boucle » tant qu’une condition donnée est vérifiée.

* La boucle while (“tant que…”) 
* La boucle for (“pour…”)

Le fonctionnement général des boucles sera toujours le même : on pose une condition qui sera généralement liée à la valeur d’une variable et on exécute le code de la boucle « en boucle » tant que la condition est vérifiée.

## La boucle Python while

La boucle while va nous permettre d’exécuter un certain bloc de code « tant qu’une » condition donnée est vérifiée.

```py
x = 1

while x < 10:
    print(x)
    x += 1
```

Note : Lorsqu’on ajoute 1 à une variable, on dit qu’on l’incrémente. À l’inverse, lorsqu’on enlève 1 à la valeur d’une variable, on dit qu’on la décrémente. Les opérations d’incrémentation et de décrémentation sont très fréquentes au sein des boucles. 

## La boucle Python for

La boucle Python for possède une logique et une syntaxe différente de celles des boucle for généralement rencontrées dans d’autres langages.

En effet, la boucle for Python va nous permettre d’itérer sur les éléments d’une séquence (liste, chaine de caractères, etc.) selon leur ordre dans la séquence.

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

Si on précise deux nombres en arguments de cette fonction, le premier nombre servira de point de départ pour la génération de nombres tandis que le second servira de point d’arrivée (en étant exclus). 

Finalement, on peut préciser un troisième et dernier nombre en argument de range() qui nous permet de préciser son pas, c’est-à-dire l’écart entre deux nombres générés.

```py
for n in range(10):
    print(n+1)

for n in range(10, 15):
    print(n+1)

for n in range(10,15,2):
    print(n)
```
## La fonction Enumerate () 
Ajoute un compteur à un itérable et le renvoie sous la forme d’un objet enumerate.
Cet objet enumerate peut ensuite être utilisé directement dans les boucles for ou être converti en une liste de tuples à l’aide de la méthode list ().
enumerate prend en paramètre une liste et renvoie un objet qui peut être associé à une liste contenant deux valeurs par élément : l’indice et l’élément de la liste parcourue.

```py
semaine = ["lundi", "Mardi", "Mercredi","Jeudi", "Vendredi", "Samedi", "Dimanche"]

for index, value in enumerate(semaine):
    print(index,value)
```
## Les instructions break et continue

Les instructions break et continue sont deux instructions qu’on retrouve dans de nombreux langages et qui sont souvent utilisées avec les boucles mais qui peuvent être utilisées dans d’autres contextes.

L’instruction break permet de stopper l’exécution d’une boucle lorsqu’une certaine condition est vérifiée. On l’inclura souvent dans une condition de type if.

```py    
for val in "string":
    if val == "i":
        break
    print(val)

print("The end")
```

L’instruction continue permet elle d’ignorer l’itération actuelle de la boucle et de passer directement à l’itération suivante. Cette instruction va donc nous permettre d’ignorer toute ou partie de notre boucle dans certaines conditions et donc de personnaliser le comportement de notre boucle.

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


# D3 Les fonctions

## Qu’est-ce qu’une fonction ?

Une fonction est un bloc de code nommé. Une fonction correspond à un ensemble d’instructions créées pour effectuer une tâche précise, regroupées ensemble et qu’on va pouvoir exécuter autant de fois qu’on le souhaite en “l’appelant” avec son nom.

Il existe deux grands “types” de fonctions en Python : les fonctions prédéfinies et les fonctions créées par l’utilisateur.

### Les fonctions prédéfinies Python

Les fonction prédéfinies sont des fonctions déjà créées et mises à notre disposition par Python. Dans ce cours, nous avons déjà utilisé des fonctions prédéfinies comme la fonction print() ou la fonction type() par exemple.

En fait, ces deux fonctions sont des fonctions complexes et qui contiennent de nombreuses lignes d’instructions leur permettant d’accomplir une tâche précise : l’affichage d’un résultat ou la détermination du type d’une valeur en l’occurence.

Cette complexité nous est cachée : nous n’avons qu’à appeler nos fonctions pour qu’elles fassent leur travail et n’avons pas à écrire la série d’instructions qu’elles contiennent à chaque fois et c’est tout l’intérêt des fonctions.

Python, dans sa version 3.7.4, met à notre disposition quasiment 70 [fonctions](https://docs.python.org/fr/3.7/library/functions.html?highlight=round#repr) prédéfinies.

### Les fonction Python définies par l’utilisateur

On va vouloir créer nos propres fonctions Python lorsque nos programmes utilisent de manière répétées une même série d’instructions : plutôt que de réécrire ces instructions à chaque fois, autant utiliser une fonction !

Pour définir une nouvelle fonction en Python, nous allons utiliser le mot clef def qui sert à introduire une définition de fonction. Ce mot clef doit être suivi du nom de la fonction, d’une paire de parenthèses au sein desquelles on pourra fournir une liste de paramètres et de : pour terminer la ligne comme ceci def ma_fonction():.

Notez que les noms de fonctions sont sensibles à la casse en Python.

```py
python=def bonjour(prenom):
    print('Bonjour',prenom,'!')

bonjour('Thomas')
```
### Préciser des valeurs par défaut pour les paramètres d’une fonction

```py
python=def bonjour(prenom, age=36, national='Belge'):
    print('Bonjour',prenom,'!','tu as',age, 'ans et tu est',national)

bonjour('Thomas')

bonjour('François', 39, 'Français')
```
### Passer un nombre arbitraire d’arguments avec *args 

La syntaxe *args (remplacez “args” par ce que vous voulez) permet d’indiquer lors de la définition d’une fonction que notre fonction peut accepter un nombre variable d’arguments. Ces arguments sont intégrés dans un tuple.

```py
python=def somme(*args):
    s=0
    for i in args:
        s+=i
    print('Somme =',s)

somme(2,3,6)
```

En programmation, nous voudrons souvent récupérer le résultat d’une fonction afin de l’utiliser dans le reste de notre script. L’instruction return va terminer l’exécution d’une fonction, ce qui signifie qu’on placera généralement cette instruction en fin de fonction puisque le code suivant une instruction return dans une fonction ne sera jamais lu ni exécuté.

### Exemples d’utilisation de return en Python

retour une valeur

```py
python=def difference(a, b):
    return a - b

x = difference(8, 4)
print(x)
```
retourn plusieurs valeurs

```py
python=def ordre(a, b):
    if a <= b:
        return a, b
    else:
        return b, a

ordonne = ordre(50, 2)
print(ordonne)
```

### Les fonctions récursives

Les fonctions récursive sont des fonctions qui s'appelle elle même dans son exécution : c’est ce qu’on appelle la récursivité. 
Exemple la factorielle de 4 par exemple est égale à 4 * 3 * 2 * 1.

```py
python=def factorielle(n):
    if n <=1:
        return 1
    else:
        return n * factorielle(n-1)

print(factorielle(4))
```

### Les fonctions de conversion

* La fonction str() retourne une chaine de caractères à partir d’une donnée qu’on va lui passer en argument 
* La fonction int() retourne un entier à partir d’un nombre ou d’une chaine contenant un nombre qu’on va lui passer en argument 
* La fonction float() retourne un nombre décimal à partir d’un nombre ou d’une chaine contenant un nombre qu’on va lui passer en argument 
* La fonction complex() retourne un nombre complexe à partir d’un nombre ou d’une chaine contenant un nombre qu’on va lui passer en argument 
* La fonction bool() retourne un booléen à partir d’une donnée qu’on va lui passer en argument 
* La fonction list() retourne une liste à partir d’une donnée itérable (une donnée dont on peut parcourir les valeurs) 
* La fonction tuple() retourne un tuple à partir d’une donnée itérable 
* La fonction dict() crée un dictionnaire à partir d’un ensemble de paires clef = “valeur” 
* La fonction set() retourne un ensemble (set) à partir d’une donnée itérable.

### Les fonctions mathématiques

La fonction *round()* permet d’arrondir un nombre spécifié en argument t à l’entier le plus proche avec un degré de précision (un nombre de décimales) éventuellement spécifié en deuxième argument.

Le nombre de décimales par défaut est 0, ce qui signifie que la fonction retournera l’entier le plus proche.

La fonction *sum()* permet de calculer une somme. On peut lui passer une liste de nombres en arguments par exemple. On peut également lui passer une valeur “de départ” en deuxième argument qui sera ajoutée à la somme calculée.

La fonction *max()* retourne la plus grande valeur d’une donnée itérable, c’est-à-dire d’une donnée dont on peut parcourir les différentes valeurs.

On peut lui passer autant d’arguments qu’on souhaite comparer de valeurs. Notez qu’on peut également comparer des chaines même si *max()* est peu souvent utilisée pour faire cela.

La fonction *min()*, au contraire, retourne la plus petite valeur d’une donnée itérable. Elle s’utilise exactement comme *max()*.

### Autres fonctions Python natives utiles

La fonction *len()*, tout d’abord, renvoie la longueur ou le nombre de valeurs d’une donnée de type séquence ou collection.

La fonction *input()* permet de dialoguer et d’échanger des données avec l’utilisateur.

# Les listes suite et les modules

## List Comprehensions

Les compréhensions de listes fournissent un moyen de construire des listes de manière très concise.

```py
python=vec = [-4, -2, 0, 2, 4]
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

d'autres exemples :wave: 

```py
python=no_integers = []

for x in semaine:
    if type(x) == int:
        lst.append(x)

print(no_integers)
```

==>

```py
python=no_integers = [x for x in semaine if isinstance(x, str)]  
print(no_integers)
```


## Définition et cas d’utilisation des modules Python

On appelle “module” tout fichier constitué de code Python (c’est-à-dire tout fichier avec l’extension .py) importé dans un autre fichier ou script.
Les modules permettent la séparation et donc une meilleure organisation du code.

En Python, on peut distinguer trois grandes catégories de module en les classant selon leur éditeur :

* Les modules standards qui ne font pas partie du langage en soi mais sont intégrés automatiquement par Python.
* Les modules développés par des développeurs externes qu’on va pouvoir utiliser.
* Les modules qu’on va développer nous mêmes.

## Importer un module

Pour importer un module, on utilise la syntaxe import nom-de-mon-module. Lorsque l’interprète rencontre une instruction import, il importe le module s’il est présent dans le path (le chemin de recherche). Pour rappel, le path ou chemin de recherche est une liste de répertoires dans lesquels l’interpréteur cherche avant d’importer un module.Pour être tout à fait précis, lorsqu’on importe un module, l’interpréteur Python le recherche dans différents répertoires selon l’ordre suivant :

* Le répertoire courant .
* Si le module est introuvable, Python recherche ensuite chaque répertoire listé dans la variable shell PYTHONPATH.
* Si tout échoue, Python vérifie le chemin par défaut. Sous UNIX, ce chemin par défaut est normalement /usr/local/lib/python/.

```py
from math import *
```

## Importer uniquement certains éléments d’un module

```py
from math import sqrt
```

## Créer un alias de nom pour un module

```py
import math as m
```

## Les modules Python standards

Il existe un grand nombre de [modules](https://docs.python.org/fr/3/library/index.html) préconçus et prêts à l’emploi qui sont fournis d’office avec Python. Ces modules vont étendre le langage et nous permettre de réaliser toutes sortes d’opérations notamment grâce aux fonctions qu’ils nous fournissent.

Pour importer un module Python, nous allons à nouveau tout simplement utiliser une instruction import comme si on importait l’un de nos modules.

Les modules Python standards à connaitre sont les suivants :

* Le module cgi (“Common Gateway Interface” ou “Interface de Passerelle Commune” en français) fournit des éléments permettant à des programmes Python de s’exécuter sur des serveurs HTTP 
* Le module *datetime* fournit des classes pour manipuler de façon simple ou plus complexe des dates et des heures 
* Le module *json* permet l’encodage et le décodage de données au format JSON 
* Le module *math* fournit un ensemble de fonctions permettant de réaliser des calculs mathématiques complexes 
* Le module *os* fournit une manière portable d’utiliser les fonctionnalités dépendantes du système d’exploitation 
* Le module *pickle* permet de sérialiser des objets Python 
* Le module *random* implémente des générateurs de nombres pseudo-aléatoires pour différentes distributions 
* Le module *re* fournit des opérations sur les expressions rationnelles similaires à celles que l’on trouve dans Perl 
* Le module *socket* fournit un accès à l’interface sockets qui correspond à un ensemble normalisé de fonctions de communication 
* Le module *sys* fournit un accès à certaines variables système utilisées et maintenues par l’interpréteur, et à des fonctions interagissant fortement avec ce dernier 
* Les modules *urllib.request* et *urllib.parse* permettent d’ouvrir, de lire et d’analyser des URLs.


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

# D4 Bonnes pratiques, exercices supplémentaires. 

## DRY

Le premier commandement de la programmation est le DRY : ne vous répétez pas (Don’t Repeat Yourself en anglais).

## Commentez votre code ! 

## Responsabilité unique 

Chaque fonction a un but unique pour une meilleure lisibilité.

## [Bonne pratiques](https://docs.python-guide.org/writing/style/) 

En python comme dans les autres langages, il existe des conventions sur la façon d'écrire du code. Vous n'êtes pas obligé de toutes les respecter, mais certaines d'entre elles sont devenues unanimement utilisées. Voyons ensemble un résumé des règles les plus importantes.

## [PEP8](https://pep8.readthedocs.io/en/release-1.7.x/intro.html) en résumé !
  
PEP 8 (pour Python Extension Proposal) est un ensemble de règles qui permet d'homogénéiser le code et d'appliquer les bonnes pratiques.

### L'indentation dans votre code doit être de 4 caractères. Plus c'est trop, moins c'est pas assez. 

### Disposition des codes : 79 caractères par ligne, pas plus.
 
###  Importation

Les importations sont déclarées au début du script. Cela semble évident, mais il est toujours bon de s'en souvenir. Vous pouvez en ajouter dans une fonction aussi (si vous ne pouvez pas faire autrement ou pour des raisons exceptionnelles) mais après la docstring. Séparer les importations. D'abord, vous devez mettre les modules internes à Python. Ensuite, vous devez importer les bibliothèques tierces comme bs4, numpy, etc. Puis vous importez vos propres modules. 
Chaque partie des modules doit être séparée par une ligne qui les espace.

### Espaces : Les opérateurs doivent être entourés d'espaces.

Good :+1: 
```py
name = 'Batman'
```
Bad :-1: 
```py
name='Batman'
```
### Conventions d'appellation

Il existe quelques conventions de nommage qui doivent être suivies afin de rendre le programme moins complexe et plus lisible. En même temps, les conventions de nommage en Python sont un peu confuses, mais voici quelques conventions qui peuvent être suivies facilement

variable, function and module : utilisation du snake_case.

Good :+1: 

```py
my_variable = 'Hello'
```
Bad :-1:

```py
myVariable = 'Hello'
MyVariable = 'Hello'

def myFunction(element):
    pass
```

class : Utiliser le PascalCase

Good :+1: 

```py
class MyClass:
```
Bad :-1: 

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

# D5 - Fun projects 

### Installez les packages avec Pip

Pip est un gestionnaire de packages Python.

```shell
pip install <package>
```
Afficher les packets déjà télécharger 

```shell
pip freeze
```
## Web scraping avec Requests et Beautifull_soup 

ETL signifie extraction, transformation et chargement (Extract, Transform, Load en anglais). C’est une procédure qui "permettant d'effectuer des synchronisations massives d'information d'une source de données (le plus souvent une base de données) vers une autre" (source [Wikipédia](https://fr.wikipedia.org/wiki/Extract-transform-load)).

```shell
pip install requests
```
```shell
pip install beautifulsoup4
```

```py

# On importe requests
import requests
# On importe beautifulsoup
from bs4 import BeautifulSoup as bs

# On défini l'url du site
url = "https://www.gov.uk/search/news-and-communications"
# On utilise la fonction get() du package requests
page = requests.get(url)
soup = bs(page.content, 'html.parser')
# On utilise beautifulsoup pour aller chercher les balises a avec la classe "gem-c-document-list__item-title"
titres_bs = soup.find_all("a", class_="gem-c-document-list__item-title")
# On utilise beautifulsoup pour aller chercher les balises a avec la classe "gem-c-document-list__item-title"
descriptions_bs = soup.find_all(
    "p", class_="gem-c-document-list__item-description")
# On utilise beautifulsoup pour aller chercher les balises p avec la classe "gem-c-document-list__item-description"

titres = []
# On initie des listes vides

descriptions = []
# On initie des listes vides

for titre in titres_bs:
    # print(titre.string)
    titres.append(titre.string)

# On boucle et on push dans notre liste

for index, description in enumerate(descriptions_bs):
    descriptions.append((index, description.string))

# On boucle et on push dans notre liste

print(titres[0],':', descriptions[0][1], end='\r')

```

## Détection de visage avec openCV et DeepFace

On va utiliser les fichiers .xml fournit par open CV pour détecter des visages dans des images. 
```shell
pip install opencv-python
```
```shell
pip install pathlib2
```

```py

from deepface import DeepFace
import pathlib
import cv2

cascade_path = pathlib.Path(cv2.__file__).parent.absolute(
)/"data/haarcascade_frontalface_default.xml"  # Path du modèle dans l'objet

# Classifier
clf = cv2.CascadeClassifier(str(cascade_path))

# camera= cv2.VideoCapture("people.mp4") - On peut aussi utiliser le programe sur une vidéo
camera = cv2.VideoCapture(0)

# Boucle infinie de génération des frames
while True:
    _, frame = camera.read()
    # Conversion des images en niveau de gris
    gray = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)

    faces = clf.detectMultiScale(
        gray,
        scaleFactor=1.1,
        minNeighbors=5,
        minSize=(30, 30),
        flags=cv2.CASCADE_SCALE_IMAGE
    )

    for (x, y, width, height) in faces:
        cv2.rectangle(frame, (x, y), (x+width, y+height), (255, 255, 3), 2)
        try:
            analyze = DeepFace.analyze(
                frame, actions=['age', 'gender', 'race', 'emotion'])
            print(analyze)
        except:
            print("no face")

    cv2.imshow("Faces", frame)

    if cv2.waitKey(1) == ord("q"):
        break

camera.release()
cv2.destroyAllWindows()
```


