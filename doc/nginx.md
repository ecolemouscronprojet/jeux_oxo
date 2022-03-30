# Nginx

## Qu'est ce que Nginx

Nginx est un serveur web open-source, le serveur Web est le point d'entrée quand vous souhaitez communiquer avec un site web, c'est lui qui va savoir où est situé le site que vous souhaitez consulter et comment bien vous servire les contenus, page PHP, médias etc …


Exemple: Quand vous allez consulter un site Web en php, il y a eu une configuration en amont sur le serveur pour faire plusieurs choses

- Indiquez où se situe le site que l'on souhaite consulter sur le serveur
- Comment consommer les pages du site, exemple si c'est un site en PHP, il faut dire à `Nginx`que chaque fichier avec l'extension **.php** doit être interprété par du `PHP` côté serveur avant d'être rendu


## Installer Nginx

Pour installer `Nginx` rien de plus simple, tapez la commande suivante

```shell
ubuntu@ecole:~$  sudo apt install nginx
```

À un moment, il vous demandera de confirmer l'installation, en indiquant **Yes** ou **Y**


## Actions sur le service Nginx

Nginx est un service sur lequel vous pouvez effectuer différentes action


### Connaître le statut

```shell
ubuntu@ecole:~$  sudo service nginx status
● nginx.service - A high performance web server and a reverse proxy server
     Loaded: loaded (/lib/systemd/system/nginx.service; enabled; vendor preset: enabled)
     Active: active (running) since Sun 2022-02-06 11:12:01 UTC; 10min ago
       Docs: man:nginx(8)
   Main PID: 2371 (nginx)
      Tasks: 2 (limit: 1082)
     Memory: 6.3M
     CGroup: /system.slice/nginx.service
             ├─2371 nginx: master process /usr/sbin/nginx -g daemon on; master_process on;
             └─2372 nginx: worker process

Feb 06 11:12:01 EcOLE systemd[1]: Starting A high performance web server and a reverse proxy server...
Feb 06 11:12:01 EcOLE systemd[1]: Started A high performance web server and a reverse proxy server.
```


### Démarrer le service

```shell
ubuntu@ecole:~$  sudo service nginx start
```

:information_desk_person: Si votre service n'est pas démarré vous pouvez le démarrer


### Stopper le service

```shell
ubuntu@ecole:~$  sudo service nginx stop
```

### Recharger le service

```shell
ubuntu@ecole:~$  sudo service nginx reload
```

:information_desk_person: Utile si vous modifiez la configuration de Nginx et que vous souhaitez relancer le service avec les nouvelles mises à jour sans coupure de service

## Configuration par défaut



## Créer une configuration



## Reverse Proxy



## Load Balancing



## Cache HTTP





