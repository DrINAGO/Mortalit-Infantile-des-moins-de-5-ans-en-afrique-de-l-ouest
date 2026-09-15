# Mortalité des moins de cinq ans en Afrique de l’Ouest — 2000–2024

Projet d’analyse descriptive réalisé avec Power Query et Power BI sur six pays : Bénin, Burkina Faso, Côte d’Ivoire, Ghana, Sénégal et Togo.

## Question étudiée

Comment la mortalité des moins de cinq ans a-t-elle évolué depuis 2000, et comment les progrès de la Côte d’Ivoire se comparent-ils à ceux des cinq autres pays étudiés ?

## Données

- Source : [Banque mondiale — indicateur SH.DYN.MORT](https://data.worldbank.org/indicator/SH.DYN.MORT).
- Producteur des estimations : UN Inter-agency Group for Child Mortality Estimation (UN IGME).
- Unité : probabilité de mourir avant le cinquième anniversaire, exprimée pour 1 000 naissances vivantes.
- Période analysée : 2000–2024.
- Licence indiquée sur la fiche source consultée : CC BY 4.0.
- Nature : estimations officielles, et non données simulées ou dossiers individuels de patients.
- Méthode du producteur : [UNICEF — mortalité des moins de cinq ans](https://data.unicef.org/topic/child-survival/under-five-mortality/).

Les données décrivent six pays sélectionnés ; elles ne constituent pas une estimation agrégée pour toute l’Afrique de l’Ouest. La date exacte du téléchargement original n’a pas été conservée dans cette documentation. La fiche source a été consultée le 13 septembre 2026 ; ses estimations peuvent être révisées ultérieurement.
## Aperçu du tableau de bord

### Vue d’ensemble
![Vue d’ensemble](captures/dash%201.png)

### Analyse détaillée
![Analyse détaillée](captures/dash%202.png)

## Résultats principaux

| Pays | Taux 2000 | Taux 2024 | Variation absolue | Variation relative |
|---|---:|---:|---:|---:|
| Bénin | 135,0 | 74,7 | −60,3 | −44,67 % |
| Burkina Faso | 176,0 | 74,9 | −101,1 | −57,44 % |
| Côte d’Ivoire | 140,4 | 64,5 | −75,9 | −54,06 % |
| Ghana | 99,9 | 35,9 | −64,0 | −64,06 % |
| Sénégal | 128,9 | 36,5 | −92,4 | −71,68 % |
| Togo | 119,2 | 56,1 | −63,1 | −52,94 % |

Les taux et variations absolues sont exprimés pour 1 000 naissances vivantes. Les résultats des tableaux Power BI ont été rapprochés du classeur fourni et recalculés indépendamment.

1. **La mortalité diminue dans les six pays entre les deux dates.** En Côte d’Ivoire, elle passe de 140,4 à 64,5 pour 1 000, soit une baisse de 54,06 %.
2. **Le niveau final et le progrès relatif donnent des classements différents.** Le Ghana présente le taux le plus faible en 2024 ; le Sénégal réalise la plus forte baisse relative depuis 2000. Le Burkina Faso réalise la plus forte baisse absolue.
3. **L’écart absolu Côte d’Ivoire–Ghana diminue globalement**, de 40,5 à 28,6 pour 1 000, après une légère hausse au début de la période. Il reste positif en 2024.
4. **La baisse ralentit légèrement en Côte d’Ivoire** : le rythme annuel moyen logarithmique passe de 3,31 % sur 2000–2015 à 3,13 % sur 2015–2024. Un ralentissement de la baisse ne signifie pas une hausse de la mortalité.

## Rapport Power BI

Deux pages ont été construites :

- **Vue d’ensemble** : cartes des taux en 2000 et 2024 et de leur variation, pays sélectionné, comparaison des trajectoires Côte d’Ivoire–Ghana–Sénégal, classement des six pays en 2024 et évolution de l’écart Côte d’Ivoire–Ghana.
- **Analyse détaillée** : tableaux comparatifs, rythmes annuels moyens de baisse, principaux constats et limite d’interprétation.

Le segment Pays pilote les cartes de la vue d’ensemble. Le changement de pays sans modification des courbes comparatives a été testé par l’auteur du rapport.

## Compétences mobilisées

Structuration d’une table pays-année, transformations dans Power Query, mesures DAX avec contexte de filtre, calcul de variations, comparaison de périodes de durées différentes, configuration des interactions entre visuels et interprétation descriptive.

## Méthode et reproductibilité

Consulter [METHODE.md](METHODE.md) pour les calculs, le protocole de préparation et les limites de vérification. Le [dictionnaire des données](DICTIONNAIRE.md) décrit les variables.

Le dossier inclut désormais le rapport Power BI original, le classeur fourni, un CSV de 150 observations et les indicateurs recalculés. Les 150 taux préparés ont été rapprochés avec succès de la feuille Data du classeur. Consulter [VERIFICATION.md](VERIFICATION.md) pour les contrôles et les limites de l’inspection du PBIX.

## Limites

- Analyse descriptive : aucune relation causale avec une politique, un événement ou une intervention n’est démontrée.
- Estimations nationales : les disparités infranationales et sociales ne sont pas étudiées.
- Les intervalles d’incertitude ne sont pas représentés ; les classements portent sur les estimations ponctuelles.
- Les taux ne doivent être ni additionnés ni interprétés comme un taux régional à partir d’une simple moyenne des pays.
- Les rythmes de baisse décrivent des moyennes sur une période, et non une baisse identique chaque année.

