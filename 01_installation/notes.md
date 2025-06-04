# 🧾 Résumé du TP Docker

Ce TP avait pour objectif de découvrir et manipuler Docker ainsi que Docker Compose à travers plusieurs étapes progressives.

## Étape 1 – Installation
- Docker et Docker Compose ont été installés sur Ubuntu.
- Vérification avec `docker --version` et `docker compose version`.

## Étape 2 – Premiers tests
- Exécution de conteneurs simples (`hello-world`, `ubuntu bash`).
- Observation des images (`docker images`) et conteneurs (`docker ps -a`).
- Exécution d’un serveur NGINX avec `docker run`.

## Étape 3 & 4 – Serveur web
- Création d’un fichier `index.html`.
- Méthode 1 : le serveur NGINX affiche la page via un volume (`-v`).
- Méthode 2 : utilisation de `docker cp` pour copier le fichier dans le conteneur.
- Différences observées documentées dans les fichiers `.md`.

## Étape 5 – Image personnalisée
- Création d’un `Dockerfile` basé sur `nginx`.
- Intégration directe de `index.html` dans l’image.
- Build avec `docker build` et exécution de l’image personnalisée.

## Étape 6 – Base de données avec Docker Compose
- Déploiement de deux services : `mysql:5.7` et `phpmyadmin`.
- Accès via navigateur à phpMyAdmin (`http://localhost:8082`).
- Configuration automatique de la base `mi_base`.

## Étape 7 – Isolation réseau
- Trois services (web, app, db) et deux réseaux (`frontend`, `backend`).
- Vérification des pings entre conteneurs :
  - `web` ↔ `app` ✅
  - `app` ↔ `db` ✅
  - `web` ✖ `db` ❌ → isolation confirmée.

---

✅ Toutes les étapes ont été versionnées avec Git (`git commit`, `git push`) pour montrer la progression.

📦 Le dossier final contient : fichiers `.md`, `Dockerfile`, `docker-compose.yml` et les logs.
