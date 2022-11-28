# Devenir Membre
	Description : Un anonyme
	Acteurs : un utilisateur Anonyme, FranceConnect, les différents mandataires de FranceConnecte.
	Prérequis : le scénario « Installer l’application » a été exécuté sans erreur.
## Étapes :
1.	L’utilisateur anonyme lance l’application.
2.	L’application détecte que c’est son premier lancement sur le média.
3.	L’application affiche une page d’information.
4.	L’application propose à l’utilisateur de se connecter via FranceConnect.
5.	L’application propose de créer un compte ne pouvant déposer ou louer des œuvres.
6.	L’utilisateur choisit de se connecter via FranceConnect.
7.	L’application propose les différents sites d’identification.
8.	L’utilisateur choisit l’un des sites.
9.	L’utilisateur s’authentifie.
10.	L’application reçoit les informations de connexion.
11.	L’application affiche toutes les actions, dont celles de dépôt.

### Scénario alternatif:
	branchement à l’étape 6
1.	L’utilisateur choisit de créer un nouvel identifiant.
2.	L’application demande le nom , prénom et date de naissance de l’utilisateur.
3.	L’utilisateur saisit les informations.
4.	À partir de ces informations, l’application crée
•	un identifiant unique garantissant l’anonymat,
•	une paire de clés, publique et privée, pour enregistrer les opérations qui seront faites.
5.	L’application transmet l’identifiant et la clé publique au serveur de l’association.
6.	L’application affiche les actions permises.
7.	L’application affiche la liste des œuvres dans le domaine public.

#### Documents :
Page d’information affichée :  pour expliquer l’objectif de l’application, ses possibilités et précise que l’utilisateur devra utiliser un compte FranceConnect s’il veut pouvoir louer des œuvres sous droits ou déposer des œuvres.
