# Python 101

## Introduction

* Presentez vous (prenom , parcours , connaissance informatique, objectif )
* Ce qui vous a amener a cette formation ( actiris , un ami , pub )
* Quels sont vos attente pour cette formation et quels sont vos "a priori"

### Installer visual studio [code](https://code.visualstudio.com/)

### Installer l'interpreteur [python](https://www.python.org/downloads/)

### Résumer de théorie du site de [Pierre Giraud](https://www.pierre-giraud.com/)

### S'entrainer à l'algorithmique sur [CodeWars](https://www.codewars.com/)

## Pourquoi apprendre python en 2022 ?

* Python est adapté aux débutants
* Python est polyvalent
* Les postes de développeurs Python sont très demandés.
* Python bénéficie d'une communauté solidaire
* Python est le langage de programmation qui connaît la plus forte croissance

C'est un language présent dans de nombreux domaines 👍

* Data Science
* Machine Learning
* Web Development ([Flask](https://flask.palletsprojects.com/en/2.1.x/), [Django](https://www.djangoproject.com/))
* Automation

# D1 les variables

## Syntaxe de base de Python : indentation, commentaires et print()

En Python, on utilise le signe # pour écrire un commentaire dans notre code.

L'indentation Python correspond au fait de créer des retraits au niveau de certaines lignes de code. Elle est utilisée par Python pour définir des blocs de code.Si on indente mal notre code Python, celui-ci ne s'exécutera tout simplement pas et Python renverra une erreur. dès qu'il y a une relation de dépendance, il faudra ajouter un retrait (une fabulation).

La fonction print() permet tout simplement d'afficher le message qu'on va lui passer entre ses parenthèses. A première vue, la fonction print() ne parait pas très utile, et c'est pourtant l'une des fonctions qu'on utilisera le plus.

La fonction print() de Python est fournie avec un paramètre appelé "end". Par défaut, la valeur de ce paramètre est '\n', c'est-à-dire le caractère de nouvelle ligne.

Vous pouvez terminer une instruction d'impression avec n'importe quel caractère ou chaîne de caractères en utilisant ce paramètre.

## Qu'est-ce qu'une variable ?

Une variable, dans le domaine de la programmation informatique, est un conteneur qui sert à stocker une valeur. Les variables possèdent deux caractéristiques fondamentales :

* Les variables ont une durée de vie limitée, ce qui signifie qu'on ne va pas pouvoir utiliser les variables pour stocker des données de manière pérenne ;
* La valeur d'une variable peut varier : les variables peuvent peuvent stocker différentes valeurs (la nouvelle valeur remplaçant l'ancienne).

Les variables Python sont automatiquement créées au moment où on leur assigne une valeur.

Le choix du nom pour nos variables est libre en Python. Il faut cependant respecter les règles usuelles suivantes :

* Le nom doit commencer par une lettre ou par un underscore ;
* Pas d'espace dans le nom d'une variable si de caractères spéciaux comme des caractères accentués ou tout autre signe;
* On ne peut pas utiliser certains mots qui possèdent déjà une signification spéciale pour le langage.

Les noms de variables en Python sont sensibles à la casse, ce qui signifie qu'on va faire une différence entre l'emploi de majuscules et de minuscules.

```py
    prenom="Thomas"
    age=23
```

## Qu'est-ce qu'un type de données ?

Python définit de nombreux types de données qu'on va pouvoir stocker dans nos variables et manipuler à loisir ensuite : nombres entiers, décimaux, complexes, chaines de caractères, booléens, listes, tuples, dictionnaires, etc.

### Les types numériques int, float et complex

* Le type int qui représente tout entier positif ou négatif ;
* Le type float qui représente les nombres décimaux et certaines expressions scientifiques comme le e pour désigner une exponentielle par exemple;
* Le type complex qui représente les nombres complexes ou nombres imaginaires et qui se sert de la lettre j pour représenter la partie imaginaire d'un nombre.

Notez que pour réaliser une division entière, on utilise l'opérateur //. On peut également utiliser l'opérateur / pour réaliser une division “classique” mais dans ce cas le résultat sera toujours considéré comme étant de type float (nombre décimal). Finalement, on utilise l'opérateur ** pour élever un nombre à la puissance.

* Toute opération arithmétique entre nombres de type float donne un résultat de type float ;
* Toute opération arithmétique entre nombres de types int et float donne un résultat de type float ;
* La division classique donne toujours un résultat de type float.

### Le type str ou chaine de caractères

Le caractère d'échappement en Python est l'antislash \.

### Le type de valeurs booléen

Le type de valeur booléen est un type qui ne contient que deux valeurs qui servent à représenter deux états. Les deux valeurs sont True (vrai) et False (faux).

**Attention en Python à bien indiquer des majuscules car dans le cas contraire Python ne reconnaitra pas ces booléens.**

### Utiliser la fonction type() pour connaitre le type d'une valeur

Pour connaitre le type de valeur stockée dans une variable, on peut utiliser la fonction Python type(). On va passer la variable à tester en argument de cette fonction

## Définition et liste des opérateurs Python

Un opérateur est un signe ou un symbole qui va nous permettre de réaliser une opération. Le signe = par exemple est en Python l'opérateur d'affectation simple : il permet d'affecter une valeur à une variable.

Python dispose de nombreux opérateurs qui peuvent être classés selon les catégories suivantes :

* Les opérateurs arithmétiques ;
* Les opérateurs d'affectation ou d'assignation ;
* Les opérateurs de chaines ;
* Les opérateurs de comparaison ;
* Les opérateurs logiques ;
* Les opérateurs d'identité ;
* Les opérateurs d'appartenance ;
* Les opérateurs binaires.

### Les opérateurs arithmétiques

| Opérateur | Nom               |
| ---------- | ----------------- |
| +          | Addition          |
| –         | Soustraction      |
| *          | Multiplication    |
| /          | Division          |
| %          | Modulo            |
| **         | Puissance         |
| //         | Division entière |

Le modulo correspond au reste d'une division Euclidienne (division entière) tandis que l'opérateur // permet d'obtenir le résultat entier d'une division

### Les opérateurs de chaines

Les opérateurs de chaines vont nous permettre de manipuler des données de type str.

Python met à notre disposition deux opérateurs de chaine : l'opérateur de concaténation + et l'opérateur de répétition *.

L'opérateur de concaténation va nous permettre de mettre bout à bout deux chaines de caractères afin d'en former une troisième, nouvelle.

L'opérateur de répétition va nous permettre de répéter une chaine un certain nombre de fois.

### Les opérateurs d'affection simple et composés Python

| Opérateur | Exemple | Equivalent à |
| ---------- | ------- | ------------- |
| =          | x = 1   | x = 1         |
| +=         | x += 1  | x = x + 1     |
| -=         | x -= 1  | x = x – 1    |
| *=         | x *= 2  | x = x * 2     |
| /=         | x /= 2  | x = x / 2     |
| %=         | x %= 2  | x = x % 2     |
| //=        | x //= 2 | x = x // 2    |
| **=        | x **= 4 | x = x ** 4    |

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

### 1.6 Ecrire un programme qui demande vos nom/prenoms, adresses et qui affiche "Bonjour *votre nom*, votre prénom et *votre adresse*"

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

Jusqu'à présent, nous n'avons stocké qu'une seule valeur à la fois dans nos variables. Les listes sont un type de données très particulier au sens où elles représentent des données composées ou combinées. Une liste est en effet par définition composée d'une suite de valeur ou d'éléments.

Pour définir une nouvelle liste en Python, on va devoir utiliser une paire de crochets [ ].

```py
prenoms= ['Michel', 'Moustafa', 'Kevin']
```

On va pouvoir stocker tous types de valeurs dans une liste.

```py
infos= ['Michel', 33, True]
```

Note : Si vous avez déjà étudié un autre langage de programmation par le passé, les liste doivent vous faire penser à ce qu'on appelle communément dans ces autres langages des tableaux. En effet, les listes Python sont très proches des tableaux qu'on peut retrouver dans de nombreux autres langages.

### Récupérer une ou plusieurs valeurs dans une liste

Les listes Python sont par défaut indexées. Cela signifie que chaque valeur d'une liste est lié à un indice qu'on va pouvoir utiliser pour récupérer cette valeur en particulier.

Les listes possèdent des indices numériques qui commencent à 0.

Pour récupérer une valeur en particulier dans une liste, on va devoir préciser le nom de la liste suivi de l'indice de cette valeur entre crochets.

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

Ce qu'on a vu jusqu'ici sur les listes s'applique également aux chaines de caractères. Les chaînes de caractères peuvent en effet également être indexées.

```py
intro = 'Salut, ça va bien ?'
>>> intro[2]
l
>>>intro[5]
,
>>> intro[13:17]
bien
```

A la différence des types de données simples comme les chaines qui sont immuables, les listes sont un type de données altérable ce qui signifie qu'on va pouvoir altérer leur structure ou modifier leur contenu en ajoutant, supprimant ou remplaçant des valeurs.

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

Écrire un programme python qui créé une liste semaine qui comprend les jours de la semaine, puis à l'aide de parcours successifs de la liste effectuer les actions suivantes :

* Afficher la liste semaine
* Afficher la valeur de semaine[4]
* Échanger les valeurs de la première et de la dernière case de cette liste
* Afficher 12 fois la valeur du dernier élément de la liste

## Tuples

Les chaines de caractères et les listes sont deux types séquentiels de données : ce sont des données qui sont organisées sous la forme de séquence de caractères ou de valeurs. Les tuples sont un autre type séquentiel de données.

Les tuples ressemblent aux listes : un tuple consiste en différentes valeurs entourées par des virgules. Notez qu'on encadre généralement les valeurs d'un tuple avec un couple de parenthèses même si cela n'est pas obligatoire.

Les tuples peuvent contenir différents types de valeurs comme des nombres, des chaines, des listes etc. et même d'autres tuples imbriqués.

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

Une fonctionnalité intéressante des tuples est le “déballage de séquence”. Un déballage de séquence correspond à une façon rapide d'affecter les différentes valeurs d'un tuple dans des variables séparées.

```py
personnage = ('Vladimir', 73, ['pêche', 'équitation'])

nom, age, sport = personnage

print(sport[0])

pêche
```

Attention ici : il faut bien faire attention à écrire les variables qui vont recevoir les valeurs du tuple avant le tuple car dans le cas contraire cela ne fonctionnerait pas.

### Exercice tuple

Écrire un programme python qui créé un tuple personnage qui comprend un non, un age et deux passions puis à l'aide de parcours successifs du tuple effectuer les actions suivantes :

* Afficher le tuple
* Afficher la valeur de passions[0]
* Échanger les valeurs de la première et de la dernière case de ce tuple

Si vous devez traiter une collection qui ne changera pas, utilisez les tuples. En revanche, si vous savez que cette collection devra être modifiée, alors utilisez les listes.

## Les Dictionnaires Python

Les dictionnaires (tableaux associatifs) sont un type de données Python.
La grande différence entre les données séquentielles (listes, tuples) et les dictionnaires se situe dans la façon d'indexer les valeurs et dans la nature de l'index. Dans le cas des séquences, les différentes valeurs dont associées à des index numériques commençant à 0. Pour les dictionnaires on va pouvoir déterminer un index "key:value".

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

Pour supprimer une paire clef : valeur d'un dictionnaire, nous allons utiliser l'instruction del.

```py

del heroes["batman"]
```

## Ensembles

Les ensemble ou sets forment un autre type de données composites Python. Un ensemble est une collection d'éléments non ordonnée, sans index et qui ne peut pas posséder l'élément dupliqué.

Une des utilisation les plus courantes des ensembles est de les utiliser pour supprimer des valeurs doublons à partir d'un autre type de données.

```py
l2 = {"Mathile", 27, "Tennis", 27, "Tennis"}
print(l2)
>>> {"Mathile", 27, "Tennis"}
```

* Les listes sont des collections d'éléments ordonnés et altérables qui peuvent contenir plusieurs fois la même valeur ;
* Les tuples sont des collections d'éléments ordonnés et immuables qui peuvent contenir plusieurs fois la même valeur ;
* Les dictionnaires sont des collection d'éléments non ordonnés mais indexés avec des clefs de notre choix et altérables qui n'acceptent pas de contenir plusieurs fois le même élément ;
* Les ensembles sont des collections d'éléments non ordonnées, non indexés et non modifiables qui n'acceptent pas de contenir plusieurs fois le même élément.

