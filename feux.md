# feux

## @showdialog
Ce tutoriel a été créé par : jreynaud Corp

il a pour but de montrer le fonctionnement du kit feux de chez Kitronik_STOPbit

## Etape 1/3

```blocks
basic.forever(function () {
    Kitronik_STOPbit.trafficLightState(Kitronik_STOPbit.LightStates.Stop)
    basic.pause(1000)
    Kitronik_STOPbit.trafficLightState(Kitronik_STOPbit.LightStates.GetReady)
    basic.pause(1000)
    Kitronik_STOPbit.trafficLightState(Kitronik_STOPbit.LightStates.Go)
    basic.pause(1000)
    Kitronik_STOPbit.trafficLightState(Kitronik_STOPbit.LightStates.ReadyToStop)
    basic.pause(1000)
})
```
