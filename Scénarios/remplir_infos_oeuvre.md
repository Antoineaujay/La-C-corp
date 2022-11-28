# Remplir les informations concernant une œuvre :
Description : Un membre souhaite remplir les informations concernant une œuvre.
Acteurs : membre
Prérequis : le scénario “Déposer une oeuvre numérisée” et “modérer une oeuvre numérisée” doivent-être complétés sans erreurs.
## Etapes :
-        Un membre se connecte à l’application par FranceConnect.
-        Le membre authentifié demande à l’application de lui afficher les œuvres qu’il à déposées et qui ont été validées.
-        L’application lui affiche la liste des œuvres déposées et validées.
-        Le membre sélectionne l’oeuvre qu’il veut modifier et clique sur le menu de modification.
-        L’application affiche un formulaire avec les champs de l'œuvre à remplir
-        Le membre modifie les champs avec les informations qu’il veut donner sur l’oeuvre.
-        Le membre valide le formulaire une fois rempli.
-        L’application demande confirmation de l’envoi.
-      Le membre authentifié confirme l’envoi.
-      L’application enregistre le fichier dans le répertoire « à valider ».
-      Les serveurs de l’association notifient les bibliothécaires qu’une nouvelle
œuvre est en attente de modération.
-	  L’application indique au membre que son partage est en attente de modération.
### Scénarios alternatifs :
-         
#### Scenario erreur :
-        l’oeuvre du membre authentifié n’est pas déposée/validée
##### Données, document, écrans : 
Page d’information affichée : Pour confirmer avec l’utilisateur si il est sûr des modifications apportées.
