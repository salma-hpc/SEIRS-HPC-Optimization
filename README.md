# Projet de Synthèse - Modélisation Épidémiologique SEIRS
**Étudiante :** Salma BENSMAIL (Master 2 CHPS)
**Année :** 2025-2026

##  Description
Ce projet étudie la dynamique d'une épidémie via deux approches complémentaires :
1.  **Partie 1 (ODE) :** Résolution numérique d'équations différentielles (Euler, RK4).
2.  **Partie 2 (SMA) :** Simulation Multi-Agents optimisée (Python, C++, C).

L'objectif est d'analyser l'impact du choix technologique sur la performance HPC et l'empreinte énergétique (Green Computing).

##  Contenu du dépôt

*   **`BENSMAIL_Rapport_Projet_SEIRS.pdf`** : Le rapport scientifique complet (Analyse, Résultats, Preuves).
*   **`BENSMAIL_Projet_Partie1_ODE.ipynb`** : Notebook contenant la résolution numérique et la comparaison Python vs C++.
*   **`BENSMAIL_Projet_Partie2_SMA.ipynb`** : Notebook principal contenant la simulation multi-agents (comparaison Python / C++ / C optimisé).
*   **`BENSMAIL_Projet_Partie3_Bonus.ipynb`** : Notebook dédié aux optimisations avancées (Générateurs aléatoires & Mesures énergétiques).

##  Instructions d'exécution
**Note importante :** Ce projet utilise une approche "Notebook Orchestrateur".
Les codes sources **C** et **C++** sont intégrés directement dans les cellules des notebooks (via la commande `%%writefile`).

Pour reproduire les résultats :
1.  Ouvrez un notebook (ex: `Partie2_SMA`).
2.  Exécutez les cellules séquentiellement (**Run All**).
3.  Le notebook va automatiquement :
    *   Générer les fichiers `.c` et `.cpp`.
    *   Les compiler avec `gcc/g++`.
    *   Lancer les exécutables.
    *   Récupérer les résultats et tracer les courbes.

##  Résultats Clés
*   **Performance :** Le code C optimisé est **91x plus rapide** que la version Python.
*   **Green Computing :** La consommation énergétique a été divisée par un facteur **270**.
