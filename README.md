# React CI 

[[_TOC_]]

## Architecture du projet

Partie front, en **React**, d'un projet plus complexe.



## Continuous Integration - Fonctionnement

Chaque `git push` déclenche une pipeline **Travis CI**, définie dans le fichier `.travis.yml`.

Les tâches exécutées : 

- Build une image docker, à partir du `Dockerfile`
- Pousse l'image sur **DockerHub** 
- Lance une analyse de code avec **SonarCloud** (configuration dans `sonar-project.properties`)
- Récupère l'image et lance les tests React.

---

Un récapitulatif est disponible sur Github, à côté de chaque commit.

Pour plus d'infos :

- [Lien du Travis](https://travis-ci.org/github/remi95/React-CI)

- [Lien du SonarCloud](https://sonarcloud.io/dashboard?id=remi95_React-CI) 
- [Lien du DockerHub](https://hub.docker.com/repository/docker/arnaudlfn/front)

