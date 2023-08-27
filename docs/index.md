## How to Deploy on Github Pages

27 August 2023

* create new repository on github
* push project to github with origin branch name
* use built in deploy to github page
```shell
    $ mkdocs gh-deploy
```
* if your account is free, make sure that your repository is public so you can use github pages for free too.
  * on your repository, go to 
```
  setting > Pages > Build and deployment > Branch > gh-pages > /root > save
```
* your site has deploy on `<your github>/<your repository>`
* for updating, you can add your update script / docs > commit and run again deploy to github pages `mkdocs gh-deploy`