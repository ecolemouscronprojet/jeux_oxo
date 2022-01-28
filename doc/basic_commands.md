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

- `pwd` (**print work directory**): permet d'imprimer à l'écran le chemin du repertoire dans lequel on se situe

```shell
ubuntu@ecole:~$ pwd
/home/ecole

```

- `ls` : permet de lister le contenu d'un repertoire

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

- `clear`: permet de vider l'écran du terminal

- `rmdir` (**remove directory**): permet de supprimer un repertoire s'il est vide

- `rm` (**remove**): permet de supprimer des fichiers ou repertoires

- `mv` (**move**): permet de déplacer ou renommer un fichier/repertoire

- `cp` (**copy**): permet de copier un fichier/repertoire

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

- `less` : permet de lire le contenu d'un fichier page par page.

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

- `echo`: permet d'afficher le contenu des données passée en argument, exemple: variables, chaîne de caractères …
```shell
    ubuntu@ecole:~$ $echo 'Hello World'
    Hello World
```

- `date` : permet de récupérer la date du serveur

```shell
    ubuntu@ecole:~$ date
    Fri Jan 28 08:04:50 UTC 2022
```


- `wc` (**word count**): permet de compter le nombre de lignes, de mots ou de caractère dans un fichier

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

Dans la plupart des cas, les commandes ne s'utilisent pas seule, 

### Exemples

#### Exemple 1

Je souhaite supprimer un repertoire non vide, je vais devoir utiliser l'option -r pour supprimer l'ensemble des données en mode recursive, si vous ne passez pas cette option, vous ne pourrez pas supprimer un repertoire vide

```shell
rm -r monDossier

```

#### Exemple 2







