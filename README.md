# rl-mecanics

> Plateforme communautaire dédiée aux mécaniques et au freestyle sur Rocket League : wiki, profils joueurs, forum, etc...

---

## 🎯 Objectif
> Le projet est composé de plusieurs repository, un public, et plusieurs repo privé.

---

Créer un site web évolutif autour du **freestyle Rocket League**, avec :
- Un **wiki** collaboratif (mécaniques, joueurs, teams…)
- Un **espace communautaire** (classements, tournois, soumission de records)
- Une architecture ouverte aux extensions : **bot Discord**, **plugin BakkesMod**, **app mobile**, etc.

---

## 🧱 Dépôts du projet

### 🔹 `freestyle-hub-frontend` (privé)
- **Techno :** React ou Next.js (JS/TS)
- **Contenu :** Interface principale du site
- **Fonction :** Affiche le contenu wiki + fonctionnalités interactives
- **Fait appel à :** `strapi-backend` & `custom-api`

---

### 🔹 `freestyle-hub-cms` (privé)
- **Techno :** Strapi (Node.js, JS/TS)
- **Contenu :** Wiki, profils joueurs/teams, mécaniques
- **Fonction :** CMS avec interface admin + API REST publique
- **Base de données :** PostgreSQL

---

### 🔹 `freestyle-hub-api` (privé)
- **Techno :** NestJS (TypeScript)
- **Contenu :** Tournois, classements, vidéos, soumission, logic métier
- **Fonction :** API REST personnalisée pour les fonctionnalités avancées
- **Scalable pour :** bots, plugins, apps externes

---

## 🗂 Structure globale


:package: freestyle-hub-frontend     → Interface utilisateur
:package: freestyle-hub-cms          → Wiki / CMS via Strapi
:package: freestyle-hub-api          → Backend custom (tournois, vidéos, etc.)
:globe_with_meridians: frontend <--> strapi + api
