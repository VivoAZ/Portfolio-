# Data Scientist Junior  

## Profil  
Marc AZIAN 

Data Scientist en devenir, formé par DATAGONG, un centre de formation international réputé basé en France et piloté par des experts en Data Science. Membre actif de l’association 10 000 Codeurs, je suis passionné par l’application de la science des données au domaine du marketing, où j’ai déjà mené plusieurs projets que vous pouvez découvrir ci-dessous.

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

Le gradient boosting nous a présenté les meilleurs scores à tous niveaux, comparé aux autres modèles. 
  
- Lien github : https://github.com/VivoAZ/Churn-project 

### Projet 2 : Clustering de la clientèle 

- Résumé : 
- Approche :
- Résultat :
- Lien github : https://github.com/VivoAZ/Projet-clustering-/tree/master 

### Projet 3 : Prédiction de prix des maisons 

- Résumé
  
  Ce projet est un jeu de données sur les maisons dans la ville de Boston avec des features capitales. Notre objectif est de prédire le prix des maisons dans cette zone en nous basant sur la relation entre les différentes variables. Nous disposons des variables quantatives et deux variables catégorielles. Le type de machine learning adapté est le ML supervisé.
  
- Approche
  
  Après chargement des données, nous avons procédé à une analyse exploratoire qui nous a conduit aux traitements des valeurs manquantes. A ce niveau, nous avons opté par l'imputation avec la moyenne pour les valeurs numériques puis l'imputation par le mode pour les valeurs catégorielles. Ensuite, nous avons procédé à la visualisons des potentiels outliers parmi nos données et leurs relations avec notre target. Les outliers détectés ont été traités suivant une troncature. Après, nous avons utilité le One Hote Encoding pour encoder les variables catégorielles. Poour finir cette partie, nous avons créer un pipeline qui résume toutes les étapes executées. Enfin, nous avons entraîné plusieurs modèles par cross validation sur notre jeu de train et l'évaluer avec la métrique MAE.     

- Résultat : 2.501 grâce au modèle Gradient Boosting.

  C'est un score acceptable au vu du nombre d'observations que nous disposons et de la relations entre nos variables et la target. Aussi, vu la problématque du métier, c'est un risque très gérable.   
  
- Lien github : https://github.com/VivoAZ/Projet-prediction-de-prix 

## Compétences techniques et outils   

- Frameworks : Scikit-learn
- Outils de visualisation : Matplotlib, Seaborn, Plotly
- Outils de gestion des données : Pandas

## Contacts  

- Lien profil LinkedIn : www.linkedin.com/in/marc-azian-data-scientist 
- Addresse email : marcazian77@gmail.com 
