# Commandes de base

Ici, nous allons voir quelques commandes de bases à connaitre pour bien démarrer sur un environnement linux



## Les commandes


- `cd` (**change directory**) : permet de naviguer entre les différents répertoires
```shell
    ubuntu@ecole:~$ cd .. # va dans le repertoire parent
    ubuntu@ecole:~$ cd monDossier # va dans le repertoire monDossier
    ubuntu@ecole:~$ cd / # va à la racine du serveur
    ubuntu@ecole:~$ cd ~ # va dans le repertoire courant de l'utilisateur
    ubuntu@ecole:~$ cd # va également dans le repertoire courant de l'utilisateur
```

- `pwd` (**print work directory**): imprime à l'écran le chemin du repertoire dans lequel on se situe

```shell
ubuntu@ecole:~$ pwd
/home/ecole

```

- `ls` : liste le contenu d'un repertoire

```
ubuntu@ecole:~$ ls -l
drwxr-xr-x  2 root root   4096 Jan 22 06:25 backups
drwxr-xr-x 15 root root   4096 Jan  5 22:36 cache
drwxrwxrwt  2 root root   4096 Jan  4 06:25 crash
drwxr-xr-x 47 root root   4096 Dec 26 16:54 lib
drwxrwsr-x  2 root ecole  4096 Oct 11 08:39 local
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
 ubuntu@ecole:~$ man ls
 ubuntu@ecole:~$ man cd
```

- `mkdir` (**make directories**) : permet de créer un repertoire
```shell
ubuntu@ecole:~$ ls -l
total 0
ubuntu@ecole:~$ mkdir folder
ubuntu@ecole:~$ ls -l
total 0
drwxr-xr-x  2 ecole  ecole  64 Jan 28 08:55 folder
```

- `whoami` (**who am i**) : donne le nom de l'utilisateur courant
```shell
ubuntu@ecole:~$ whoami
ubuntu
```

- `clear`: vide l'écran du terminal

- `rmdir` (**remove directory**): Supprime un repertoire s'il est vide

```shell
    ubuntu@ecole:~$ ls -l
    drwxr-xr-x  2 ecole  ecole  64 Jan 28 08:55 folder
    ubuntu@ecole:~$ rmdir folder
    ubuntu@ecole:~$ ls -l
    total 0
```

- `rm` (**remove**): Supprime des fichiers ou repertoires
```shell
    ubuntu@ecole:~$ ls -l
    drwxr-xr-x  2 ecole  ecole  64 Jan 28 08:55 folder
    ubuntu@ecole:~$ rm -R folder
    ubuntu@ecole:~$ ls -l
    total 0
```

- `mv` (**move**): Déplace ou renomme un fichier ou repertoire

```shell
    ubuntu@ecole:~$ ls -l
    drwxr-xr-x  2 ecole  ecole  64 Jan 28 08:55 folder
    ubuntu@ecole:~$ mv folder folder_move
    ubuntu@ecole:~$ ls -l
    total 0
    drwxr-xr-x  2 ecole  ecole  64 Jan 28 08:55 folder_move
```

- `cp` (**copy**): Copie un fichier ou repertoire

```shell
    ubuntu@ecole:~$ ls -l
    total 0
    drwxr-xr-x  2 ecole  ecole  64 Jan 28 08:55 folder
    ubuntu@ecole:~$ cp -r folder copy_folder
    total 0
    drwxr-xr-x  2 ecole  ecole  64 Jan 28 09:15 copy_folder
    drwxr-xr-x  2 ecole  ecole  64 Jan 28 08:55 folder
```

- `touch`: permet de créer un fichier, mais également de modifier le **timestamp** d'un fichier

```shell
    ubuntu@ecole:~$ touch message
    ubuntu@ecole:~$ ls -l
    -rw-r--r--  1 ecole  ecole  0 Jan 28 09:10 message
```

- `cat` : permet de lire le contenu d'un fichier et de le renvoyer en sortie

```shell
    ubuntu@ecole:~$ cat message
    Hello
    Comment
    Allez
    Vous
    ?
```

- `less` : permet de lire le contenu d'un fichier en mode page à page ( pour naviguer vers la page suivante utiliser la touche **f** et pour la précédente **b**)

- `head` : permet d'imprimer à l'écran par défaut les 10 premières lignes d'un fichier ou d'une sortie standard
```shell
ubuntu@ecole:~$ head auth.log
Jan 23 00:02:01 ecole sshd[563664]: Invalid user emilie from 103.253.146.82 port 43590
Jan 23 00:02:02 ecole sshd[563664]: Connection closed by invalid user emilie 103.253.146.82 port 43590 [preauth]
Jan 23 00:02:24 ecole sshd[563666]: Invalid user ftpuser from 106.13.31.93 port 33478
Jan 23 00:02:24 ecole sshd[563666]: Received disconnect from 106.13.31.93 port 33478:11: Bye Bye [preauth]
Jan 23 00:02:24 ecole sshd[563666]: Disconnected from invalid user ftpuser 106.13.31.93 port 33478 [preauth]
Jan 23 00:03:00 ecole sshd[563670]: Invalid user emilie from 103.253.146.82 port 44164
Jan 23 00:03:01 ecole sshd[563670]: Connection closed by invalid user emilie 103.253.146.82 port 44164 [preauth]
Jan 23 00:04:01 ecole sshd[563672]: Invalid user emilie from 103.253.146.82 port 44744
Jan 23 00:04:01 ecole sshd[563672]: Connection closed by invalid user emilie 103.253.146.82 port 44744 [preauth]
Jan 23 00:07:28 ecole sshd[563678]: Invalid user emilie from 103.253.146.82 port 46848
```


- `history` : permet de récupérer l'historique des commandes tapées précédemment

```shell
ubuntu@ecole:~$ history
  ……
  126  ls- l
  127  sudo su
  128  cd /home/
  129  ls
  130  cd /var/www/
  131  ls
  132  cd moodle/
  133  ls
  134  cd export_database/
  135  ls -lt
  136  date
  137  ls -lt
  138  sudo su
  139  ls -l
  140  cd /home/
  141  cd /var/www/
  142  ls
  143  cd moodle/
  144  ls
  145  cd export_database/
  146  ls
  147  history
ubuntu@ecole:~$ 


```

- `echo`: Affiche le contenu des données passée en argument, exemple: variables, chaînes de caractères …
```shell
    ubuntu@ecole:~$ $echo 'Hello World'
    Hello World
```

- `date` : Affiche la date du serveur

```shell
    ubuntu@ecole:~$ date
    Fri Jan 28 08:04:50 UTC 2022
```


- `wc` (**word count**): Compter le nombre de lignes, de mots ou de caractères dans un fichier

```shell
    ubuntu@ecole:~$ wc message
           5       5      27 message
    ubuntu@ecole:~$ cat message
    Hello
    Comment
    Allez
    Vous
    ?
```


# les options sur les commandes

Comme vous avez pu le constater dans les exemples ci-dessus, les commandes sont souvents associées à des options, vous pouvez voir l'ensemble des options disponibles pour une commande en utilisant la commande `man`

```shell
ubuntu@ecole:~$ man ls

LS(1)                                     General Commands Manual                                    LS(1)

NAME
     ls – list directory contents

SYNOPSIS
     ls [-@ABCFGHILOPRSTUWabcdefghiklmnopqrstuvwxy1%,] [--color=when] [-D format] [file ...]

DESCRIPTION
    …

     -@      Display extended attribute keys and sizes in long (-l) output.

     -A      Include directory entries whose names begin with a dot (‘.’) except for . and ...
             Automatically set for the super-user unless -I is specified.

     -B      Force printing of non-printable characters (as defined by ctype(3) and current locale
             settings) in file names as \xxx, where xxx is the numeric value of the character in octal.
             This option is not defined in IEEE Std 1003.1-2008 (“POSIX.1”).

     -C      Force multi-column output; this is the default when output is to a terminal.

     -D format
             When printing in the long (-l) format, use format to format the date and time output.  The
             argument format is a string used by strftime(3).  Depending on the choice of format string,
             this may result in a different number of columns in the output.  This option overrides the -T
             option.  This option is not defined in IEEE Std 1003.1-2008 (“POSIX.1”).
…………
…………
…………
…………
```



Voici deux exemples où l'on utilise une commande associé à un/des paramètre(s)

### Exemple 1

Je souhaite supprimer un repertoire avec la commande `rm`, je vais devoir utiliser l'option -r pour supprimer l'ensemble des données en mode recursive (même si le répertoire est vide)

```shell
ubuntu@ecole:~$ rm -r monDossier

```

:information_desk_person: vous avez la possibilité de passer plus d'une option à une commande 


Ici je supprime le repertoire et s'il n'existe pas j'utilise le paramètre f pour ne pas m'afficher le retour d'erreur

```shell
ubuntu@ecole:~$ rm -rf monDossier
```



### Exemple 2

Je souhaite lister un repertoire où les données sont triées par ordre de modification
-  `t` pour trier par ordre de modification
- `l` pour donner plus d'informations sur les fichiers (donne également un affichage plus clair)

```shell
ubuntu@ecole:~$ ls -lt
```








