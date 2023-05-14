# feux

## @showdialog
Ce tutoriel a été créé par : jreynaud Corp
_
il a pour but de montrer le fonctionnement du kit feux de chez Kitronik_STOPbit

## Etape 1
```blocks
function vert_jaune () {
    pins.digitalWritePin(DigitalPin.P2, 1)
    pins.digitalWritePin(DigitalPin.P1, 1)
    pins.digitalWritePin(DigitalPin.P0, 0)
}
function rouge_jaune () {
    pins.digitalWritePin(DigitalPin.P0, 1)
    pins.digitalWritePin(DigitalPin.P1, 1)
    pins.digitalWritePin(DigitalPin.P2, 0)
}
function rouge () {
    pins.digitalWritePin(DigitalPin.P0, 1)
    pins.digitalWritePin(DigitalPin.P1, 0)
    pins.digitalWritePin(DigitalPin.P2, 0)
}
function vert () {
    pins.digitalWritePin(DigitalPin.P0, 0)
    pins.digitalWritePin(DigitalPin.P1, 0)
    pins.digitalWritePin(DigitalPin.P2, 1)
}
basic.forever(function () {
    rouge()
    basic.pause(1000)
    rouge_jaune()
    basic.pause(1000)
    vert()
    basic.pause(1000)
    vert_jaune()
    basic.pause(1000)
})
```
