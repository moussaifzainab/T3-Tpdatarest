# TP 3 – Service Web REST avec Spring Data REST et Spring Boot

Ce projet met en œuvre un service web REST basé sur Spring Data REST. L’objectif est d’exposer automatiquement des opérations CRUD sur les entités Article et Categorie, sans écrire de contrôleurs. Spring Data REST génère les endpoints à partir des Repository, et la base de données utilisée est H2.

## Objectifs du TP

* Exposer un modèle métier via l’API Spring Data REST.
* Générer les opérations CRUD automatiquement à partir des interfaces JPA.
* Utiliser une base H2 embarquée.
* Tester les endpoints avec Postman et Swagger UI.
* Consulter la documentation OpenAPI générée automatiquement.

## Démarrage du projet

Après avoir cloné le dépôt, exécuter :

```
mvn spring-boot:run
```

L’application démarre sur le port 8080.

## URLs principales

* Console H2 : [http://localhost:8080/h2](http://localhost:8080/h2)
* Liste des articles : [http://localhost:8080/ecommerce](http://localhost:8080/ecommerce)
* Article par ID : [http://localhost:8080/ecommerce/{id}](http://localhost:8080/ecommerce/{id})
* Catégories : [http://localhost:8080/categories](http://localhost:8080/categories)
* Recherche par catégorie :
  [http://localhost:8080/ecommerce/search/byCategorie?categorie=CATEGORIE_1](http://localhost:8080/ecommerce/search/byCategorie?categorie=CATEGORIE_1)
* Documentation OpenAPI :
  [http://localhost:8080/api-docs](http://localhost:8080/api-docs)
* Swagger UI :
  [http://localhost:8080/swagger-ui/index.html](http://localhost:8080/swagger-ui/index.html)

## Données de test

À l’exécution, la base H2 est initialisée avec plusieurs catégories (CATEGORIE_1, 2, 3) et des articles associés.

## Dépôt GitHub

[https://github.com/moussaifzainab/T3-Tpdatarest](https://github.com/moussaifzainab/T3-Tpdatarest)

