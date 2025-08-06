# Data Scientist Junior  

## Profil  
Marc AZIAN 

Data Scientist, formé par DATAGONG, un centre de formation international réputé basé en France et piloté par des experts en Data Science. Membre actif de l’association 10 000 Codeurs, Je suis Data Scientist et je dispose déjà d'une solide expérience professionnelle en matière de manipulation des données. Pour ma soutenance de fin de formation, j'ai travaillé sur un projet de classification binaire visant à prédire les résultats électoraux des Etats-Unis sur la base des données sociodémographiques. En plus de ça, j'ai travaillé sur d'autres projets de machine learning comme le scoring, la segmentation de la clientèle, la classification binaire et la régression linéaire et j'ai également passé trois mois dans une entreprise de télécommunications (Celtiis Bénin) en tant que stagiaire où j'ai développé un modèle de churn pouvant permettre d'anticiper les risques de résiliation d'une offre de la part des clients de la société. Grâce à travers cette expérience, j'ai affiné mes compétences en matière d'analyse exploratoire pour l'identification des Insights fondamentaux pouvant orienter l'équipe marketing dans la prise de ses décisions stratégiques en vue de l'amélioration des chiffres d'affaires de la société. 

Ma spécialité réside dans l’utilisation de Python et je sais également manipuler les bases de données relationnelles avec SQL. Je dispose aussi des compétences en création des Dashbord de visualisations avec Power BI. Mon adaptabilité et ma capacité à maîtriser rapidement de nouveaux outils technologiques sont des atouts clés de mon parcours.

 Découvrez l’ensemble de mes réalisations dans ce portfolio.    

## Mes Projets 

### Projet 1 : Prédiction du churn des clients 

- Résumé 

  Dans ce projet de classification binaire, nous disposons d'une base de données d'une entreprise de telecom (Orange) divisée en deux parties.
La première composée de 80% des individus est consacrée à l'entraînement de notre modèle et la seconde pour le testing. 
L'objectif est bien sûr de construire un modèle capable de prédire la probabilité de churn des clients, en se reférant aux informations relatives à leurs divers plans de communication.

- Approche

  Après importation du jeu de données de train, nous avons procéder à la mise à l'echelle des valeurs numériques avec la méthode StandardScaler puis l'encoding des valeurs catégorielles par la méthode One Hot Encoding. Ensuite, nous avons effectué son prétraitement avant d'importer la base du test sur laquelle nous avons effectué le même exercice. Après cette étape, nous avons implémenté les modèles a utiliser (regression logistique, Xgboost, gradient boosting, SVM et KNeighbors) et les métriques d'évaluation : (roc_auc_score, classification_report). Pour terminer, nous avons comparé les résultats et choisir le meilleurs. 
  
- Résultat

Le gradient boosting nous a présenté les meilleurs scores à tous les niveaux, comparé aux autres modèles. 
  
- Lien github : https://github.com/VivoAZ/Churn-project 

### Projet 2 : Clustering de la clientèle 

- Résumé
  
  Nous disposons d'une base de données issue d'une campagne marketing d'une entreprise. L'objectif est de segmenter la clientèle en tenant compte du comportement des individus. C'est donc un projet de classification qui vise à regrouper les clients par catégorie afin de proposer des offres adaptées à chaque classe et optimiser le budget des campagnes et faciliter l'ecoulement des articles. 
  
- Approche

  Pour y arriver, nous avons utilisé d'abord la méthode du coude pour avoir une idée sur le nombre de cluster optimal, bien évidemment après avoir procédé au prétraitement des données. Dès lors, nous avons utilisé l'algorithme KMeans pour effectuer les prédictions sur les jeux de données de test et de train. Ensuite, grâce à PCA, nous avons réduis les dimensions avant de procéder à la visualisation des clusters. La même démarche a été répétée pour l'algorithme CAH afin de comparer les deux modèles. Sans surprise, les résultats étaient similaires. Pour terminer, nous avons effectué l'évaluation avec l'indice de silhouette. 

- Résultat

  Indice de Silhouette pour K-Means: 0.5518549972456119
  
  Indice de Silhouette pour CAH: 0.5435529942489229
  
- Lien github : https://github.com/VivoAZ/Projet-clustering-/tree/master 

### Projet 3 : Prédiction de prix des maisons 

- Résumé
  
  C'est un projet de regression linéaire sur les maisons dans la ville de Boston avec des features capitales. Notre objectif est de prédire le prix des maisons dans cette zone en nous basant sur la relation entre les différentes variables. Nous disposons des variables quantatives et deux variables catégorielles. Le type de machine learning adapté est le ML supervisé.
  
- Approche
  
  Après chargement des données, nous avons procédé à une analyse exploratoire qui nous a conduit aux traitements des valeurs manquantes. A ce niveau, nous avons opté par l'imputation avec la moyenne pour les valeurs numériques puis l'imputation par le mode pour les valeurs catégorielles. Ensuite, nous avons procédé à la visualisons des potentiels outliers parmi nos données et leurs relations avec notre target. Les outliers détectés ont été traités suivant une troncature. Après, nous avons utilité le One Hote Encoding pour encoder les variables catégorielles. Poour finir cette partie, nous avons créer un pipeline qui résume toutes les étapes executées. Enfin, nous avons entraîné plusieurs modèles par cross validation sur notre jeu de train et l'évaluer avec la métrique MAE sur le jeu de test.     

- Résultat 

  Le modèle Gradient Boosting nous a montré une bonne perfomance sur le jeu de train et du test. En effet, le MAE a donné respectivement 1.013 et 0.637. Ce sont de très bons scores qui montrent la capacité de notre modèle à s'adapter à de nouvelles données.  
  
- Lien github : https://github.com/VivoAZ/Projet-prediction-de-prix

### Projet 4 (soutenance) : Prédiction des résultats électoraux  

- Résumé 

  Pour ce projet, il est mis à notre disposition plusieurs bases de données à étudier pour prédire les résultats des élections présidentielles aux USA. Nous distinguons d'une part de quatres tables sur les données sociodémographiques à savoir : l'éducation, la population, la pauvreté et l'employablité. D'autres part, nous avons aussi les archives des élections de 2020, et un autre fichier sur les résultats de 2008 à 2016. Les bases de données sociodémographiques nous ont servir à créer un nouveau dataframe final et celle de 2020 à créer le target pour la prédiction. Quant à celle des archives de 2008 à 2016, elle nous a juste servi d'exploration et de comparaison. 

- Approche

  Pour rendre la base de données exploitable, nous avons suivi plusieurs étapes de nettoyage et de préparation, telles que la jointure des différentes bases de données, l’élimination des doublons, ainsi que le traitement des valeurs manquantes et des valeurs aberrantes. Lors de cette phase, nous avons rapidement identifié des variables et des individus présentant plus de 80 % de valeurs manquantes, que nous avons alors supprimés. Par la suite, nous avons constaté que plusieurs variables manquantes étaient fortement corrélées entre elles, ce qui a justifié le recours à la méthode KNN pour l'imputation des valeurs manquantes. En ce qui concerne les valeurs aberrantes, nous avons choisi de les détecter et de les remplacer par les moyennes des variables correspondantes.
  
  La base finale contient 3112 individus et 311 variables. La variable cible (target) a été déterminée en fonction des résultats des votes des républicains et des démocrates : si le nombre de votes des républicains était supérieur à celui des démocrates, la cible était assignée à 1 ; sinon, elle était assignée à 0. Après cette partie, nous avons procédé à l'analyse exploratoire de nos données, puis l'approche scientifique qui s'est déroulée en cinq différentes étapes :

1- Prétraitement des données avec Pipeline : Le prétraitement des données a été automatisé grâce à un pipeline, incluant l’encodage des variables catégorielles via OneHotEncoder et la standardisation des variables numériques avec StandardScaler. Cela a permis une préparation homogène des données et a évité les fuites de
données. 

2- Modélisation avec plusieurs algorithmes : Quatre modèles ont été évalués 

- Régression Logistique comme modèle de référence
  
- Arbre de Décision
  
- Forêt Aléatoire
  
- AdaBoost 
  
3- Optimisation des hyperparamètres avec GridSearchCV : Chaque modèle a été affiné à l’aide de GridSearchCV, en explorant diverses combinaisons d'hyperparamètres avec une validation croisée pour éviter le sur-ajustement et maximiser la performance.

4- Évaluation des modèles avec plusieurs métriques : Les modèles ont été évalués à l'aide de plusieurs métriques comme l'accuracy, le F1-score, la matrice de confusion, et la courbe ROC & AUC, permettant ainsi une analyse complète et fiable de leurs performances.

5- Visualisation des résultats : Des graphiques ont été utilisés pour illustrer les résultats, incluant la matrice de confusion, les courbes ROC, l’importance des variables, et les graphiques SHAP pour mieux comprendre et expliquer les décisions prises par les modèles.
  
- Résultat

Logistic Regression : 

Accuracy (87,64 %) : Prédiction correcte dans 87,64 % des cas. Le modèle est généralement fiable, mais quelques erreurs subsistent. 

F1-score (0.92) : Bon équilibre entre précision et rappel, indiquant une solide performance pour classer les électeurs dans les bonnes catégories. 

AUC (0.91) : Excellente capacité à différencier les classes. 

Decision Tree :

Accuracy (87 %) : Moins précis que la régression logistique. 

F1-score (0.91) : Reste élevé malgré l'accuracy plus faible.
        
AUC (0.75) : Moins performant pour différencier les classes. 


Random Forest :

Accuracy (88,28 %) : Le plus précis des modèles.

F1-score (0.93) : Excellente gestion de la précision et du rappel.

AUC (0.92) : Très bonne capacité à faire des distinctions claires entre les classes.

AdaBoost :

Accuracy (86,84 %) : Moins élevé que Random Forest, mais toujours bon.

F1-score (0.9204) : Bon équilibre entre précision et rappel.

AUC (0.87) : Moins performant que les autres modèles.


Random Forest est le modèle le plus performant, avec la meilleure accuracy et AUC, ce qui en fait le meilleur choix pour prédire les résultats. Logistic Regression suit de près et peut être une alternative simple mais efficace. 
 
- Lien github : https://github.com/VivoAZ/VF-Projet-Datagong

### Projet 5 : Projet de scoring des clients d'une entreprise de télécommunication

- Résumé

Développement d’un modèle de scoring prédictif du churn client dans le secteur des télécommunications à partir de données comportementales et démographiques. L’objectif était d’identifier les clients à risque de résiliation afin d’orienter les actions marketing ciblées et améliorer la rétention. Le modèle final repose sur un Gradient Boosting Classifier avec une explicabilité assurée via SHAP. 

- Approche méthodologique

Feature engineering : création de nouvelles variables dérivées, encodage des variables catégorielles (OneHot + Ordinal).

Sélection des variables : filtrage via SelectKBest (chi²) pour ne conserver que les 20 meilleures.

Prétraitement & pipeline : pipeline scikit-learn combinant encodage, standardisation et classification.

Modélisation : entraînement et évaluation de plusieurs modèles, avec métriques (F1, AUC, précision).

Explicabilité : analyse de l’importance des variables via SHAP pour l’interprétabilité du modèle. 

Exportation du fichier csv de tous les clients avec les niveaux de risque de churn et les recommandations marketing 

- Résultat

| Modèle                  | Accuracy | F1-score (classe 1) | AUC      |
| ----------------------- | -------- | ------------------- | -------- |
| **Logistic Regression** | 0.80     | **0.59**            | 0.83     |
| **Random Forest**       | 0.78     | 0.55                | 0.81     |
| **Gradient Boosting**   | 0.79     | 0.57                | **0.84** |
| **SVM**                 | 0.78     | 0.52                | 0.79     |
| **KNN**                 | 0.76     | 0.53                | 0.77     |

Commentaire analytique
Logistic Regression affiche un excellent compromis entre simplicité, F1-score et AUC, ce qui en fait un modèle de référence solide.

Gradient Boosting obtient le meilleur score AUC (0.84), indiquant une forte capacité de discrimination, mais avec un léger recul en F1 par rapport à la régression logistique.

Les modèles Random Forest et SVM présentent une performance correcte, mais avec un recall plus faible sur la classe 1, essentielle pour ce projet (détection des clients potentiellement "upsellables").

KNN est le moins performant, aussi bien en recall qu’en F1-score.

Conclusion
Malgré une performance équilibrée de la régression logistique, le choix final se porte sur le Gradient Boosting à cause de son score AUC. En effet, contrairement à la RL qui est un modèle linéaire et qui présente des limites en matière de capture des relations complexes, le gradient boosting quant à lui est non linéaire et défit donc cette limite. Ce qui constitue un facteur très important au vu des données et la problématique de notre étude. Aussi, ce modèle donne une meilleure flexibilité pour ajuster le seuil selon le besoin métier. 

## Compétences techniques et outils   

- Langages de programmation : Python, SQL
- Bibliothèques et frameworks : Pandas, Matplotlib, Seaborn, Plotly, Missingno, Scikit-learn
- Outils : Git, VS Code, Colab, Jupyter Notebook, Power BI, Excel 

## Contacts  

- Lien profil LinkedIn : www.linkedin.com/in/marc-azian-data-scientist 
- Addresse email : marcazian77@gmail.com 
