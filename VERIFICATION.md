# Vérification des fichiers fournis

Contrôle effectué le 15 septembre 2026. Les originaux ont été conservés sans modification et copiés dans le dossier.

## Données : contrôles réussis

- Table préparée : 150 observations, six pays, 25 années par pays (2000–2024).
- Aucune clé pays-année dupliquée, aucune année absente, aucune valeur manquante ou non positive dans les quatre colonnes analysées.
- Les 150 taux de la table préparée correspondent exactement aux valeurs pays-année de la feuille Data du même classeur.
- Tous les rythmes annuels recalculés correspondent aux pourcentages affichés, à deux décimales.
- Valeurs Côte d’Ivoire confirmées : 140,4 en 2000 ; 64,5 en 2024 ; variation −54,06 % ; rythmes annuels 3,31 % puis 3,13 %.
- Écart Côte d’Ivoire–Ghana : 40,5 en 2000 et 28,6 en 2024.
- Date de mise à jour indiquée dans la feuille Data : 2026-07-13. Il ne s’agit pas de la date de téléchargement.

Le classeur fourni a déjà été enrichi : il contient une feuille préparée et des éléments d’analyse. Il est conservé comme **classeur fourni**, pas présenté comme une copie brute certifiée du téléchargement initial. Le CSV préparé est extrait de ses quatre premières colonnes, sans reprise des éléments annexes situés à droite.

## Rapport Power BI : inspection de la structure enregistrée

- Deux pages retrouvées : vue d’ensemble et analyse détaillée.
- Le classement utilise une somme de SH.DYN.MORT, avec un filtre explicite Année = 2024. Sur une table à une ligne par pays-année, ce calcul restitue correctement le taux annuel. Ce n’est donc pas une erreur en soi.
- La courbe d’évolution utilise également une somme du taux : correcte au grain pays-année, sous réserve que le modèle chargé conserve l’unicité vérifiée dans le classeur.
- Un segment Année référence une autre table que celle des courbes. Son effet réel dépend des relations du modèle ; ne pas présumer que tous les visuels réagissent de la même manière.

## Limites de la vérification

Le modèle de données du PBIX est compressé. Les expressions DAX enregistrées, les relations et l’historique Power Query n’ont pas été extraits. Les recalculs ci-joints sont indépendants, réalisés depuis le classeur, et non une exécution du moteur Power BI. Le rendu final n’a pas été réexporté depuis Power BI. Les captures déjà partagées et le test d’interaction signalé par l’auteur complètent cette inspection, sans remplacer ces contrôles.

Le PBIX n’a pas été modifié. Sur un autre ordinateur, un chemin de source local peut nécessiter une mise à jour avant actualisation. Le classeur nécessaire est inclus dans donnees/.
