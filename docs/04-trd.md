# TRD — Stack et services

## Frontend

- HTML5 + CSS3 (styles en ligne + un bloc `<style>` global) + JavaScript vanilla (ES5/ES6).
- Aucun framework, aucun bundler, aucun gestionnaire de paquets : pas de `package.json`, pas de `node_modules`, pas d'étape de build.
- Un seul fichier `index.html` à la racine, plus un dossier `assets/` pour les images (avec variantes WebP + `srcset`) et `assets/fonts/` pour les polices auto-hébergées (Fraunces, Work Sans).

## Hébergement et déploiement

- **Hébergement** : GitHub Pages.
- **Dépôt** : `vincentmatray-69600/mariage-Laly-Vincent`, branche `main`, contenu servi depuis la racine.
- `.nojekyll` présent : désactive le traitement Jekyll de GitHub Pages (site statique pur).
- **Déploiement** : automatique à chaque `push` sur `main`, via l'action GitHub "pages build and deployment". Pas de CI personnalisée, pas d'étape de test automatisé.
- **Domaine** : domaine personnalisé configuré via le fichier `CNAME` à la racine. Le site est servi sur `https://www.mariage-laly-vincent.fr/` (adresse par défaut `vincentmatray-69600.github.io/mariage-Laly-Vincent/` toujours active en parallèle, via les réglages GitHub Pages).

## Ce qui n'existe pas

- Pas de backend, pas de serveur applicatif.
- Pas de base de données.
- Pas d'API.
- Pas d'authentification ni de compte utilisateur.
- Pas d'outil d'analytics ni de tracking (cohérent avec `confidentialite` dans le site : aucun cookie déposé).

## Services externes liés

Services non intégrés au site (pas d'appel API, pas de clé, pas de SDK) : simples liens sortants ou polices chargées.

| Service | Rôle | Intégration |
|---|---|---|
| Google Calendar | Bouton "Ajouter au calendrier — Google" | Lien `calendar.google.com/calendar/render?...` pré-rempli |
| — (aucun service, fichier statique) | Bouton "Ajouter au calendrier — Apple" | Fichier `assets/mariage-laly-vincent.ics` servi directement par le site, mêmes informations que l'événement Google Calendar |
| Google Maps | Boutons "Itinéraire" | Liens `google.com/maps/search/?...` |
| Google Forms | Formulaire RSVP | Lien externe vers un formulaire existant, réponses non visibles depuis le site |
| Google Drive | Album photo du mariage | Lien externe, ajouté après le mariage dans la variable `DRIVE_URL` du code — [EN ATTENTE, cf. PRD] |
| Google Search Console | Suivi du référencement (indexation, sitemap, données structurées) | Outil de supervision externe, aucune intégration dans le code du site hormis le fichier de vérification `googleb3fba4beb249fbe8.html` et `sitemap.xml` |
