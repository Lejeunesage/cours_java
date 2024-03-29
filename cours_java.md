# COURS JAVA

JAVA a été créer en 1995.
Oracle est l'netreprise qui détient JAVA aujourd'hui (2023).
Pour exécuter du code Java:

- Javac Main.java
javac => javacompiler

- Java Main => pour obtenir le resultat.

# Compilation d'un code JAVA.

La JVM (Java Virtuel Machine) est un programme qui convertit du code en bytecote, qui n'est rien d'autre code intermédiaire.

# JRE (Java Runtime Environment)

La JRE comporte une JVM. Elle comporte les complement nécessaire pour l'exécution du code. La JVM est dans la RAM. C'est un porgramme qui tourne dans la RAM.

Le code est exécuter en bytecode grâce  à la JVM qui fait appel aux librairie offertes par la JRE pour l'exécution du programme. La JDK fournit tout un autre ensemble qui prend en compte la JVM et la JRE.

# Package

Un package en JAVA est l'équivalent de l'espace de nom en PHP.


# La OOP

c'est un paradigme qui consiste à écrire du code en utilisant le concept de classe.

# Les conceptes qui découlent de la POO

- Class
- Object
- Héritage
- Polymorphisme
- Class Abstraite
- Encapsulation

# Class 

Une class est une collection d'objets ou un model d'objet

# Objet

Un objet est une instance de class

# Héritage

C'est  un terme qui s'emploi lorsqu'une class acquiert les méthodes et proproétés d'une autre class


# Encapsulation

C'est un terme qi lie le code et les données et qui sont liés à une unité.

Nom de classe : PascalCase;
Nom de méthodes : camelCase;
Nom de prooriété : cameCase;

# Polymorphisme

C'est un terme utilisé lorsqu'on parle de surcharge de méthode . Une méthode du parent peut être redefinis à l'intéérieur de la classe de l'enfant.

# Sygnature

Type de retour 
Nom de la méthode
Les paramétres
# Overloading 
 
Overloading c'est quand plusieurs méthodes peuvent avoir le même nom et des paramètres différents:
- Il est utiliser pour améliorer la lisibilité du code.
- S'éffctue dans la même classe
- Les paramètres doivent ètre diffenrents
- Ne peut ètre effectuer en changeant uniquement le type de retour de la méthode. 
- Le type de retour peut ètre identiques ou differente. Mais nous devont changer les paramètre(Type, ordre et le nombre)

il verifie: 
- le nom de paramètre ,
- le type des paramètres ,
- l'odre des paramètre ,
- le nombre de paramètre ,


public String presente();
public String presente(String fn);
public int presente(int age);

# Overiding
Consiste à redéfinir la méthode dun parent à l'intérieur d'une classe enfant.


- C'est quand une class B hérite d'une autre class A et B change une méthode de A.
- Utiliser pour une  implémentation spécifique d'une méthodes déja fournit dans la class parente, La super class.
- S'éffectue dans deux class ayant une relation d'héritage.
- Le type de retour, le nom de la méthode et les paramètre  doivent être identiques.

# Les variables static

Il y a de l'espace qui est alloué pour stocker des variables de classe.
On utilise static dans une classe pour garder en mémoire une information à chaque instanciation de l'objet.

Note: Une vartiable static ne peut être modifier durant toute la duréé de vie de l'application.

Il est déconseillé d'utiliser une instance de la classe pour affiher la variable static. Il est plutôt conseillé d'utiliser directement la classe.

# Bloc Static

C'est un bloc qui est utiliser pour initialiser les variables static.

public int foot;

static{
    foot = 2;
}

Ce bloc s'exécute bien avant le constructeur.

 Le bloc static s'appele une seule fois durant toute la vie de l'application.


# Info return Object
Tout les class java héritent toutes d'une class Object .
On écrit class Person maos pour java c'est class Person extends Object.



# Mot clé final

final {
    champs
    méthodes
    class
}

final utilisé sur une variable la rends constante.
Une constante doit être initialisé (Une valeur doit lui être affecté à  l'instant on la déclaration de la variable est faite.)

On ne peut pas faire un override d'une méthode de la superclass.

L'ajout du mot clé final ne change en rien le override.

Lorsqu'une class est précéder du mot clé final, une autre class ne peut plus hériter d'elle.

# L'Aggrégation

C'est une forme d'héritage dans laquelle une entité est passé à un autre objet.

L'aggrégation est une expression qui traduit la relation qu'une classe a une caractéristique et non une classe est.

L'aggrégation c'est une forme d'association qui traduit une relation de type "A" entre deux objets.

Ex: Une personne a une adresse.

Pour être considérer comme une aggrégation , un objet et ses membres doivent avoir la relation suivante. 
1- Le membre fait partie de l'objet.
2- Le membre peut appartenir à plus d'un objet.
3- Le membre n'a pas son existence géré par l'objet => il est indépendant.


# Super Keywords

Super{
    champs super x
    methods super . add
    constructeur
}

Super appélé comme une fonction fait appel au constructeur du parent super.x => pour utiliser la proprité x de la superclass

super.add => pour utiliser la méthode de la superclasse

super() => appel au constructeur de la super class

# Bloc d'initialisation d'instance

bloc dinstance: 

jsute des accolades

{
    l//On met ici le code d'initiation de variable
}

A la compolation , tout le code est coupé et envoyé dans le constructeur après le super.


1- Le bloc d'instance est exécutée los de l'instanciation de la classe.
2- Bloc d'instance est exécuté après le constructeur de la super class.
3- Le bloc d'instance est exécuter après le constructeur de la super class
4- Les blocs d'instance s'exécutent dans l'ordre dans lequel ils apparaîssent.

# Les modificateurs d'accès 
public
private
protected
default

Un modificateur d'accès est un mot clé qui permet de changer la visibilité oi la portée d'une méthode, d'un champs ou d'une classe.

Ces mot clé peuveunt se placer partout.

            class   package     sous-class hors package     hors package
private     v       *           *                           *
default     v       v           *                           *
protected   v       v           v                           *
pulbic      v       v           v                           v



* public : désigne l'assecibilité poirtout dans un programme. Même hors du package une classe / méthode / champs est accessible.

* protected : placcé derrière une classe / méthode / champs signifie que la classe / méthode / chaps peut etre accessible tant que l'utilisation est faite dans le même package.

* default : C'est le modificateur d'une affecté a une classe / champs / méthode qui n'est ni private ni public ni protected.

* private : Implique que ce n'est accessible qu'a l'interieur de la classe.


## Classe abstraite et Interface

# L'abstraction : 
C'est la faite de cahcher des fonctionnements de l'appplication et de montrer uniquement celles qui sont abstraites

L'abstraction en Java

 Une classe abstraite est precedé du mot abstract

 NB: On doit utiliser "abstract" pour les class abstract

 Peut avoir ou non des méthodes abstraite

 Pas d'instanciation

 Peut avoir des méthodes final

 Elle peut avoir des construceur et des m"thodes static

## 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


