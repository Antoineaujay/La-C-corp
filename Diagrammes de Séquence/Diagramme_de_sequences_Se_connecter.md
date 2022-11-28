@startuml

actor Utilisateur as Utili

boundary FranceConnect as FRC

control authentification as Auth

entity Utilisateur as Utili2

Utili -\> FRC : Afficher Interface authentification

FRC --\> Utili : Interface affichée

Loop

Utili -\> FRC : Saisir nom d'utilisateur

Utili -\> FRC : saisir MDP

Utili -\> FRC : Cliquer sur "se connecter"

FRC --\> Utili : Afficher exception

FRC -\> FRC : controle de saisie

end

FRC -\> Auth : (succès de contrôle)

Auth -\> Utili2 : Verifier (nom utilisateur, mdp)

Utili2 --\> Auth : réponse

group Si vérifier() = false

Auth --\> FRC : voir alerte (utilisateur et mdp)

FRC --\> Utili : Message d'erreur s'affiche

end

Auth --\> FRC : connexion validée

FRC --\> Acceuil : Rediriger vers Acceuil

@enduml
