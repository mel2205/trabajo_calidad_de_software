## Flujo de trabajo GitFlow

El flujo de trabajo GitFlow es una metodología comúnmente utilizada en el desarrollo de software para gestionar las ramas en un proyecto Git. A continuación, se detallan los comandos clave que debes utilizar para seguir el flujo de trabajo GitFlow en este proyecto:

### Crear la rama de desarrollo desde la rama master:

```bash
git checkout -b develop master

git checkout -b develop master
git checkout -b feature/x develop
git checkout develop
git merge --no-ff feature/x
git branch -d feature/x
git checkout -b release/x develop
git checkout master
git merge --no-ff release/x
git checkout develop
git merge --no-ff release/x
git branch -d release/x
git checkout -b hotfix/x master
git checkout master
git merge --no-ff hotfix/x
git checkout develop
git merge --no-ff hotfix/x
git branch -d hotfix/x



