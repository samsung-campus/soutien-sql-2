# Soutien SQL - Jour 02 #

Ce second jour de soutien servira à compléter les bases ré-acquises au cours du jour #1.

Si l'on résume, nous avons pour le moment re-travaillé le SELECT de base, le AS pour le nom des colonnes et pour terminer le ORDER BY (ASC / DESC).
Nous avons également révisé les commandes de base d'SQL en console afin d'être capable d'afficher l'aide, d'y chercher quelque chose, d'afficher la liste des bases de données, en choisir une pour travailler avec, afficher la liste des tables etc etc.

Dans ce second jour de soutien, nous allons voir :

- WHERE
- LIMIT / OFFSET
- AVG / MAX / MIN
- LIKE
- COUNT
- GROUP BY

Ce Joue 02 n'est donc pas fondamentalement très chargé. Il faut cependant que vous assimiliez bien ces concepts. Notre 3ème et dernier jour sera consacré aux jointures, ce qui représente la partie la plus "complexe" de SQL.

----------

## Exercice 0 ##

Nous allons reprendre la base de données que nous avons utilisé pour le jour #1. Elle ne change pas.

Vous pouvez donc ouvrir un terminal, et y lancer l'invite de commande mysql en root.

## Exercice 1 ##

Les SELECT sont je pense bien compris. Nous allons donc passer à la suite.

Selectionnez donc tous les messages privés envoyés entre Mathias (id_member 3) et Sophie (id_member 4). Vous afficherez l'ID de l'envoyeur, et l'ID du destinataire, puis le contenu du message, et enfin la date.

Les colonnes seront nommées respectivement "From", "To", "Message" et enfin "Date".

N'utilisez pas les jointures ! Pas encore ;)

## Exercice 2 ##

Selectionnez maintenant tous les posts de murs pour lesquels le mot "je" est utilisé.

Vous afficherez le contenu du message dans une colonne nommée "Contenu", et la date dans une colonne nommée "Date".

On classera les posts par ordre décroissant de dates.

## Exercice 3 ##

Selectionnez maintenant 3 utilisateurs de la tables members à partir de l'ID 2, en exculant l'ID 3.

Vous afficherez leurs prenoms, leurs noms, et leur mail. Les colonnes seront respectivement nommées "Prenom", "Nom", et "Adresse mail".

Les résultats seront classés par ordre alphabétique inverse de noms.

## Exercice 4 ##

Affichez le nombre de posts de mur que l'utilisateur id_member=1 a posté.

On nommera la colonne de résultat "Nombre de posts".

## Exercice 5 ##

Affichez le dernier post de mur en date qu'a posté le membre ayant pour id 1.

Vous devez utiliser MAX().

Vous afficherez le contenu du post dans une colonne nommée "Post", puis la date à laquelle la publication a été postée dans une colonne nommée "Date".