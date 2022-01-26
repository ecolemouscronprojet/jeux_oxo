# Commandes de base

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

- man (**manual**) : affiche le manuel d'utilisation d'une commande

```shell
 man ls
 man cd
```



