@startuml

actor Utilisateur\_auth as Utili

acceuil \<- Utili : Seconnecter(nom d'utilisateur, MDP)

acceuil --\> Utili : retourne la page d'acceuil

Utili -\> acceuil : clique sur 'mes oeuvres'

acceuil --\> Utili : affiche les oeuvres faites par l'utilisateur

Utili -\> mes\_oeuvres : rentre le filtre

mes\_oeuvres -\> UIcontroller : applique le filtre

UIcontroller -\> UIcontroller : applyfilter()

UIcontroller -\> mes\_oeuvres : Updateview()

mes\_oeuvres --\> Utili

Utili -\> mes\_oeuvres : clique sur ''modifier''

mes\_oeuvres --\> Utili : montre le formulaire

Utili -\> UIcontroller : édite les détails

Utili -\> mes\_oeuvres : clique sur ''sauvegarder''

mes\_oeuvres -\> UIcontroller : save les changements (partID)

UIcontroller -\> Database : modérer\_une\_oeuvre()

Group si modérer\_une\_oeuvre() = Oui

UIcontroller -\> Database : Updatelist()

UIcontroller -\> mes\_oeuvres : Updateview()

mes\_oeuvres --\> Utili : "oeuvre modifiée''

end

@enduml
