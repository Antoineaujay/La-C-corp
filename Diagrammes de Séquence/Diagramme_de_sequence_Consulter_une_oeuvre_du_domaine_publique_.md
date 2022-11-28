@startuml

actor Utilisateur\_auth as Utili

Page affichée \<- Utili : Seconnecter(nom d'utilistaeur, MDP)

Utili -\> UIcontroller : applique le filtre "domaine publique"

UIcontroller -\> UIcontroller : applyfilter()

UIcontroller -\> Page affichée : Updateview()

Page affichée --\> Utili : retourne une liste des oeuvres dans ce filtre

Utili -\> Page affichée : clique sur le bouton "Lire l'ouvrage" de
l'oeuvre souhaitée

Page affichée --\> Utili : retourne l'oeuvre en question sous format
numérique
