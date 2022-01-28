# Commandes de base

Ici, nous allons voir quelques commandes de bases indispensables à connaitre pour bien démarrer sur un environnement linux



## Les commandes


- `cd` (**change directory**) : permet de naviguer entre les différents répertoires
```shell
    cd .. # va dans le repertoire parent
    cd monDossier # va dans le repertoire monDossier
    cd / # va à la racine du serveur
    cd ~ # va dans le repertoire courant de l'utilisateur
    cd # va également dans le repertoire courant de l'utilisateur
```

- `pwd` (**print work directory**): permet d'imprimer à l'écran le chemin du repertoire dans lequel on se situe

```shell
pwd
/home/ecole

```

- `ls` : permet de lister le contenu d'un repertoire

```
ls -l
drwxr-xr-x  2 root root   4096 Jan 22 06:25 backups
drwxr-xr-x 15 root root   4096 Jan  5 22:36 cache
drwxrwxrwt  2 root root   4096 Jan  4 06:25 crash
drwxr-xr-x 47 root root   4096 Dec 26 16:54 lib
drwxrwsr-x  2 root staff  4096 Oct 11 08:39 local
lrwxrwxrwx  1 root root      9 Oct 14 11:59 lock -> /run/lock
drwxrwxr-x 12 root syslog 4096 Jan 23 00:00 log
drwxrwsr-x  2 root mail   4096 Oct 14 11:59 mail
drwxr-xr-x  2 root root   4096 Oct 14 11:59 opt
lrwxrwxrwx  1 root root      4 Oct 14 11:59 run -> /run
drwxr-xr-x  5 root root   4096 Oct 14 12:10 snap
drwxr-xr-x  4 root root   4096 Oct 14 12:00 spool
drwxrwxrwt  6 root root   4096 Jan 25 15:39 tmp
drwxr-xr-x  4 root root   4096 Dec 26 16:27 www

```

- `man` (**manual**) : affiche le manuel d'utilisation d'une commande

```shell
 man ls
 man cd
```

- `mkdir` (**make directories**) : permet de créer un repertoire

- `whoami` (**who am i**) : donne le nom de l'utilisateur courant

-`clear`: permet de vider l'écran du terminal

- `rmdir` (**remove directory**): permet de supprimer un repertoire s'il est vide

- `rm` (**remove**): permet de supprimer des fichiers ou repertoires

- `mv` (**move**): permet de déplacer ou renommer un fichier/repertoire

- `cp` (**copy**): permet de copier un fichier/repertoire

- `touch`: permet de créer un fichier, mais également de modifier le **timestamp** d'un fichier

- `cat` : permet de lire le contenu d'un fichier et de le renvoyer en sortie

- `less` : permet de lire le contenu d'un fichier page par page.

- `head` : permet d'imprimer à l'écran les 10 premières lignes (par défaut) d'un fichiers ou d'une sortie standard

- `history` : permet de récupérer l'historique des commandes tapées précédemment

- `echo`: permet d'afficher le contenu des données passée en argument, exemple: variables, chaîne de caractères …
```shell
    echo 'Hello World'
    Hello World
```

- `date` : permet de récupérer la date du serveur

- `wc`(**word count**): permet de compter le nombre de lignes, de mots ou de caractère dans un fichier


# les options sur les commandes

Dans la plupart des cas, les commandes ne s'utilisent pas seule, 

### Exemples

#### Exemple 1

Je souhaite supprimer un repertoire non vide, je vais devoir utiliser l'option -r pour supprimer l'ensemble des données en mode recursive, si vous ne passez pas cette option, vous ne pourrez pas supprimer un repertoire vide

```shell
rm -r monDossier

```

#### Exemple 2







