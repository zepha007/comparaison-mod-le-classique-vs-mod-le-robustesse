Comparaison entre modèle classique OLS et modèle de régression robuste

Ce projet présente un TP réalisé en Python visant à comparer les performances d'un modèle de régression linéaire classique OLS face à un modèle de régression robuste de type Huber, en présence de valeurs aberrantes ou outliers.

Dataset utilisé
Le dataset utilisé est California Housing, disponible via la bibliothèque scikit-learn. Des perturbations et des outliers artificiels ont été volontairement injectés dans la variable cible afin d'analyser l'impact de ces valeurs extrêmes sur les différents algorithmes.

Méthodologie et Analyse
Dans un premier temps, un modèle linéaire OLS et un modèle robuste HuberRegressor ont été entraînés sur les données corrompues par des outliers.
Ensuite, une phase d'évaluation s'appuyant sur les métriques du coefficient de détermination R-deux, de la racine de l'erreur quadratique moyenne RMSE et de l'erreur absolue moyenne MAE a permis de comparer leur comportement.
Enfin, une analyse de la stabilité des coefficients a été menée après le nettoyage et la suppression des valeurs extrêmes.

Résultats et Conclusion
L'analyse des résultats montre que l'ajout d'outliers perturbe fortement le modèle OLS standard, tandis que le modèle de régression robuste de Huber encaisse mieux ces perturbations et se montre plus fiable face aux données bruitées.
On en conclut qu'il est préférable d'utiliser des approches robustes lorsque le jeu de données réel contient des valeurs aberrantes non nettoyées.
