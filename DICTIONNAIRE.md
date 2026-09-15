# Dictionnaire des données

Grain attendu : une ligne par pays et par année. Clé attendue : Country Code + Année.

| Colonne du rapport | Signification | Type attendu | Unité / valeurs |
|---|---|---|---|
| Pays | Nom du pays | Texte | Bénin, Burkina Faso, Côte d’Ivoire, Ghana, Sénégal, Togo |
| Country Code | Identifiant pays | Texte | BEN, BFA, CIV, GHA, SEN, TGO |
| Année | Année de l’estimation | Entier | 2000 à 2024 |
| SH.DYN.MORT | Probabilité estimée de décéder avant le cinquième anniversaire | Décimal | Pour 1 000 naissances vivantes |

Les noms affichés dans le fichier peuvent être non accentués, par exemple Benin ou Cote d'Ivoire. Utiliser de préférence les codes pour identifier les pays dans les filtres de calcul.

Ne pas confondre la mortalité des moins de cinq ans avec la mortalité infantile, qui concerne les moins d’un an. SH.DYN.MORT n’est pas un nombre de décès et n’est pas exprimé directement en pourcentage.

Source : https://data.worldbank.org/indicator/SH.DYN.MORT

