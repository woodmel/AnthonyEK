# Analyse du phasage énergétique en France (2018-2023)

# Contexte du projet
La transition énergétique transforme en profondeur le système électrique français. L'intégration croissante des énergies renouvelables (éolien, solaire), qui se caractérisent par une production intermittente, soulève de nouveaux défis pour maintenir l'équilibre constant entre l'offre et la demande. 
L'objectif de ce projet est d'évaluer la capacité du système électrique à assurer cet équilibre (phasage) aux échelles nationale et régionale, dans ce contexte de transition.

# Données et Stack Technique
Source des données : Plateforme Open Data Réseaux Énergies (ODRE) via la base éco2mix publiée par RTE.
Volumétrie : Plus d'un million d'observations couvrant la période de janvier 2018 à janvier 2023 à une résolution temporelle horaire.
Outils utilisés : Python (nettoyage, pré-traitement, agrégation, visualisations analytiques et analyses statistiques).
# Lien vers le code source : https://colab.research.google.com/drive/19-6uddq3BzWdM8zEI9xfl3Q4TXlDjkg9?usp=sharing

# Méthodologie
1. Pré-traitement et nettoyage : Filtrage temporel, traitement des valeurs manquantes, et sélection des variables pertinentes (exclusion des technologies très peu renseignées comme le stockage batterie ou l'éolien offshore).
2. Feature Engineering : Construction de variables temporelles complémentaires (année, mois) et agrégation des données horaires par région.
3. Analyse exploratoire et Visualisation : Création de tableaux de bord et de graphiques pour analyser l'évolution annuelle, les profils saisonniers, et la composition du mix électrique par région et par filière.

# Insights Clés (Résultats)
Une robustesse nationale face à la saisonnalité : Le système est structurellement excédentaire en moyenne mensuelle, mais la consommation est très saisonnalisée avec de forts pics hivernaux liés au chauffage.
Des tensions conjoncturelles plutôt que structurelles : L'année 2022 a été particulièrement critique avec un écart production-consommation réduit (54 MW d'excédent annuel), principalement en raison d'une indisponibilité exceptionnelle du parc nucléaire et de la crise énergétique européenne.
Des spécialisations territoriales très hétérogènes : 
Des régions comme la Bourgogne-Franche-Comté ou la Bretagne sont très dépendantes des renouvelables en proportion.
Le mix renouvelable varie fortement : l'Occitanie et PACA sont dominées par l'hydraulique (pilotable), tandis que les Hauts-de-France et les Pays de la Loire dépendent massivement de l'éolien (intermittent).
Le paradoxe du verdissement : L'augmentation de la part des énergies renouvelables complexifie le phasage temporel, rendant le système de plus en plus dépendant des moyens de production pilotables (nucléaire, hydraulique, thermique) pour combler les creux de production.

# Recommandations Métier & Stratégiques
Pour sécuriser durablement l'équilibre du réseau, l'analyse des données mène aux recommandations suivantes :
Renforcer la flexibilité : Développer les capacités de stockage (batteries, stations de pompage) pour absorber la variabilité des énergies renouvelables à court terme.
Maintenir un socle de production pilotable : Préserver un minimum de production contrôlable pour compenser l'intermittence verte et assurer la sécurité d'approvisionnement.
Adapter la planification à l'échelle locale : La stratégie énergétique ne peut pas être uniforme à l'échelle nationale ; elle doit s'adapter aux potentiels et contraintes spécifiques de chaque région.
Optimiser la gestion de la demande : Développer les mécanismes d'effacement pour réduire les pics de consommation, notamment inciter les industriels et les particuliers à adapter leurs usages.

---
# Ce projet a été réalisé dans le cadre d'un mémoire pour la certification Business Data Analyst délivré par l'Ecole des Mines de Paris sous la direction de M. Antoine TARDIVON.
