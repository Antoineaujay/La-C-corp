@startuml

class Utilisateur {

String nom d'utilisateur

String MDP

SeConnecter(nom d'utilisateur, MDP)

}

class acceuil {}

protocol UIcontroller {

applyfilter()

Updateview()

}

Utilisateur -\> acceuil : SeConnecter(nom d'utilisateur,MDP)

Utilisateur -\> acceuil : rentre le filtre

acceuil -\> UIcontroller : applique le filtre

UIcontroller -\> UIcontroller : applyfilter()

UIcontroller -\> acceuil : Updateview()

acceuil --\> Utilisateur : retourne liste oeuvre avec ce filtre

Utilisateur -\> acceuil : clique sur 'lire l'ouvrage'

acceuil -\> Utilisateur : affiche l'ouvrage voulu

@enduml
