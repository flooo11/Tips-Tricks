#GIT


Mise en place de glg1 et autres: Texte à ajouter en fin de fichier -->  /etc/profile.d/aliases.sh
alias glg1="git log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all"
alias glg2="git log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold cyan)%aD%C(reset) %C(bold green)(%ar)%C(reset)%C(bold yellow)%d%C(reset)%n'' %C(white)%s%C(reset) %C(dim white)-%an%C(reset)' --all "
alias glg="git log --graph --abbrev-commit --decorate --date=relative --all"


Commandes

depuis la branche_destination
git  merge branche_source --ff-only



Ressources : 
http://www.dynamic-mess.com/developpement/git-merge-fast-forward-rebase-culture-git/

Lister les branches : 
$ git branch

Aller dans la branche master : 
$ git checkout master

Supprimer la branche distante (stage1 la branche à supprimer) :
$ git push origin --delete stage1

Supprimer la branche locale (stage1 la branche à supprimer) :
$ git branch -d stage1

Mettre des fichiers modifié de coté (stash) :
http://dauzon.com/lire-Git-Utiliser-git-stash-41

----------------------------------------------------------------------------------------------------------------------------------------------------------
Mise en place du git pour un projet existant coté local à intégrer dans un Git
Creer le Git coté serveur ainsi que la branche souhaitée

Sur la machine locale dans le projet
git init
git remote add origin https://toto.visualstudio.com/DefaultCollection/toto.PowerPlateForm/_git/SchemaComptage
git push -u origin MBa-Dev --force

Ici nous avons une branche serveur existante MBa-Dev et un repo se nommant SchemaComptage
--force détruit l'existant coté serveur git

vérifier coté serveur que le code est bien présent. 
----------------------------------------------------------------------------------------------------------------------------------------------------------

Nettoyage GIT
https://gist.github.com/Thithip/cfc058442e4e052aa817
