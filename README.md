# README - TP Spark

Ce README fournit des instructions sur l'installation de PySpark et sur la manière de transférer des fichiers entre votre PC local et un conteneur Docker lors de la réalisation de ce TP Spark.

## Installation de PySpark

1. Depuis votre terminal (CMD), exécutez la commande suivante pour installer PySpark en utilisant Docker :
2. Une fois le téléchargement terminé, vérifiez sur Docker Desktop que :
- Une image de PySpark est créée avec le nom `jupyter/pyspark-notebook`.
- Un conteneur PySpark est lancé.

3. Copiez le dernier lien (par exemple, `127.0.0.1:8888/lab?token=xxx`) sur votre navigateur. Cela lancera Jupyter Notebook, vous permettant d'expérimenter PySpark. Notez que vous devez garder votre terminal ouvert avant de quitter votre environnement Jupyter.

Vous disposez maintenant d'un environnement Jupyter Lab avec PySpark préconfiguré, fonctionnant dans un conteneur Docker.

## Transfert de fichiers

1. Copiez le Jupyter Notebook (`.ipynb`) et le jeu de données (`.csv`) depuis votre PC local vers le conteneur. Utilisez la commande suivante dans un autre terminal (CMD) :

2. Pour trouver le nom du conteneur, ouvrez Docker Desktop et vérifiez le nom affecté à votre conteneur PySpark.

3. Pour trouver le chemin où mettre les fichiers sur le conteneur, connectez-vous au niveau du conteneur depuis un terminal avec la commande :

   Puis, utilisez la commande `pwd` depuis le bash du conteneur. Cela vous donnera le chemin (le nom affecté à votre home).
Exemple : docker cp Spark-SQL.ipynb hardcore elbakyan:/home/jovyan/work


## Lors de la réalisation de ce TP

- Assurez-vous de sauvegarder régulièrement vos fichiers de travail dans le conteneur.
- Suivez les instructions données dans le TP pour les exercices et les tâches à accomplir.
- Profitez de l'environnement Jupyter Lab préconfiguré avec PySpark pour expérimenter et apprendre.
- N'hésitez pas à consulter la documentation officielle de PySpark pour plus d'informations et de ressources utiles.

## A la fin du TP

A la fin du TP, enregistrez le travail effectué dans le conteneur sur votre PC (en local). Pour récupérer, en local sur votre PC, les fichiers que vous avez créés sur votre conteneur, utilisez la commande suivante (depuis CMD) : docker cp nom_container:chemin/dossier/dans/le/container chemin_vers_dossier_local




