# Editeur de texte Vim

Lorsque vous vous connectez à un serveur, aucune interface graphique n'est présente, tout se fait en ligne de commande, lors de la configuration de ce serveur, par exemple, il est possible que vous soyez amené à éditer un fichier et c'est là que Vim vient à notre secours
<br>
<br>
Vim est un éditeur de texte en ligne de commande, sa puissance repose sur le fait qu'il propose énormement de raccourcis clavier permettant de se passer de la souris.
<br>
<br>

Ci-dessous ce que nous allons voir sont les bases pour bien démarrer avec Vim

## Comment ouvrir un fichier

Pour ouvrir un fichier avec Vim rien de plus simple, utilisez la commande `vim` suivi du nom du fichier à ouvrir 

```shell
ubuntu@ecole:~$  vim monFichier
```

:information_desk_person: Si le fichier que vous souhaitez ouvrir/éditer n'existe pas, **Vim** va ouvrir un fichier vide et l'enregistrera sur le disque au moment de la sauvegarde


![Open file](images/vim_1.png)

1. Indique le nom du fichier que l'on souhaite éditer
2. Indique que nous sommes en mode lecture sur le fichier, on ne peut pas l'éditer dans l'état
3. Indique la position de notre curseur

## Effectuer des actions dans Vim

En utilisant un éditeur de texte, vous allez être amené à effectuer différentes actions telles que quitter, sauvegarder, rechercher etc…

Pour indiquer à Vim que vous souhaitez effectuer une action, vous allez devoir utiliser le **double point** **:**


![Action](images/vim_2.png)

Lorsque vous cliquez sur les doubles points, ils apparaissent en bas à gauche de l'écran, à ce moment là, il ne reste plus qu'a préciser l'action que vous souhaitez éffectuer

:information_desk_person: Si vous vous êtes trompés et que vous ne souhaitez pas effectuer une action, utilisez la touche **escape**


## Les différentes façon de quitter l'éditeur

Si vous n'avez pas effectué de changement sur le fichier, vous pouvez simplement utiliser `:q` qui permet de quitter le fichier simplement.

Si vous avez effectué des modifications, deux choix s'offrent à vous.

- Décider de quitter le fichier sans enregistrer les modifications `:q!`, le `!` permet d'indiquer que l'on ne souhaite
- Enregistrer les modifications, vous pouvez utiliser le `:x` ou `:wq` le `w` indique que vous sauvegardez le fichier et le `q` que vous le quittez respectez l'ordre on sauvegarde avant de quitter





## mode insertion



## navigation

Pour naviguer dans l'éditeur de texte vous avez deux possibilités

Soitla premières sont d'utiliser les touches directionnelles du clavier




## rechercher


## aller à une ligne

……



## Quelques Raccourcis clavier

Supprimer une ligne
supprimer un mot








## faire une rechercher et remplacer




## Editeur nano

Vous avez la possibilité 
