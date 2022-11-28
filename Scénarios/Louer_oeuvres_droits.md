# Louer une œuvre sous droits d’auteur
Description : Location d’une œuvre sur l’application par l’utilisateur pour pouvoir la consulter.
Acteurs : L’utilisateur
Prérequis : L’oeuvre ne doit pas déjà être en cours de validation, le membre ne doit pas être anonyme
## Etapes :
-        Un membre se connecte à l’application par FranceConnect
-        Le membre sélectionne les œuvres qu’il voudrait louer à partir d’une recherche avec des filtres
-        L’application lui affiche la liste des œuvres qu’il voulait avec les filtres
-        Le membre authentifié sélectionne l’œuvre qu’il souhaite Louer.
-        L’application affiche un formulaire avec les champs à remplir pour la location (date de location, numéro de carte, nom, prénom…).
-        Le membre authentifié  remplit les champs avec les informations à fournir.
-        Le membre authentifié  valide le formulaire une fois rempli pour valider la location
- 	  Le membre authentifié peut accéder à l’oeuvre louée par l’application pour la durée pour laquelle il a payer.
### Scénarios alternatifs :
### Scenario erreur :
-	l’oeuvre n’est pas présente dans l’application ou est en phase de validation
-	Les infos données par l’utilisateur son fausses
#### Données, document, écrans :
