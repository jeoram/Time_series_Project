📘 Rewriting the AI Time Series Notebook in PyTorch
🎯 Objectif du projet

Ce projet consiste à réécrire un notebook de séries temporelles (Time Series) en utilisant PyTorch, tout en comparant cette nouvelle implémentation avec le notebook d’origine.
L’objectif est d’obtenir une version plus claire, plus modulaire, et orientée vers l’entraînement d’un modèle réellement déployable.

🔍 Contenu du projet

Le projet se compose de trois éléments principaux :

1. Analyse et comparaison de deux notebooks existants

Étude des approches : preprocessing, architecture, entraînement.

Mise en lumière des différences :

méthodologie

fonctions utilisées

structure générale

qualité du code et facilité de réutilisation

Synthèse des avantages et limites de chaque version.

2. Réécriture complète en PyTorch

Le modèle original est réimplémenté en PyTorch pour :

mieux contrôler l’architecture du réseau

comprendre chaque étape du forward pass

maîtriser l’entraînement : loss, optimiser, device, batchs

rendre le code plus modulaire et réutilisable

3. Explication détaillée du modèle PyTorch

Le notebook fournit :

une description du modèle (type de réseau : RNN, LSTM, GRU ou autre)

l’explication des choix d’architecture

le schéma du pipeline :
Préprocessing → Dataset → DataLoader → Modèle → Entraînement → Évaluation

🧠 Architecture du modèle PyTorch

Le modèle implémenté suit la structure suivante :

Définition d’un Dataset personnalisé

Fenêtrage de la série temporelle

Normalisation

Création des séquences d’entrée / cible

Modèle PyTorch

Couche(s) récurrente(s) ou transformer

Couche fully connected en sortie

Activation adaptée au problème (prédiction continue)

Boucle d’entraînement PyTorch manuelle

Forward pass

Calcul de la perte (MSELoss)

Backpropagation

Mise à jour avec Adam

Suivi de la courbe de loss

Évaluation finale

📁 Structure du repository
├── notebooks/
│   ├── original_notebook.ipynb
│   ├── rewritten_pytorch_notebook.ipynb
│   └── comparison_notebook.ipynb
├── requirements.txt
├── .gitignore
└── README.md

🚀 Installation
1. Cloner le repo
git clone https://github.com/USERNAME/NOM-DU-REPO.git
cd NOM-DU-REPO

2. Installer les dépendances
pip install -r requirements.txt

📈 Résultats et observations

Le modèle PyTorch offre une meilleure modularité.

La structure du code est plus flexible pour tester différentes architectures.

Les performances dépendent du choix du modèle (LSTM/GRU/Transformer).

Le nouvel entraînement est reproductible et personnalisable.

🧩 Perspectives d’amélioration

Ajouter le support GPU/accelerator.

Intégrer un modèle Transformer pour séries temporelles.

Ajouter une évaluation plus complète (MAE, RMSE).

Exporter le modèle entraîné.
