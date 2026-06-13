# Projet de Synthèse - Modélisation Épidémiologique SEIRS

**Étudiante :** Salma BENSMAIL (Master 2 CHPS)  
**Année :** 2025-2026

## Description

Ce projet étudie la dynamique d'une épidémie via deux approches complémentaires :

1. **Partie 1 (ODE)** : résolution numérique d'équations différentielles (Euler, RK4).
2. **Partie 2 (SMA)** : simulation multi-agents optimisée (Python, C++, C).

L'objectif est d'analyser l'impact du choix technologique sur la performance HPC et l'empreinte énergétique (Green Computing).

## Structure du dépôt

```text
Projet_Synthese_SEIRS_Bensmail/
├── README.md
├── notebooks/
│   ├── Salma_BENSMAIL_Projet_Partie1_ODE.ipynb
│   ├── Salma_BENSMAIL_Projet_Partie2_SMA.ipynb
│   └── Salma_BENSMAIL_Projet_Partie3_Bonus.ipynb
└── reports/
    └── Salma_BENSMAIL_Rapport_Projet_SEIRS.pdf
```

## Contenu du dépôt

- `reports/Salma_BENSMAIL_Rapport_Projet_SEIRS.pdf` : rapport scientifique complet, incluant l'analyse, les résultats et les preuves.
- `notebooks/Salma_BENSMAIL_Projet_Partie1_ODE.ipynb` : notebook contenant la résolution numérique et la comparaison Python vs C++.
- `notebooks/Salma_BENSMAIL_Projet_Partie2_SMA.ipynb` : notebook principal contenant la simulation multi-agents et la comparaison Python / C++ / C optimisé.
- `notebooks/Salma_BENSMAIL_Projet_Partie3_Bonus.ipynb` : notebook dédié aux optimisations avancées, notamment les générateurs aléatoires et les mesures énergétiques.

## Instructions d'exécution

**Note importante :** ce projet utilise une approche de type *Notebook Orchestrateur*. Les codes sources C et C++ sont intégrés directement dans certaines cellules des notebooks via la commande `%%writefile`.

Pour reproduire les résultats :

1. Ouvrir un notebook, par exemple `notebooks/Salma_BENSMAIL_Projet_Partie2_SMA.ipynb`.
2. Exécuter les cellules séquentiellement (**Run All**).
3. Le notebook va automatiquement :
   - générer les fichiers `.c` et `.cpp`,
   - les compiler avec `gcc` / `g++`,
   - lancer les exécutables,
   - récupérer les résultats et tracer les courbes.

## Résultats clés

- **Performance :** le code C optimisé est jusqu'à **91x** plus rapide que la version Python.
- **Green Computing :** la consommation énergétique a été divisée par un facteur **270**.
