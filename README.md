# La-C-corp

Nom du projet : NuméBook

L'objectif de ce projet est de pouvoir une bibliothèque numérique à gestion décentralisée.
Le principe est de permettre à chaque membre de numériser les œuvres et aux bibliothécaires de 
les proposer à l'emprunt selon deux modalités. Sois des livres qui sont libres de droits et sont donc 
accessibles à tout le monde du moment que les memebres ont bien asser d'espace sur le disque réservé
et des oeuvres sous droits qui sont proposées en location pour une période de 2 semaines.

Description :
Toutes les œuvres du domaine public sont accessibles gratuitement, toutes les œuvres sous droits sont proposées en location pour une période de 2 semaines.
Lorsqu'une œuvre passe dans le domaine public, elle devient accessible gratuitement et est diffusée aux membres ayant accordé à l'application suffisamment d'espace disque.
Chaque membre de la bibliothèque peut emprunter ou louer une œuvre.
Chaque membre peut proposer une œuvre et ainsi enrichir la bibliothèque.
Chaque œuvre est constituée d'un fichier contenant l'œuvre et d'un fichier au format json contenant les informations sur l'œuvre.
L'application bibliothèque possède un index des œuvres qui est mis à jour à chaque ajout ou suppression d'œuvre.
L'application possède quatre rubriques proposées sous forme de répertoires.
Un répertoire "fond_commun" avec une partie des œuvres libres de droits de l'association.
Un répertoire "emprunts" avec les œuvres sous droit empruntées par le membre qui sont chiffrées avec sa clé.
Un répertoire "séquestre" avec une partie des œuvres sous droit gérée par l'association, tous les fichiers y sont chiffrés, l'index n'y est pas accessible de façon directe.
Un répertoire "à modérer" avec les œuvres que le membre a proposées.
Lorsqu'une œuvre est proposée par un membre, elle est soumise à modération.
Les bibliothécaires voient les œuvres soumises, vérifient et complètent les données telles que les auteurs, éditeur, langue, pays d'origine, date de publication, droits, catégorie de l'œuvre, format du support, puis ils décident du statut de l'œuvre et donc si elle est dans le domaine public ou non, ou si elle est rejetée.
Selon le statut de l'œuvre modérée, l'application range dans la bonne rubrique et gère les droits d'accès.
Si l'œuvre est dans le domaine public il peut y en avoir autant de copie qu'il y a de membre.
Si l'œuvre est protégée alors il ne peut y avoir que 3 fois plus de copies que de licence d'exploitation, et chaque œuvre est chiffrée par une clé différente ayant une date de validité.
À la fin de la validité d'un emprunt, l'application bibliothèque supprime automatiquement l'œuvre du répertoire du membre.

Date de dernière modification : 28/11/2022
Auteurs : Mohamed Dumerchez/Aujay Antoine/Rayan Hamadache Desplanques

Version : 2

Liens différents readme :

Scénarios : https://github.com/Antoineaujay/La-C-corp/blob/main/Sc%C3%A9narios/readme.md

Diagrammes de classe : https://github.com/Antoineaujay/La-C-corp/blob/main/Diagrammes%20de%20Classes/readme.md

Diagramme de séquence : https://github.com/Antoineaujay/La-C-corp/blob/main/Diagrammes%20de%20S%C3%A9quence/readme.md

Glossaire + Suivi : https://github.com/Antoineaujay/La-C-corp/blob/main/Glossaire%20%2B%20Suivi/readme.md

