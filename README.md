# gen018-e2e-mw9hljpp

Projet généré par AIOps.

## Stack

- java-spring-boot 4.1.0
- Java 21
- Dépendances : web, actuator

## Build et lancement

```bash
./mvnw clean install
./mvnw spring-boot:run
docker compose up -d
```

L'application écoute sur le port 8080.

Healthcheck : `/actuator/health`.

## Outils

- docker
- github-actions

## Branches

- Modèle : git-flow
- Branche de déploiement : `main`

## Intégration continue

Le pipeline est décrit dans `.github/workflows/ci.yml`.

---

Généré par AIOps — voir `.aiops/manifest.json`.

## 🧭 Pourquoi ces choix

- **Docker** — emballe l'application et ses dépendances dans une image : elle tourne à l'identique sur ton poste et sur le serveur.
- **GitHub Actions** — lance le build et les tests automatiquement à chaque push : tu sais immédiatement si un changement casse le projet.
- **Branches (Git Flow)** — `develop` reçoit le travail en cours, `main` ne reçoit que du validé : les livraisons restent isolées du développement quotidien. `release/*` et `hotfix/*` sont des conventions de nommage à utiliser au besoin, pas des branches créées d'avance.
