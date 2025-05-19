# Transfer-Learning-by-Chen-et-Al.-2013
Le présent projet ne peut être considéré comme indépendant des travaux intitulés "Améliorer la régression linéaire multiple grâce au transfert d'apprentissage" et "Transfer Learning par Bouveyron et al. 2010", dont la lecture est indispensable avant d’aborder celui-ci.

Nous allons expliciter comment l’estimateur par transfert est obtenu dans l’étude citée.
Comme dans les autres travaux, l’objectif est de combiner deux régressions linéaires issues de deux sources de données différentes :
- un petit ensemble de données, constitué d’observations de haute qualité mais coûteuses à obtenir,
- et un grand ensemble de données, plus facilement accessible, mais potentiellement biaisé.

Le but est de pouvoir effectuer des prédictions sur le petit ensemble de données de haute qualité en exploitant les informations fournies par le grand ensemble de données, malgré ses limitations.

L’application concrète de cette étude se situe chez Google, où l’on cherche à faire des prédictions sur une population cible à partir d’un petit échantillon de consommateurs. Ces derniers ont été sélectionnés et rémunérés pour partager leurs données de navigation sur Internet et de consommation de contenu télévisé.
Le grand échantillon, lui, provient d’une autre population ayant accepté librement la collecte de leurs données, mais sans incitation financière.

Si ce grand ensemble de données est totalement différent du petit, il ne présente aucun intérêt. En revanche, s’il est suffisamment similaire, sans être identique, il peut s’avérer utile.
Utiliser ce grand ensemble devient alors avantageux, même s’il existe un risque d’introduire un certain biais.

L’idée est donc de tirer parti des informations contenues dans l’ensemble de données le plus large pour enrichir l’analyse effectuée sur l’ensemble plus restreint, tout en minimisant l’introduction du biais.

Le Notebook relatif au projet est consultable via le lien ci-dessous.
