# Chapitre 4 — Un modèle pour une station : le GB à La Clapière

Le gradient boosting (GB) d'une seule station, et tout ce qu'on a appris en l'améliorant : les vraies prévisions météo, les variables, les intervalles de confiance, la cible « écart au débit actuel ».

| notebook | ce qu'on y trouve |
|---|---|
| [4.1](4.1_les_premiers_modeles.md) | X et Y, trois modèles (GB, Keras, PyTorch), le test avec les vraies prévisions ECMWF, les 51 scénarios. |
| [4.2](4.2_le_criblage_des_variables.md) | Le criblage des variables et de la grille (9 ou 25 km : presque la même note). |
| [4.3](4.3_les_intervalles_de_confiance.md) | Les intervalles de confiance : réglés sur la calibration avec les 50 scénarios, plafonnés. |
| [4.4](4.4_l_ecart_au_debit_actuel.md) | Prévoir l'écart au débit actuel plutôt que le débit : devenu la cible par défaut. |
| [4.5](4.5_combien_d_annees.md) | Combien d'années d'apprentissage faut-il au GB. |
| [4.6](4.6_les_crues_et_pluies_anciennes.md) | Apprendre aussi sur les crues puis sur les grosses pluies anciennes (Val-des-Prés, depuis 1976). |
| [4.7](4.7_en_ecart_a_la_partie_periodique.md) | Apprendre en écart à la partie périodique (chapitre 2.7). |
