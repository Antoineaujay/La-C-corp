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

Utilisateur - FRC : se connecte grâçe à \>

FRC --o authentification : vérifie les identifiants

authentification -\> application : si vérifier() = True

authentification -\> Database : va chercher les identifiants dedans

Database -\> authentification : confirme la présence des identifiants

authentification -\> Utilisateur : si verifier() = False, envoie un
message d'erreur

@enduml
