@startuml

class Utilisateur {

String nom d'utilisateur

String MDP

SeConnecter(nom d'utilisateur, MDP)

}

Interface FRC {

}

Protocol authentification {

vérifier(nom d'utilisateur, MDP)

}

class Database{

}
interface application{

}

class acceuil {}

class mes_oeuvres{

Savechanges()

}
protocol UIcontroller {

applyfilter()

Updateview()

Ajoutoeuvre()

Updatelist()

modérer_une_oeuvre() 
}
UIcontroller -> acceuil : applique les filtres et les changements
UIcontroller -> mes_oeuvres : applique les filtres et les changements
Utilisateur - FRC : se connecte grâçe a l'application graçe à >
FRC --o authentification : vérifie les identifiants
FRC --o application : donne accès à >
application -> acceuil : affiche
authentification -> Database : confirme les identifiants donnés en les cherchants 
UIcontroller -> Database : indique les modifications à prévoir (ajout,modif)
acceuil -> mes_oeuvres : affiche la liste des oeuvres de l'utilisateur

@enduml
