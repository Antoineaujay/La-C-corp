# Modifier les informations concernant une œuvre
Description : Modifier les informations d’une œuvre déjà déposée et validée
Acteurs : Bibliothécaire, membre authentifié
Prérequis : le scénario “remplir les informations concernant une oeuvre” et “modérer une oeuvre numérisée” doivent-être validés sans erreurs.
## Etapes :
-        Un membre se connecte à l’application par FranceConnect.
-        Le membre authentifié demande à l’application de lui afficher les œuvres qu’il à déposées et qui ont été validées.
-        L’application lui affiche la liste des œuvres déposées et validées.
-        Le membre sélectionne l’oeuvre qu’il veut modifier et clique sur le menu de modification.
-        L’application affiche un formulaire avec les champs de l'œuvre à modifier.
-        Le membre modifie les champs avec les informations qu’il veut modifier sur l'œuvre.
-        Le membre valide le formulaire une fois rempli.
-        L’application demande confirmation de l’envoi.
-      Le membre authentifié confirme l’envoi.
-      L’application enregistre le fichier dans le répertoire « à valider ».
-      Les serveurs de l’association notifient les bibliothécaires qu’une nouvelle œuvre est en attente de modération.
-	  L’application indique au membre que son partage est en attente de modération.
-	  Un bibliothécaire se connecte à l’application par FranceConnect
-	L’application lui affiche la liste des fichiers d’œuvres numérisées modifiées.
-	Le bibliothécaire positionne ses filtres pour ne voir que les œuvres
-	susceptibles de l’intéresser.
-	L’application n’affiche que les résultats correspondant aux filtres.
-	Le bibliothécaire positionne les tris pour les afficher dans l’ordre voulu.
-	L’application affiche les résultats dans l’ordre souhaité.
-	Le bibliothécaire sélectionne un fichier d’une œuvre.
-	L’application affiche les informations saisies par le membre ayant modifier l’œuvre.
-	Le bibliothécaire parcours les modifications
-	Le bibliothécaire accepte les modifications
-	Les changements sont immédiats sur l'application.
### Scénarios alternatifs :
#### Scenario erreur :
-	l’oeuvre n’est pas dans la base de donnée
-	l’application plante
-	il n’y a pas de connection internet
-	les modifications ne s'enregistrent pas.
-	le bibliothécaire ne les acceptent pas
##### Données, document, écrans : 
La base de données des œuvres, l’application
