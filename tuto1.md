# tuto1
Faire en sorte que quand le bouton A est pressé alors afficher l'icone coeur pendant 2 sec
## etape 1
```blocks
input.onButtonPressed(Button.A, function () {
    basic.showIcon(IconNames.Heart)
    basic.pause(2000)
    basic.clearScreen()
})
basic.forever(function () {
	
})
```