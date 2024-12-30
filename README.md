# Data Scientist Junior  

## Profil  
Marc AZIAN 

Data Scientist Junior, formé par DATAGONG, un centre de formation international réputé basé en France et piloté par des experts en Data Science. Membre actif de l’association 10 000 Codeurs, je suis passionné par l’application de la science des données au domaine du marketing, où j’ai déjà mené plusieurs projets que vous pouvez découvrir ci-dessous.

Ma spécialité réside dans l’utilisation de Python, et je suis en cours d’apprentissage de SQL pour enrichir mes compétences. Je m'intéresse également aux frameworks comme TensorFlow et PyTorch afin de développer mes connaissances en apprentissage profond. Mon adaptabilité et ma capacité à maîtriser rapidement de nouveaux outils technologiques sont des atouts clés de mon parcours.

Actuellement, je travaille sur un projet de classification binaire visant à prédire les résultats électoraux, un projet majeur dans le cadre de ma soutenance de fin de formation. Découvrez l’ensemble de mes réalisations et projets dans ce portfolio.    

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

## Compétences techniques et outils   

- Frameworks : Scikit-learn
- Outils de visualisation : Matplotlib, Seaborn, Plotly, Missingno 
- Outils de gestion des données : Pandas

## Contacts  

- Lien profil LinkedIn : www.linkedin.com/in/marc-azian-data-scientist 
- Addresse email : marcazian77@gmail.com 
