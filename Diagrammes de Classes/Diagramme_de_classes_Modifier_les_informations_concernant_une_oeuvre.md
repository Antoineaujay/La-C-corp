@startuml

class Utilisateur {

String nom d'utilisateur

String MDP

SeConnecter(nom d'utilisateur, MDP)

}

Interface application{

}

class acceuil {}

class mes\_oeuvres{}

protocol UIcontroller {

applyfilter()

Updateview()

Updatelist()

modérer\_une\_oeuvre()

}

class Database {}

Utilisateur -\> application : Se connecte à \>

application --o acceuil : affiche

mes\_oeuvres -\> UIcontroller : applique le filtre

UIcontroller -\> Database : modérer\_une\_oeuvre()

Utilisateur -\> acceuil : clique sur 'mes oeuvres'

acceuil --\> Utilisateur : affiche la page 'mes\_oeuvres'

Utilisateur -\> mes\_oeuvres : rentre le filtre

Utilisateur -\> mes\_oeuvres : clique sur 'sauvegarder'

Utilisateur -\> mes\_oeuvres : clique sur 'modifier'

Utilisateur -\> UIcontroller : édite les détails

mes\_oeuvres -\> Utilisateur : montre le formulaire

UIcontroller -\> Database : Updatelist()

UIcontroller -\> mes\_oeuvres : Updateview()

mes\_oeuvres -\> UIcontroller : Save les changements

Utilisateur -\> acceuil : clique sur 'mes oeuvres'
