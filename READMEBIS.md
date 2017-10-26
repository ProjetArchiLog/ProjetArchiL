# ProjetArchiL

# ----------------------------------------------------------------------------------------------------------------------- #
# --------------------------------------------------- AUTHORS/AUTEURS --------------------------------------------------- #
# ----------------------------------------------------------------------------------------------------------------------- #

IMT ATLANTIQUE, GIPAD 2017-2018
Professeur encadrant : Hervé Grall
Étudiants : Clara TERSEN, Gabrielle Panizzoli, Denis LY
Cours : Architecture Logicielle


# ----------------------------------------------------------------------------------------------------------------------- #
# --------------------------------------------------- GOALS/OBJECTIFS --------------------------------------------------- #
# ----------------------------------------------------------------------------------------------------------------------- #

L'objectif de ce projet est de comparer les structures de données mutables à celles immutables. Nous avons considéré l'exemple des files FIFO ("First In, First Out" i.e. premier arrivé, premier sorti). Après la définition de l'interface des files, plusieurs implémentations seront données, avec des propriétés ou des usages différents : mutabilité ou non, persistance ou non.
Les critères de comparaison utilisés seront : la complexité structurelle, la complexité opérationnelle en temps et en espace.


# ----------------------------------------------------------------------------------------------------------------------- #
# -------------------------------------- NAMING CONVENTIONS/CONVENTIONS DES NOMS ---------------------------------------- #
# ----------------------------------------------------------------------------------------------------------------------- #

Les conventions utilisées sont les conventions classiques qui peuvent être retrouvées sur le l'adresse suivante : http://www.iwombat.com/standards/JavaStyleGuide.html.
Cette partie est un résumé des conventions utilisées. Le lecteur est libre de consulter la ressource citée précedemment s'il souhaite davantage de précisions.

Peu importe l'objet qui doit être nommé, le nom doit être assez explicite pour qu'il n'y ait aucune confusion possible sur le rôle joué par l'objet.

# Package/Paquet
Tous les noms des packages sont en minuscule et dans le cas d'un nom à plusieurs mots, ces mots ne sont en aucun cas séparés par un espace.
Dans notre cas : etat, fabrique, file

# Class/Classe
Le nom de la classe devrait toujours être un nom commun. Les verbes sont à proscrire. La première lettre doit toujours être en majuscule et le nom doit être gardé au singulier.
Dans notre cas : FileMutable

# Interface
Le nom de l'inteface devrait toujours un adjectif donnant une description des classes qui l'implémentent. Quand cela est possible, il faut choisir un nom se terminant par "-able" . La première lettre doit toujours être en majuscule et le nom doit être gardé au singulier.
Dans notre cas : File, FabriqueFileMutable

# Method/Méthode
Les méthodes sont en général des verbes mais des noms peuvent également être utilisés pour certains cas (accesseurs par exemple. Le nom doit être assez explicite pour comprendre ce que fait la méthode rien qu'en lisant son nom.

# Variable
Le nom des variables sont en général écrits complètement et doit refléter son but. S'il est composé de plusieurs mots, ils doivent alors tous être collés et la première lettre de chaque mot doit être en majuscule, à l'excepetion du premier mot.


# ----------------------------------------------------------------------------------------------------------------------- #
# ----------------------------------------------- COMPLEXITY/COMPLEXITÉ ------------------------------------------------- #
# ----------------------------------------------------------------------------------------------------------------------- #

Cette partie va s'attacher à évaluer la complexité des méthodes implémentées dans les différents codes du projet.

# push(T)
On ajoute un élément en queue de file
Complexité : O(1)

# getTop()
On lit la valeur de la tête de file
Complexité : O(1)

# pop()
On retire l'élement en tête de file
Complexité : O(1)

# getSize()
Retourne la taille de la file
Complexité : O(1)

# toString()
Retourne les éléments de la file
Complexité : O(n)
