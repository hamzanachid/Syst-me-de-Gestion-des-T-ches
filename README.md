# Cahier des Charges - Système de Gestion des Tâches

## Objectif du Projet
Le projet vise à développer un système de gestion des tâches robuste utilisant Spring Boot, intégrant des fonctionnalités de sécurité avancées, de gestion des utilisateurs, et des notifications par e-mail.

## Fonctionnalités Principales

### Authentification et Autorisation
1. **Enregistrement et Connexion :**
   - Les utilisateurs doivent pouvoir s'inscrire en fournissant des informations telles que le nom, l'e-mail, et le mot de passe.
   - La connexion doit être sécurisée, utilisant Spring Security avec JWT pour l'authentification.

2. **Gestion des Rôles :**
   - Définir deux rôles : Utilisateur standard et Administrateur.
   - Les administrateurs auront des autorisations spécifiques telles que la suppression de tâches.

3. **Modification de Mot de Passe :**
   - Les utilisateurs doivent pouvoir modifier leur mot de passe en fournissant l'ancien mot de passe et le nouveau mot de passe.

4. **Token de Rafraîchissement :**
   - Mettre en place un mécanisme de token de rafraîchissement pour prolonger la durée de session sans avoir à se reconnecter.

### Gestion des Tâches
1. **CRUD de Tâches :**
   - Permettre aux utilisateurs de créer, lire, mettre à jour et supprimer des tâches.
   - Les tâches doivent avoir des attributs tels que le titre, la description, la date d'échéance et le statut.

2. **Contrôle d'Accès aux Tâches :**
   - Définir des autorisations basées sur les rôles pour les actions sur les tâches (p. ex., les utilisateurs normaux ne peuvent pas supprimer de tâches).

3. **Recherche et Filtrage :**
   - Implémenter une fonction de recherche permettant aux utilisateurs de rechercher des tâches par titre, statut, date d'échéance, etc.
   - Ajouter des filtres pour affiner les résultats.

### Notifications par E-mail
1. **Notifications d'Événements :**
   - Envoyer des e-mails pour des événements tels que la création de tâches, la date d'échéance approchant, etc.
   - Utiliser des modèles d'e-mails pour une personnalisation.

### Sécurité
1. **Gestion des Exceptions :**
   - Mettre en place une gestion robuste des exceptions pour fournir des messages d'erreur significatifs aux utilisateurs.

2. **Audit Trail :**
   - Enregistrer les actions importantes effectuées par les utilisateurs (p. ex., modification de tâches, connexions, déconnexions).

### Documentation
1. **Documentation API :**
   - Utiliser Swagger ou Spring RestDocs pour documenter toutes les API REST.

### Tests
1. **Tests Unitaires et d'Intégration :**
   - Rédiger des tests pour assurer le bon fonctionnement des composants critiques.

## Technologies Utilisées

- **Backend :**
  - Spring Boot (Spring MVC, Spring Data JPA)
  - Spring Security (JWT)
  - Base de données : H2 ou MySQL
  - Maven ou Gradle pour la gestion de projet

- **Frontend (Optionnel) :**
  - React ou Angular

- **Outils Supplémentaires :**
  - Swagger ou Spring RestDocs pour la documentation de l'API
  - Git pour le contrôle de version
  -

## Livrables Attendus

1. Application Spring Boot fonctionnelle avec les fonctionnalités spécifiées.
2. Documentation détaillée de l'API.
3. Rapport de tests décrivant les tests effectués et les résultats obtenus.

## Contraintes Techniques
- Utiliser Java 8 ou version ultérieure.
- Assurer la sécurisation des données sensibles, notamment les mots de passe.
- Respecter les principes SOLID et les bonnes pratiques de développement.

## Échéancier
Le projet devra être livré d'ici 01/02/2024 avec des points de contrôle réguliers pour évaluer les progrès.
