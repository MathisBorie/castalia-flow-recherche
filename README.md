# Castalia Flow — la recherche

Prévoir le débit des rivières françaises jusqu'à **5 jours**, avec des **intervalles de confiance** honnêtes, à partir des prévisions
météorologiques de l'ECMWF et des débits mesurés. Ce dépôt raconte la démarche : les données, leur analyse, les modèles essayés,
ce qui a marché et ce qui n'a pas marché, avec les figures et les résultats chiffrés.

Les prévisions sont en ligne sur **[castaliaflow.com](https://castaliaflow.com)**.

## Les chapitres

1. **[Les données](1_donnees/0_sommaire.md)** : une rivière et ses mesures, la météo (archive, prévisions, scénarios), les débits.
2. **[L'analyse des données](2_analyse_des_donnees/0_sommaire.md)** : liens entre débit et météo, erreurs des prévisions météo
   (lois gamma et normale), comparaison à GloFAS, le débit en fréquences.
3. **[L'atlas, les stations et les familles](3_atlas_stations_familles/0_sommaire.md)** : les bassins versants (BasinATLAS), le
   choix des points météo, le classement des rivières en 5 familles de régime.
4. **[Un modèle pour une station](4_gb_une_station/0_sommaire.md)** : le gradient boosting à La Clapière (Durance), les variables,
   les intervalles de confiance.
5. **[Le LSTM et les modèles multi-rivières](5_lstm_multi_rivieres/0_sommaire.md)** : un réseau pour des dizaines puis des centaines
   de rivières, les rivières jamais vues, un réseau par famille de régime.
6. **[Bien entraîner](6_bien_entrainer/0_sommaire.md)** : la validation, la demi-précision, le volume d'entraînement.
7. **[Bilans](7_bilans_et_service/0_sommaire.md)** : tous les modèles côte à côte, échéance par échéance.

## En bref

- Toutes les notes sont calculées **en conditions réelles** : sur des jours que le modèle n'a jamais vus, avec les prévisions
  météo telles qu'elles étaient publiées à l'époque (pas la météo observée après coup).
- Sur 36 rivières (R² médian à 1, 3 et 5 jours) : persistance (« le débit ne bouge pas ») 0,63 / 0,10 / −0,06 ; gradient boosting
  d'une station 0,77 / 0,59 / 0,49 ; **LSTM multi-rivières 0,85 / 0,68 / 0,56**.
- Un réseau par **famille de régime** (5 familles, 3 réseaux chacune) fait mieux sur les rivières jamais vues et pendant les crues :
  c'est le modèle en service.

## Le code

Ces pages sont les carnets de travail **sans leur code** : le texte, les figures et les tableaux de résultats. Le code (préparation
des données, modèles, service de prévision) est privé ; il peut être montré sur demande.

## Les données

Débits : Hub'Eau (Licence Ouverte), via RiverApp. Météo : ECMWF (CC BY 4.0), Open-Meteo (CC BY 4.0), dynamical.org. Bassins versants :
HydroSHEDS / BasinATLAS (CC BY 4.0). GloFAS : Copernicus.

## Contact

[mathis.borie@castaliaflow.com](mailto:mathis.borie@castaliaflow.com) — © 2026 Mathis Borie, tous droits réservés.
