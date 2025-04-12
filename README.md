# 🧩 Image Matching Challenge 2025 - Reconstruction de Scènes 3D

## 📌 Présentation du Projet

Ce projet est réalisé dans le cadre du **Image Matching Challenge 2025**, qui comporte deux tâches principales :

1. **Regrouper les images par scène** : Identifier quelles images appartiennent à une même scène 3D et éliminer les images "bruitées" ou hors-sujet.
2. **Estimation de la pose 3D** : Estimer la position et l’orientation (matrice de rotation et vecteur de translation) de la caméra pour chaque image retenue.

L’objectif est de repousser les limites des systèmes de vision par ordinateur dans des environnements complexes, réels, et non structurés.

---

## 🧠 Motivation

Les collections d’images du monde réel sont souvent désorganisées : elles contiennent des photos non pertinentes, des objets différents mais visuellement similaires, et parfois des selfies ou des photos de café prises à proximité de monuments.  
Les méthodes traditionnelles de Structure-from-Motion (SfM) peinent dans ce genre de contexte.

Ce défi a pour objectif de concevoir des algorithmes capables de :

- Regrouper les images qui représentent la **même scène physique**,
- Écarter les **images inutiles ou parasites**,
- Reconstruire les **positions 3D des caméras** à partir de ces images.

---

## 📁 Structure du Projet

```bash
image-matching-2025/
│
├── notebooks/               # Notebooks Jupyter pour l'exploration, l'entraînement et les tests
├── src/                     # Code source : clustering, reconstruction et évaluation
│   ├── clustering/          # Algorithmes de regroupement d’images
│   ├── reconstruction/      # Logique SfM et estimation de pose
│   └── utils/               # Fonctions utilitaires (I/O, métriques, etc.)
│
├── data/                    # Données d'entraînement, de validation et de test
│   ├── train/
│   ├── test/
│   └── validation/
│
├── submission/              # Fichiers de soumission finale
│   └── submission.csv
│
├── requirements.txt         # Dépendances du projet
├── README.md                # Ce fichier
└── LICENSE
