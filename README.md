# PREDICTION DE CHURN POUR SPARKIFY


## Table des matières

1. [Installation](#installation)
2. [Motivation du projet](#motivation)
3. [Descriptions de fichiers](#description)
4. [Résultats](#résultats)
5. [Remerciements](#Remerciements)


## Installation <a name="installation"></a>
Le code devrait s'exécuter sans problème avec les versions Python 3.* et PySpark 2.4.5. Si vous utilisez Anaconda, assurez-vous d'installer PySpark [ici](https://anaconda.org/conda-forge/pyspark).



## Motivation du projet <a name="motivation"></a>
Sparkify est un service de musique numérique fictif, créé par Udacity pour simuler des entreprises du monde réel telles que Spotify ou Pandora. Sur Sparkify, les utilisateurs peuvent lire des chansons avec un plan gratuit ou un plan d'abonnement premium, qui offre des fonctionnalités avancées et sans publicité. Les utilisateurs peuvent mettre à niveau, rétrograder ou annuler leurs services à tout moment, et par conséquent, il est très important de garder les utilisateurs satisfaits et de ne pas abandonner le service.

Le but de ce projet est d'analyser les journaux d'activité des utilisateurs et de créer un classificateur pour identifier les utilisateurs susceptibles de se désabonner - service de diffusion de musique Sparkify annulé. De plus, compte tenu de la réalité des données de streaming écrasantes, je n'utilise qu'un petit ensemble de données (98 Mo) de données Sparkify complètes (12 Go) pour l'exploration de données et le développement de modèles. Le modèle final est construit à l'aide de Spark, il est donc évolutif pour s'exécuter dans un environnement de clustering distribué.

Dans ce projet, je vais construire et évaluer les modèles ci-dessous et choisir les meilleures performances d'entre eux en fonction du score F1 :

1. Random Forest
2. Gradient Boosted Trees
3. Support Vector Machine


## Descriptions de fichiers <a name="description"></a>
1. **Churn_prediction_Sparkify.ipynb** - Modèle de prédiction EDA et Churn
2. **Sparkify_event.json** - Journaux des activités des utilisateurs


## Résultats<a name="résultats"></a>

Classement des performances par F1 :

1. Random Forest: F1 score 0.746, Accuracy 0.781
2. Gradient Boosted Trees: F1 score 0.731, Accuracy 0.734
3. Support Vector Machine: F1 score 0.685, Accuracy 0.781
4. Baseline Model: F1 score 0.685, Accuracy 0.781


## Remerciements <a name="Remerciements"></a>
Remerciements à **Udacity** pour les données.
