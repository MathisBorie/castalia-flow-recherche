# Chapitre 6 — Bien entraîner

Les réglages d'apprentissage qui valent pour tous les réseaux.

| notebook | ce qu'on y trouve |
|---|---|
| [6.1](6.1_la_validation_au_debut.md) | La validation au début de l'historique (2010-2012) plutôt qu'à la fin : 0,736 contre 0,714 ; c'est le réglage par défaut. Suivi du mélange des places de la validation dans l'ensemble. |
| [6.2](6.2_kaggle_demi_precision.md) | Kaggle (cartes T4) en demi-précision : 2,8 fois plus vite, même qualité ; réglage par défaut. |
| [6.3](6.3_plus_d_entrainement_ou_de_memoire.md) | Pluvial continental : 5 fois plus d'entraînement rattrape presque le LSTM 36 (0,761 contre 0,775) ; plus de mémoire n'apporte rien et abîme les crues. C'était surtout le volume d'entraînement. |
