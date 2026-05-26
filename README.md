# Application CNED86 - Gestion des absences

---

## 1. Contexte du projet
Cette application a été développée dans le cadre de l'atelier 2 du BTS SIO SLAM.

Elle permet la gestion des absences du personnel (ajout, modification, suppression, consultation).

---

## 2. Objectif de l’application
L’objectif est de fournir un outil de gestion des absences permettant de centraliser les informations des personnels, services et motifs.

## Cas d'utilisation couverts

L'application permet de :

- Se connecter en tant que responsable
- Ajouter un personnel
- Modifier un personnel
- Supprimer un personnel
- Consulter les absences
- Ajouter une absence
- Modifier une absence
- Supprimer une absence
- Empêcher le chevauchement des périodes d'absence

---

## 3. Fonctionnalités
- Authentification utilisateur
- Gestion des personnels
- Gestion des services
- Gestion des motifs d’absence
- Gestion des absences (CRUD)
- Interface de consultation

---

## 4. Technologies utilisées
- C#
- Windows Forms
- MySQL  (XAMPP)
- Visual Studio
- Git / GitHub

## Architecture du projet

L'application suit une organisation en couches :

- Model : représentation des données
- DAL : accès à la base de données
- Controller : traitement logique
- View : interfaces utilisateur

Cette architecture facilite la maintenance et l'évolution du projet.

---

## 5. Base de données
Le script SQL complet est fourni dans le dépôt.

Il contient :
- création des tables
- relations entre tables
- données d’exemple
- création utilisateur et droits

---

## 6. Modélisation

### MCD
![MCD](images/image_bdd.png)

### Diagramme de paquetages
![Paquetages](images/image_schéma.png)
---

## 7. Interfaces de l’application

### Connexion
![Login](images/image_connexion_responsable.png)

### Gestion du personnel
![Menu](images/image_gestion_du_personnel.png)

### Ajout d'un personnel
![Ajout Personnel](images/image_ajouter_un_personnel.png)

### Modifier un personnel
![Modifier Personnel](images/image_modifier_un_personnel.png)

### Gestion des absences
![Absences](images/image_gestion_des_absences.png)
### Ajout d'une absence
![Ajout absence](images/image_ajouter_une_absence.png)

### Modifier une absence
![Modifier absence](images/image_modifier_une_absence.png)
---

---

## 8 Installation de l’application

### Prérequis

- Visual Studio
- XAMPP
- MySQL/MariaDB
- .NET Framework compatible

### Installation

1. Installer XAMPP et démarrer Apache + MySQL
2. Importer le script SQL fourni
3. Créer automatiquement la base cned86
4. Vérifier l'utilisateur SQL :

login : admin
mot de passe : admin123

5. Installer l'application via le fichier .msi
6. Lancer l'application

### Connexion à l'application

Identifiant : admin

Mot de passe : admin123

---

## Historique des commits

### 1. Initialisation du projet
Mise en place de la solution Visual Studio, organisation de l’architecture générale (Model, View, Controller, DAL) et création du dépôt Git.

### 2. Ajout de la base de données
Création et intégration de la base de données MySQL (via XAMPP). Mise en place des tables principales : personnel, absence, service, motif et responsable.

### 3. Création des interfaces utilisateur
Développement des interfaces Windows Forms permettant l’interaction utilisateur (navigation principale et formulaires de gestion).

### 4. Mise en place de l’authentification
Développement du système de connexion avec vérification des identifiants via la table responsable.

### 5. Gestion du personnel
Implémentation des fonctionnalités CRUD (ajout, modification, suppression, affichage) pour la gestion des employés.

### 6. Gestion des absences
Création du module de gestion des absences avec liaison aux tables personnel et motif.

### 7. Création du README et documentation
Rédaction du fichier README, ajout des captures d’écran (MCD, interfaces, architecture) et documentation complète du projet.

### 8. Génération de l’installeur
Création du package d’installation permettant de déployer l’application sur un autre poste utilisateur.

---

## 9. Documentation utilisateur

Une vidéo de démonstration présentant l’ensemble des fonctionnalités est disponible dans le portfolio :

- authentification
- gestion du personnel
- gestion des absences
- contrôle des chevauchements
- suppression et modification


## 10. Améliorations possibles
- Export PDF
- Recherche avancée
- Gestion des rôles
