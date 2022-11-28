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

mes\_oeuvres \<- Utili : clique "ajouter les infos de cette oeuvre"

mes\_oeuvres --\> Utili : montre formulaire

Utili -\> UIcontroller : met les details

Utili -\> mes\_oeuvres : clique sur "sauvegarder"

mes\_oeuvres -\> UIcontroller : Savechanges()

UIcontroller -\> Database : modérer\_une\_oeuvre()

group si modérer\_une\_oeuvre() = Oui

UIcontroller -\> Database : ajoutoeuvre()

UIcontroller -\> mes\_oeuvres : Updateview()

mes\_oeuvres --\> Utili : réponse automatique

end

@enduml
