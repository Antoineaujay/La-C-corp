# Se connecter:
Description : un membre veut se connecter à l’application à laquelle il s’est inscrite
Acteurs : Un utilisateur, FranceConnect, Les différents mandataires de FranceConnect
Prérequis: Le scénario “Devenir membre” et “Installer l’application” doivent être remplis sans erreur.
## Etapes:
-	L’utilisateur lance l’application
-	L'application détecte que l’utilisateur n’est pas connecté
-	l’application affiche une page de connection via FranceConnect avec comme champs : “identifiant” et “mot de passe”
-	l’utilisateur rentre ses identifiant créés auparavant
-	l’utilisateur est demandé de confirmer sa connection par une double authentification
-	l’application lui envoie un mail avec un code chiffré à rentrer
-	L’utilisateur rentre le code envoyé
-	Le membre maintenant authentifié accède à l’application sans soucis
### Scénario alternatif : 
#### Scénario erreur : 
-	l’utilisateur n’est pas inscrit
-	l’utilisateur à oublié ses identifiants
-	l’utilisateur ne rentre pas le code chiffré
Documents,données,équipement: 
Déposer une oeuvre numérique :
Données,documents,écrans: 
Documents : fichiers dans le répertoire “à modérer”, fichier journal local
Données : serveur de l’association 
