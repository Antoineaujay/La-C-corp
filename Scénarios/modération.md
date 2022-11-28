# Modérer une œuvre numérisée
	Description : Les bibliothécaires sont avertis des numérisations d’œuvres à modérer.
	Acteurs : Bibliothécaire, serveur de la Bibliothèque Nationale de France
	Prérequis :Le fichier d’une œuvre numérisée doit avoir été déposé et soumis en modération
## Étapes :
1.	L’un des bibliothécaires se connecte à l’application.
2.	L’application lui affiche la liste des fichiers d’œuvres numérisées soumises.
3.	Le bibliothécaire positionne ses filtres pour ne voir que les œuvres susceptibles de l’intéresser.
4.	L’application n’affiche que les résultats correspondant aux filtres.
5.	Le bibliothécaire positionne les tris pour les afficher dans l’ordre voulu.
6.	L’application affiche les résultats dans l’ordre souhaité.
7.	Le bibliothécaire sélectionne un fichier d’une œuvre.
8.	L’application affiche les informations saisies par le membre ayant soumis l’œuvre.
9.	L’application affiche un lecteur spécifique au type de fichier.
10.	Le bibliothécaire parcourt l’œuvre.
11.	Le bibliothécaire complète les informations sur l’œuvre.
12.	Le bibliothécaire accepte l’œuvre en précisant sa nature.
13.	13. L’application demande un confirmation de l’acceptation de l’oeuvre dans son répertoire
14. Le bibliothécaire valide la confirmation
15. L’application envoie une notification au membre qui a déposé l’oeuvre numérisée comme quoi leur oeuvre a été reçue et est dorénavant présente dans le répertoire de l’application
16. L’application enregistre le fichier de l’oeuvre et l’incrémente dans son fichier d’oeuvres.
### Scénario alternatifs:
-	Le bibliothécaire refuse l’oeuvre
-	L’application lui demande de donner une raison au refus en donnant un emplacement texte
-	Le bibliothécaire remplis tape ses raisons sur l’application et appuie sur confirmer
-	L’application envoie une notification à l'auteur de l’oeuvre disant que leur oeuvre a été refusée pour les raisons écrites par le bibliothécaire.
#### Scénario erreur : 
erreur de connexion au serveur et donc aucun accès au fichier avec les œuvres à valider.
##### Données,documents,écrans:
-	documents : fichier d’oeuvres numérisées soumises
-	données : serveur de l’association

