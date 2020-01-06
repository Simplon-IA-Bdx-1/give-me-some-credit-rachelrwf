# Compétition KAGGLE : Give Me Some Credit

[Lien de la compétition Kaggle : Give Me Some Credit](https://www.kaggle.com/c/GiveMeSomeCredit)

## Préambule

Ce projet a été réalisé dans le cadre de la formation de développeur·se data IA (Microsoft/Simplon Bordeaux) pour ***une première approche sur les traitements des données*** (features).
Le but a été :
- d'utiliser les APIs BIGML et Kaggle
- découvrir sklearn (les graphiques) et XGBoost
- réaliser des learning curves, une matrice de confusion, auc, roc


## Prérequis

Il va vous falloir :
* un compte [BigML](https://bigml.com/) et créer un nouveau projet
* un compte [Kaggle](https://www.kaggle.com/)
* créer un dossier "data" là où vous sauvegarderez vos fichiers csv


## Démarrer l'environnement de développement Jupyter

Nous utiliserons un environnement Jupyter fourni par un conteneur Docker. L'image utilisée est définie par le [Dockerfile](docker/Dockerfile) fourni. Celui-ci est basé sur [handson-ml2](https://github.com/ageron/handson-ml2/tree/master/docker) et il installe les packages Python listés dans [requirements.txt](requirements.txt). Ces fichiers sont à customiser au besoin.

1. Créez un fichier `docker/auth.env` basé sur `docker/auth-sample.env`, qui contiendra vos noms d'utilisateur et clés d'API pour [BigML](https://bigml.com) et Kaggle.
2. A partir du dossier `docker/`, exécutez la commande shell:

    ```bash
    docker-compose up
    ```

## A modifier dans le notebook

Modifier les ids des ressurces par les votres (vous les trouverez sur la plateforme BigML).

```
api= BigML(project='project/id_de_votre_projet')
```
