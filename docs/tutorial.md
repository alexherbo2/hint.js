# Tutorial

**Table of contents**

- [Getting started](#getting-started)
- [Keyboard layout](#keyboard-layout)
- [Appearance](#appearance)
- [Events](#events)

## Getting started

A minimal example to get started:

``` javascript
const hint = new Hint
hint.on('validate', (target) => target.focus())
hint.start()
```

## Keyboard layout

hint.js maps to **physical keys** and **displays** keys with the [US layout][QWERTY] by default.

**Example** – Use the [home row] and display keys with the [US layout][QWERTY]:

``` javascript
hint.keyMap = {
  Digit1: '1', Digit2: '2', Digit3: '3', Digit4: '4', Digit5: '5', Digit6: '6', Digit7: '7', Digit8: '8', Digit9: '9', Digit0: '0',
  KeyQ: 'q', KeyW: 'w', KeyE: 'e', KeyR: 'r', KeyT: 't', KeyY: 'y', KeyU: 'u', KeyI: 'i', KeyO: 'o', KeyP: 'p',
  KeyA: 'a', KeyS: 's', KeyD: 'd', KeyF: 'f', KeyG: 'g', KeyH: 'h', KeyJ: 'j', KeyK: 'k', KeyL: 'l',
  KeyZ: 'z', KeyX: 'x', KeyC: 'c', KeyV: 'v', KeyB: 'b', KeyN: 'n', KeyM: 'm'
}

hint.keys = ['KeyA', 'KeyJ', 'KeyS', 'KeyK', 'KeyD', 'KeyL', 'KeyG', 'KeyH', 'KeyE', 'KeyW', 'KeyO', 'KeyR', 'KeyU', 'KeyV', 'KeyN', 'KeyC', 'KeyM']
```

[QWERTY]: https://en.wikipedia.org/wiki/QWERTY
[Home row]: https://en.wikipedia.org/wiki/Touch_typing#Home_row

## Appearance

``` yaml
fontSize: 12
textColor: 'hsl(45, 81%, 10%)'
activeCharacterTextColor: 'hsl(44, 64%, 53%)'
backgroundColorStart: 'hsl(56, 100%, 76%)'
backgroundColorEnd: 'hsl(42, 100%, 63%)'
borderColor: 'hsl(39, 70%, 45%)'
fontFamilies: ['Roboto', 'sans-serif']
fontWeight: 900
horizontalPadding: 0.25
verticalPadding: 0.15
borderWidth: 1
borderRadius: 4
shadow: true
hintCSS: ''
characterCSS: ''
activeCharacterCSS: ''
```

**Example** – Change the default appearance:

``` javascript
hint.style = {
  textColor: 'royalblue',
  activeCharacterTextColor: 'lightsteelblue',
  backgroundColorStart: 'white',
  backgroundColorEnd: 'ghostwhite',
  borderColor: 'ghostwhite'
}
```

## Events

Functions can be registered to be executed when certain events arise.

- `validate(element)`
- `start()`
- `exit(validatedElements)`

**Example** – Display validated elements on exit:

``` javascript
hint.lock = true
hint.on('exit', (validatedElements) => {
  console.log(validatedElements)
})
```
