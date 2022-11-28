@startuml

class Utilisateur {

String nom d'utilisateur

String MDP

SeConnecter(nom d'utilisateur, MDP)

}

Interface application{

}

abstract class acceuil {}

abstract class mes\_oeuvres{

Savechanges()

}

protocol UIcontroller {

applyfilter()

Updateview()

Ajoutoeuvre()

modérer\_une\_oeuvre() }

class Database {}

Utilisateur -\> application : Se connecte à \>

application --o acceuil : affiche

mes\_oeuvres -\> UIcontroller : applique le filtre

UIcontroller -\> Database : modérer\_une\_oeuvre()

acceuil --\> Utilisateur : affiche la page 'mes\_oeuvres'

Utilisateur -\> mes\_oeuvres : rentre le filtre

Utilisateur -\> mes\_oeuvres : clique sur 'sauvegarder'

Utilisateur -\> mes\_oeuvres : clique sur 'ajouter les infos de cette
oeuvre'

Utilisateur -\> UIcontroller : met les détails

mes\_oeuvres -\> Utilisateur : montre le formulaire

UIcontroller -\> Database : Ajoutoeuvre()

UIcontroller -\> mes\_oeuvres : Updateview()

mes\_oeuvres -\> UIcontroller : Savechanges()

Utilisateur -\> acceuil : clique sur 'mes oeuvres'
