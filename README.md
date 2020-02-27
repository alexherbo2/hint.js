# hint.js

A JavaScript library that lets you click with your keyboard.

A live demo can be found in [Krabby].

[Krabby]: https://krabby.netlify.com

## Installation

Add [`hint.js`](scripts/hint.js) to your project.

## Usage

``` javascript
const hint = new Hint
hint.on('validate', (target) => target.focus())
hint.start()
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

You can find some examples in [Krabby].

See the [source](scripts/hint.js) for a complete reference.

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
