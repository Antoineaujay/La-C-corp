# Glossaire Technique : 

-	Anonyme : Utilisateur non encore authentifié ou n’ayant pas de compte.

-	Téléchargement de l’application :

-	Installation de l’application : 

-	Utilisateur : Anonyme ou Membre ou Bibliothécaire utilisant l’application. 

-	Média : Support permettant d'exécuter l’application de la bibliothèque décentralisée. 

-	authentifié:Membre dont la connexion s’est faite avec FranceConnect. 

-	Numéro de transaction : Identification unique de toute opération réalisée.

-	Fichier journal local : Fichier contenant un historique de toutes les opérations ayant été effectuées par le membre. 

-	Filtre : Permet de cacher des éléments d’une liste lorsque ces éléments ne sont pas voulus. 

-	Tri : Permet d’ordonner les éléments d’une liste selon les critères souhaités.

## Classes et rôles :
Uicontroller : Un protocole qui détecte les changements que les membres veulent faire sur la base de donnée (ajout, modifs) ou sur l’affichage (filtre) et fait en sorte de soi afficher le nécessaire ou d’envoyer un mail aux modérateurs avant de faire la modification si il reçoit l’info que cela été accepté.

FRC : Une interface qui sert de portail pour pouvoir accéder à l’application en elle-même, les utilisateur doivent avoir leurs identifiants(Nom d’utilisateur et MDP) pour pouvoir passer ce portail et donc accéder à l’application

Authentification : Protocole qui marche en tandem avec FRC pour pouvoir vérifier la présence des identifiants rentrés sur l’interface dans la base de données des utilisateurs.

Application : Une interface qui affiche les différentes partie de celle-ci (acceuil, mes œuvres, barre de recherche…)

Accueil : Une classe qui caractérise l’accueil de l’application et donc la page principale de celle-ci avec les différentes parties telles que la barre de recherches ou la liste des œuvres que l’utilisateur peu consulter.

Mes œuvres : une classe qui caractérise la liste des œuvres que l’utilisateur à implémentés, quelles soient validées ou non, d’ici il peut accéder à différentes tâches comme la modification ou le remplissage d’infos sur une œuvre.

Database : Une classe qui caractérise la base de données de l’application, les identifiants des membres, les œuvres, les modifications et ajouts en cours d’implémentation ou de refus, toute la vie de l’application se trouve dans cette partie.
