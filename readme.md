Les devoirs Anymo
=================

Le refuge pour animaux abandonnés Anymo veur mettre en ligne les animaux qu'ils ont à faire adopter. 

![Anymo](public/images/logo_anymo.svg)

On vous demande de faire les pages d'administration du site web.

Ce projet est un amalgame de 2 devoirs simples : L'interface (5%) et la mécanique (5%)

Préparation
-----------
1. Télécharger ou cloner le dépôt du projet
1. Compléter l'installation avec :
   1. La commande `composer update`
   2. L'ajout du `.env`
   3. La commande `php artisan key:generate`

Visuel (l'interface)
--------------------
Vous devez faire une interface simple, agréable et fonctionnelle de votre cru.

Le site doit nécessairement utiliser une page maîtresse dans laquelle on doit inclure minimalement les fichiers `entete`, `menu` et `pied` afin de bien normaliser le code.

Vous devez inclure le logo de l'organisme qui se trouve dans le dossier `public/images`. Comme il s'agit d'un SVG, vous pouvez facilement ajuster les couleurs en modifiant le code du fichier directement dans VSCode. De plus, si vous voulez utiliser la fonte du logo (optionnel) celle-ci se trouve également dans le dossier `public/images`

Fonctionnalités (la mécanique)
------------------------------
Dans votre site, l'usager doit pouvoir :
- faire afficher la liste des animaux (seulement le nom et l'espèce)
- faire afficher la fiche complète d'un animal choisi
- ajouter un animal
- modifier un animal existant
- naviguer aisément d'une fonctionnalité à l'autre

Votre site n'a pas besoin de :
- premettre de faire une recherche
- trier les animaux
- permettre de supprimer un animal

Les routes
----------
Utiliser le pattern d'adressage vu dans les exemples de "Monde Pokémons" avec la différence que les pages se trouvent dans un "dossier" `admin`. Par exemple, la fiche de Fido est accessible à l'adressse `http://localhost/admin/animal/123`

La table de données
-------------------
|Nom du champ|Type de donnée|Autres détails   |
|------------|--------------|-----------------|
|id          |Auto-increment|                 |
|nom         |text          |                 |
|espece      |text          |                 |
|race        |text          |                 |
|sexe        |integer       |0=femelle; 1=mâle|
|age         |real          |                 |
|couleur     |text          |                 |
|description |text          |nullable         |
|image       |text          |nullable. URL absolue vers une image d'animal|

Les données
-----------
Puisque le site comporte une fonction "create", vous n'avez pas à ajouter des données lors de l'installation de la base de données. Vous n'avez donc pas à créer de seeder ni de faker.

Remise
------
- Compte pour 10% de la note finale
- Durée une semaine. À remettre le lundi 12 avril avant minuit.
- Remettre dans le projet `anymo` sur https://remise.cstj.qc.ca
