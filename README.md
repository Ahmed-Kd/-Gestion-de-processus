# Calcul Distribué de la Persistance des Nombres
## Description
Cette application permet de distribuer le calcul de la persistance multiplicative des nombres sur plusieurs machines afin de bénéficier d'une grande capacité de calcul. La persistance multiplicative d'un nombre est le nombre de fois que vous devez multiplier les chiffres d'un nombre jusqu'à obtenir un seul chiffre.

## Fonctionnalités
### Serveur :

Produit et distribue les tâches à exécuter aux workers.
Conserve les informations sur les workers disponibles et leur charge actuelle.
Stocke et enregistre périodiquement les résultats sur le disque.
### Workers :

Se connectent au serveur pour signaler leur disponibilité et indiquer le nombre de tâches qu'ils peuvent exécuter en parallèle.
Exécutent les calculs et renvoient les résultats au serveur.
### Client :

Permet la supervision du système (voir les workers actifs, consulter les résultats, visualiser des statistiques).
Plusieurs clients peuvent se connecter au serveur en même temps.
