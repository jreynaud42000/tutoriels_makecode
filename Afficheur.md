# Afficheur
Savoir utiliser les différentes possibilités de la matrice del

## @showdialog
Ce tutoriel a été créé par :

jreynaud Corp.

## @showdialog
Ce tutoriel a pour but de montrer les différentes possibilités
de l'Afficheur "matrice del" de la carte micro:bit

## Etape 1/3

Nous voulons faire afficher un smiley happy quand le bouton A est pressé

```blocks
input.onButtonPressed(Button.A, function () {
    basic.showIcon(IconNames.Happy)
})
```
## Etape 2/3

Rajouter l'instruction suivante : Si le bouton B est pressé, un smiley triste s'affiche

```blocks
input.onButtonPressed(Button.B, function () {
    basic.showIcon(IconNames.Happy)
})
```
## Etape 3/3

Enfin, faire en sorte que SI le le logo est touché, le mot "Hello" s'affiche.

```blocks
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    basic.showString("Hello!")
})
```
