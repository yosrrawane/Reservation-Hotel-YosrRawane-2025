EasyHotel_Spec.pdf
Projet – Document de Spécifications – Rendu 1
Auteurs : Yosr Rawane, taha ben rayana , rana miled , wassim belhaj , ele gharbi .
1. Introduction au projet
Objectif et périmètre du projet :
EasyHotel est une plateforme web de réservation d’hôtel en ligne. Elle permet aux utilisateurs de rechercher, comparer et réserver des chambres selon plusieurs critères (ville, dates, prix, confort). Le projet vise à faciliter la réservation, aussi bien pour les clients que pour les gestionnaires d’hôtels. L’application doit être accessible, intuitive et responsive.
Motivations :
Nous avons choisi ce projet car il touche un besoin réel, permet de mettre en œuvre plusieurs compétences (base de données, interface, logique métier), et offre des possibilités d’extensions futures. Il faisait partie de nos premières idées, car il combine utilité pratique et richesse fonctionnelle.
2. Spécification du projet
Notions de base et contraintes :
- Application web responsive.
- Authentification sécurisée pour deux profils (client / gestionnaire).
- Gestion des disponibilités via un calendrier.
- Paiement simulé en ligne.
- Langues : français / anglais.
- Technologies envisagées : HTML/CSS/JS, PHP ou Node.js, MySQL/MongoDB.
Acteurs et fonctionnalités (point de vue utilisateur) :
Client :
- Rechercher un hôtel par ville, date, filtre.
- Consulter les détails d’un hôtel (photos, services, avis).
- Réserver une chambre et simuler un paiement.
- Consulter, modifier ou annuler ses réservations.
Gestionnaire d’hôtel :
- Connexion sécurisée.
- Gérer les chambres (ajout, modification, suppression).
- Consulter les réservations, gérer les disponibilités.
Administrateur (optionnel) :
- Gérer les comptes utilisateurs, surveiller les contenus.
4. Priorisation des cas d’utilisation
Cas d’utilisation	Priorité
Rechercher un hôtel	Haute
Réserver une chambre	Haute
Gérer les chambres	Moyenne
Authentification	Haute
Paiement	Moyenne
5. Sprint 1 – Sélection et planification
Cas sélectionnés :
1. Rechercher un hôtel
2. Réserver une chambre
6. Spécifications détaillées et tests de validation
Cas : Rechercher un hôtel
Précondition : L’utilisateur est connecté.
Postcondition : Affichage d’une liste d’hôtels selon les critères.
Scénario principal :
1. L’utilisateur saisit la ville, les dates, les filtres.
2. Le système affiche les résultats.
3. L’utilisateur peut consulter les détails d’un hôtel.
Table de décision :
Ville saisie	Date valide	Résultat attendu
Oui	Oui	Liste d’hôtels correspondants
Oui	Non	Message : « date invalide »
Non	Oui	Message : « veuillez saisir une ville »
Cas : Réserver une chambre
Précondition : Hôtel et chambre sélectionnés.
Postcondition : Réservation enregistrée.
Scénario principal :
1. L’utilisateur sélectionne une chambre.
2. Il remplit ses informations.
3. Le système valide la disponibilité et confirme la réservation.
Table de décision :
Chambre dispo	Infos complètes	Résultat attendu
Oui	Oui	Réservation confirmée
Non	Oui	Message : « chambre non dispo »
Oui	Non	Message : « infos incomplètes »
## 📊 Diagrammes UML

### Cas d'utilisation
![Cas d'utilisation](diagrammes/cas_utilisation.png)

### Diagramme de classes
![Diagramme de classes](diagrammes/diagramme_classe.png)
