# Chapitre 5 — Le LSTM et les modèles multi-rivières

Du réseau d'une station au LSTM appris sur des centaines de rivières. Résultats clés (R² moyen médian, conditions réelles) : LSTM 36 rivières 0,684 contre 0,646 pour le GB de chaque rivière ; ensemble de 3 graines 0,714 ; 310 rivières n'aide pas (0,675) ; **familles de régime × 3 : meilleur modèle sur les rivières jamais vues (0,731 contre 0,691 pour le GB), meilleures en crue** — c'est le modèle en service.

| notebook | ce qu'on y trouve |
|---|---|
| [5.01](5.01_un_reseau_pour_4_stations.md) | Un seul réseau pour 4 stations de la Durance. |
| [5.02](5.02_un_lstm_pour_la_clapiere.md) | Un LSTM « passé + futur » pour La Clapière (90 jours de passé). |
| [5.03](5.03_l_albarine.md) | L'Albarine (karst) : 90 jours, puis 5 mois de passé et 5 réseaux. |
| [5.04](5.04_un_lstm_pour_36_rivieres.md) | Un seul LSTM pour 36 rivières, avec les attributs BasinATLAS. |
| [5.05](5.05_sur_des_rivieres_jamais_vues.md) | Ce LSTM sur des rivières qu'il n'a jamais vues. |
| [5.06](5.06_lstm_ou_nombre_de_rivieres.md) | GB et LSTM sur 4 puis 36 rivières : c'est surtout le nombre de rivières. |
| [5.07](5.07_combien_de_rivieres_ensemble_de_3.md) | La courbe du nombre de rivières (plateau vers 18), l'ensemble de 3 réseaux. |
| [5.08](5.08_310_rivieres.md) | Un LSTM sur 310 rivières, et sur 40 rivières jamais vues. |
| [5.09](5.09_lstm_commun_gb_correcteur.md) | Un LSTM commun sur 8 ans et un GB correcteur par rivière (écrit, jamais exécuté). |
| [5.10](5.10_un_lstm_par_famille_d_attributs.md) | Un LSTM par famille d'attributs (chapitre 3.4) : mieux en crue. |
| [5.11](5.11_un_lstm_par_famille_de_regime.md) | Un LSTM par famille de régime (chapitre 3.9), 3 graines, sur Kaggle : le modèle en service. |
| [5.12](5.12_familles_contre_lstm_36.md) | Famille par famille face au LSTM 36 : les grosses familles sont sous-entraînées. |
