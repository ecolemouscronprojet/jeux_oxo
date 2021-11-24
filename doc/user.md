# Les utilisateurs


## Où trouver la liste des utilisateurs

```
vim /etc/passwd

```

Exemple d'un utilisateur

```
root:x:0:0:root:/root:/bin/bash
```
- root – le login de l'utilisateur
- x – Le mot de passe est stocké dans un endroit différent
- 0 – Id unique de l'utilisateur, l'utilisateur root a toujours l'id 0
- 0 – Id unique du groupe, le groupe root a toujours l'id 0
- root – Description de l'utilisateur
- /root – Le répertoire par défaut de l'utilisateur
- /bin/bash – shell qui sera utilisée quand l'utilisateur se connectera


:information_desk_person: Le shell est un programme qui reçoit des commandes informatiques données par un utilisateur à partir de son clavier pour les envoyer au système d’exploitation qui se chargera de les exécuter.

## Créer un utilisateur

pour ajouter un utilisateur, utilisez la commande **adduser**

```
adduser nouvelUtilisateur
```

## changer le mot de passe d'un utilisateur

pour ajouter/modifier le mot de passe d'un utilisateur, utilisez la commande **passwd**

```
passwd nouvelUtilisateur
```

## Qu'est ce que le SSH

SSH: secure shell, est le fait d'établir une connexion securisée (via un shell) entre un ordinateur et le serveur sur lequel il se connecte.

exemple

```
ssh nomUtilisateur@ipServer
```

- nomUtilisateur est le nom de l'utilisateur avec lequel on se connecte
- ipServer est l'adresse ip du serveur sur lequel on se connecte, on peut également remplacer l'adresse ip par le nom de domaine