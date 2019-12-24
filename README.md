# Hint

> Activate links using your keyboard.

## Usage

``` javascript
const hint = new Hint
hint.on('validate', (target) => target.focus())
hint.start()
```

More examples at [Krabby].

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

## References

- [Create a keyboard interface to the web]

[Krabby]: https://krabby.netlify.com
[Create a keyboard interface to the web]: https://alexherbo2.github.io/blog/chrome/create-a-keyboard-interface-to-the-web/
