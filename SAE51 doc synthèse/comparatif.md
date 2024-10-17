# SAE51
**18/09/24**
***Valentin DAVID
Corentin CHRETIEN***

## Objectif

Produire un document de synthèse présentant les solutions libres (Loki, Elastic, Graylog) de centralisation et présentation de logs, nous donnerons aussi leurs points-clé (features, communauté associée, etc.) et leurs avantages et inconvénients respectifs :
``
ø     |Loki   |Elastic   | Graylog  |
 |------|-------|---|---|
Communauté Github | 7k3+ commit   | 79K+ commit | 25k+ commit   | 
Facilité de mise en place | Très facile  | Difficile  | Facile  |   
Filtrage des logs | Basique  | Puissant  |Puissant   |     
Problème connu | Lent sur gros volume  | Node setup  | Gestions indices   |   
Scalabilité |Faible   | Haute  |  Haute |   
Modèle eco|Gratuit   | Gratuit  |  Gratuit |
Conso ressource| Faible  | Gourmand  |Gourmand   |   
Stockage Data | Cloud |Gourmand   | Gourmand  |

``
Pour suivre l'activité des 3 solutions nous avons choisis de comparer l'activité sur Github. La taille des commits est bien entendu variable mais donnes tout de même une indication de l'implication des utilisateurs sur la solution.

## Sources
https://stackshare.io/stackups/graylog-vs-loki
https://stackshare.io/stackups/elasticsearch-vs-graylog
https://signoz.io/blog/loki-vs-elasticsearch/
https://github.com/





## Graylog
est une solution mature, complète et personnalisable, idéale pour les entreprises qui recherchent une plateforme de gestion de logs robuste et intuitive. Elle offre une large gamme de fonctionnalités et une communauté active.

## Loki
 est une solution légère et spécialisée dans la collecte et la visualisation de logs, particulièrement adaptée aux environnements cloud-native et aux équipes qui utilisent déjà Grafana. Elle est idéale pour ceux qui cherchent une solution simple et efficace.
 
## Elastic
 (avec Elasticsearch comme composant central) est une suite complète d'outils pour la recherche, l'analyse et la visualisation de données. Elle offre des performances élevées et une grande flexibilité, mais peut nécessiter une configuration plus complexe. Elle est particulièrement adaptée aux entreprises qui ont besoin d'une solution unifiée pour gérer différents types de données.

## Conclusion

Notre choix entre Graylog, Loki et Elastic dépendra en grande partie de nos besoins spécifiques et de la quantité de ressource que nous avons à disposition.

Graylog utilise une interface plus simple et agréable qu'Elastic Stack.
Cependant, il utilise Elastic Search dans son fonctionnement et cela ne nous convient pas au vu de la configuration nécéssaire.
Elasticsearch indexe toutes les données dans chaque champ, et chaque champ indexé dispose d'une structure de données dédiée et optimisée. Une configuration minutieuse est nécessaire ainsi qu'une haute compréhension.
Pour la SAE51, nous avons opté pour Loki. Pourquoi ? Parce que c'est l'outil le plus simple à prendre en main et qu'il répond parfaitement à nos besoins actuels. Il nous permet de centraliser nos logs rapidement et efficacement, sans avoir à nous plonger dans des configurations complexes.



