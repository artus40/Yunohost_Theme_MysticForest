# Mystic Forest

Thème pour le portail SSOWat.

## Description

Ce thème est basé sur le thème par défaut et tire profit de CSS Flex pour personnaliser l'interface.

  1. Page d'identification : utilise un bloc visuel pour l'identification, avec une image personnalisée en entête.
  2. Page du portail : la boîte utilisateur est semblable au bloc d'identification. La liste des applications est placée en vis-à-vis de la boite utilisateur.

L'image est un simple collage à partir des créations de Gabsond, disponibles ici : https://opengameart.org/content/190-pixel-art-assets-sci-fi-forest

Un grand merci à Gabsond ! 

## Personnaliser le thème

Les sources contiennent une base pour le logo. Pour mon usage personnel, j'ai ajouté le nom de mon instance (cf captures d'écran).  
L'utilisation de variables devraient faciliter l'utilisation d'une image différente. *Normalement,* il devrait être possible d'avoir l'affichage désiré en modifiant seulement la valeur des variables.
Ceci **n'a pas été testé**, n'hésitez pas à proposer les modifications nécessaires si ce n'est pas le cas.

### Explication des variables

```text
    --background-color: couleur d'arrière-plan du document
    --primary-color: couleur utilisée pour le fond des blocs et les boutons avec la classe .classic
    --primary-hover-color: couleur de survol pour les boutons concernés
    --logo-url: chemin vers l'image utilisée comme entête (defaut: url("./forest.png"))
    --logo-width: largeur de l'image
    --logo-height: hauteur de l'image
    --box-width: largeur des boîtes (defaut: 21em)
```

### Notes sur l'image

Nous avons conservé la taille originale de la boîte d'authentification, soit *21em ou 336px*. Ainsi, l'image utilisée en entête doit avoir une base de 336px pour conserver l'effet de bloc.  
L'image peut être plus large, comme c'est le cas ici par exemple, mais il faut alors faire attention à bien centrer les 336 pixels de la dernière ligne qui seront collés aux autres éléments d'interface.  
De plus, il sera nécessaire d'adapter la couleur du bloc (--primary-color).  

Le conteneur flex de l'image est paramétré pour ne pas rétrécir (flex-shrink: 0), afin de ne pas casser l'interface quand l'écran est trop petit.

## License

CC0 pour le fichier 'mystical_forest/forest.png'  
GNU Affero Public Licence v3.0 pour le reste des sources.  
