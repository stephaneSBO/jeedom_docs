# Shelly

## Présentation

Ce plugin permet d'interconnecter Jeedom avec des modules Shelly.

Il permet de commander les relais ou fonctions des différents modules Shelly. Ainsi que récupérer les informations (statut, consommation, couleur ...)

Shelly sont une série de produits fonctionnant en Wifi, ils proposent une application mobile pour leur configuration ainsi qu'un cloud pour leur utilisation à distance.

Le plugin Jeedom utilise une API locale au module directement, pas besoin du cloud.

https://shelly.cloud/

## Configuration

Le plugin ne comporte pas de configuration générale.

Sur chaque équipement il faut configurer :

  - l'adresse IP

  - le type

Les commandes sont créées automatiquement à la sauvegarde. POur chaque type, les commandes infos et actions disponibles seront disponibles.

Pour les relais, sur sauvegarde de l'équipement Jeedom va allez configuré chaque "push url" du Shelly pour recevoir en temps réel les changements d'état.

Dans le cas du Shelly 1, si le bouton est configuré en "Detached type", alors Jeedom en plus pendant la sauvegarde équipement va créer une commande représentant le bouton et qui sera liée au "push url" du bouton. Permettant ainsi son utilisation en plus du relais comme bouton poussoir dans Jeedom.

## FAQ

> Est-ce que le plugin s'appuie sur des API tiers ?

Oui, le plugin utilise l'API locale des modules Shelly, pas besoin du cloud ou autre.


## Changelog

[Voir la page dédiée](changelog.md).
