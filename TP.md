# Intégration Continue - Évaluation 2024
## Séparation du projet en trois dépôts
Téléchargement local du projet initial
Code:
```
git clone https://github.com/DeborahK/Angular-GettingStarted.git
```
Création du dépôt Angular-GettingStarted-APM-Start
Changement de l'URL du dépôt local
Code:
```
git remote set-url origin https://github.com/Vonkuro/Angular-GettingStarted-APM-Start.git
```
Envoi de la branche master sur le nouveau dépôt
Code:
```
git push --force
```
Suppression des dossiers APM-Final et APM-Final-v16
Commit de cette suppression sur la branche master
Code:
```
git add .
git commit -m "fork of Angular-GettingStarted of only the master branch and APM-Start"
git push
```
Création de la branche develop
Code:
```
git checkout -b develop
git push --set-upstream origin develop
```
Répétition de l'opération pour les deux autres dépôts en conservant les codes sources adéquats.
## Installation des outils de build
### Node v14
Installation de nvm sur linux
Code:
```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
```
Installation de node version 14
Code:
```
nvm install 14
nvm use 14
```
### Angular cli
Code:
```
npm install -g @angular/cli
```