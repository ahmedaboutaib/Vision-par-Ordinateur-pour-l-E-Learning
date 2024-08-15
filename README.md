# Projet de Traitement Vidéo et Génération d'Images

Ce projet comprend deux scripts Python qui se concentrent sur la détection de poses dans des vidéos et la génération d'images à partir de contenu HTML. Ce fichier `README.md` fournit des détails sur le rôle de chaque script et les instructions d'installation.

## Introduction

Le projet inclut deux scripts principaux :
1. **Détection de Pose et Extraction de Frames** : Ce script traite des vidéos pour détecter les poses humaines et extrait les frames où les points de pose sont les plus éloignés en termes de profondeur.
2. **Génération d'Image HTML et Traitement Vidéo** : Ce script génère une image basée sur du contenu HTML avec une couleur de fond moyenne calculée à partir d'une image source et superpose cette image générée sur une autre image. Il traite également des vidéos pour supprimer l'arrière-plan et afficher l'image superposée.

## Code 1: Détection de Pose et Extraction de Frames

### Description

Ce script utilise la bibliothèque MediaPipe pour détecter les poses humaines dans des vidéos. Il analyse chaque frame de la vidéo pour extraire les coordonnées de deux points spécifiques de la pose. Ensuite, il identifie les frames où la profondeur (valeur `z`) de ces points est la plus élevée, et sauvegarde ces frames ainsi que leurs coordonnées dans un fichier Excel. Cela peut être utile pour des applications qui nécessitent l'analyse de la position des membres du corps dans des vidéos.

### Fonctionnalités

- Détection des poses humaines en temps réel.
- Extraction des frames basées sur la profondeur maximale des points de pose.
- Sauvegarde des frames extraites et des informations associées dans un fichier Excel.

## Code 2: Génération d'Image HTML et Traitement Vidéo

### Description

Ce script crée une image PNG à partir de contenu HTML. Il calcule d'abord la couleur moyenne d'une image source et utilise cette couleur comme fond pour l'image HTML générée. Ensuite, il superpose cette image générée sur une autre image. Le script traite également une vidéo pour supprimer l'arrière-plan et afficher l'image superposée dans la vidéo. Ce processus peut être utilisé pour intégrer des éléments visuels dans des vidéos ou des images, tout en conservant la qualité de la présentation.

### Fonctionnalités

- Génération d'images à partir de contenu HTML avec une couleur de fond calculée à partir d'une image source.
- Superposition de l'image générée sur une autre image.
- Traitement de vidéos pour supprimer l'arrière-plan et intégrer l'image superposée.

## Installation

Pour exécuter ces scripts, assurez-vous que toutes les dépendances nécessaires sont installées. Les instructions d'installation complètes sont fournies dans le fichier `install.ipynb`, qui contient tous les détails nécessaires pour configurer votre environnement et installer les packages requis.

## Utilisation

1. **Détection de Pose et Extraction de Frames** :
   - Placez les vidéos dans le répertoire spécifié dans le script.
   - Exécutez le script pour traiter les vidéos et extraire les frames avec les valeurs `z` maximales.

2. **Génération d'Image HTML et Traitement Vidéo** :
   - Préparez les images et vidéos nécessaires.
   - Exécutez le script pour générer l'image HTML, superposer l'image générée sur une image source, et traiter la vidéo pour supprimer l'arrière-plan et afficher l'image superposée.

Pour toute question ou problème, veuillez consulter le fichier `install.ipynb` ou contacter l'auteur du projet.

