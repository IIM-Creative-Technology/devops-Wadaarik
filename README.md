# Portfolio Nicolas Boudier

Le portfolio utilise Github action puis Heroku.
Le projet est commit sur 2 branches :
  - La première sert de commit de pré-prod
  - La seconde sert de commit de prod

## Détails

  - Le projet est développé sous Vuejs.
  - preprod.yaml est le fichier permettant de push ses commits vers la branche de préprod.
  - master-prod.yml est le fichier permettant de push ses commits vers la branche de prod.
  - static.json : permet de spécifier une racine active différente pour le répertoire de l'application
  
### Buildpacks heroku

  - nodejs
  - https://github.com/heroku/heroku-buildpack-static

## Commandes

  - npm install -g @vue/cli : va installer le package en global sur le projet pour vuejs
  - vue create my-app : créer l'application vue
  - vue ui (facultatif) : permet d'ouvrir l'interface de gestion de projet vue
  - git init
  - git commit -m "first commit"
  - git branch -M master/preprod
  - git remote add origin https://github.com/repo/project.git
  - git push -u origin master
