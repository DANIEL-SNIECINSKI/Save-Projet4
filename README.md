# Save-Projet4
Save Projet4 Formation OC

PROJET VALIDÉ
Automatisez la publication sur votre blog freelance
50 heures
Mis à jour le mardi 2 juillet 2019
Scénario

Vous êtes freelance, et vous aimeriez augmenter votre visibilité, faire partager vos expériences professionnelles, et parler de votre code. Vous vous dites : “Damned, mais bien sûr, je devrais tenir un blog !”.

Cependant, vous ne voulez pas de Wordpress, ni même de passer trop de temps à coder votre site. Vous voulez écrire vos articles simplement, si possible dans la même syntaxe que la documentation.

Comme vous aimez automatiser tout ce qui vous entoure, vous aimeriez automatiser tout ce qui se passe entre la rédaction d'un article, et sa publication.

Vous disposez désormais de votre environnement de travail en local, vous allez donc pouvoir installer votre premier outil d’intégration continue, le très complet Gitlab.

Ainsi, vous pourrez à la fois disposer de votre propre dépôt de source, local et privé, et créer facilement vos premiers "pipelines" d'automatisation.

La mission que vous vous fixez est la suivante :

Vous voulez écrire vos articles en Markdown
Vous voulez utiliser un outil qui génère un site web statique à partir des fichiers Markdown, comme par exemple Pelican
Vous allez versionner vos articles avec Gitlab
Vous construisez votre site statique à chaque “push”
Vous voulez pouvoir le déployer sur la partie hébergement statique de Github.
 Belle ambition ! À vous de jouer !

Instructions :
Installer d’abord Gitlab dans votre machine virtuelle
Installer également Pelican dans votre machine virtuelle
Créez votre répertoire pour Pelican, et versionnez le avec Gitlab
Prenez en main Pelican et générez votre premier “hello world”
Créez votre .gitlab-ci.yml pour automatiser le processus
 

Livrables attendus
Dans un dossier nommé “Projet_04_Nom_Prenom”, vous mettrez à disposition de votre mentor :

Un répertoire nommé “blog”, qui contiendra :

les fichiers nécessaires au fonctionnement de Pelican
Un fichier .gitignore pour ne versionner que les sources et non les articles générés
Un fichier de déploiement .gitlab-ci.yml qui permet
De générer les articles à chaque commit
De déployer le code source manuellement
Soutenance (15-20min)
A l'oral, en partageant votre écran au mentor, vous présenterez d’abord votre installation de Gitlab. Vous lui montrerez les différents compte que vous avez créés, ainsi que votre projet “blog”votre fichier.

Le mentor vous demandera de procéder manuellement à la transformation d’un de vos articles en markdown, puis html, puis visualisation dans un navigateur.

Enfin, toujours en partage d’écran, vous ferez la démonstration des différentes étapes de votre déploiement automatisé, en expliquant le fonctionnement de votre fichier .gitlab-ci.yml

La soutenance se déroule comme suit :

La présentation de votre installation de Gitlab, avec questions et réponses : 10 min
La présentation de votre installation de Pelican, avec question et réponses : 10 min
La démonstration de votre pipeline d’automatisation, avec question et réponses : 10 min
Le mentor prendra 5 minutes à la fin de votre "soutenance" pour débriefer avec vous.
 

 

Compétences évaluées
Mettre en place les outils nécessaires à l’automatisation du cycle de vie des applications
Mettre en place une chaine d'intégration continue pour automatiser les déploiements
