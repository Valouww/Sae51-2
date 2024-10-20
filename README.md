# Sae51-2 - Guide d'utilisation et de fonctionnement

## Rappel de l'objectif

Produire un Dockerfile/Docker-compose qui met un oeuvre une situation simple de collecte de logs, basée sur une des solutions existantes.

## Description

Pour ce projet, nous avons opté pour la stack Grafana, Loki et Alloy. Pourquoi ? Parce que c'est l'outil le plus simple à prendre en main et qu'il répond parfaitement à nos besoins actuels ainsi qu'à nos connaissances. Il nous permet de centraliser nos logs rapidement et efficacement, sans avoir à nous plonger dans des configurations complexes.
De plus, nous avons mis en place un docker Nginx afin de traiter et visualiser les logs de ce serveur Nginx.

## Fonctionement

Notre docker-compose lance 4 dockers dont leur rôle est:
* Grafana est utilisé pour visualiser les logs via un tableau de bord.
* Loki stocke les logs et les expose à Grafana.
* Alloy est configuré pour collecter les logs de fichiers locaux et les envoyer à Loki.
* Un serveur Nginx génère des logs qui sont collectés et analysés.

Afin de mieux comprendre, voici un schéma de leur fonctionnement :
![Diagram_Fonctionnement](Diagram_Fonctionnement.png)
