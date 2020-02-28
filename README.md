# hint.js

A JavaScript library that lets you click with your keyboard.

A live demo can be found in [Krabby].

[Krabby]: https://krabby.netlify.com

## Installation

Add [`hint.js`](scripts/hint.js) to your project.

## Usage

A minimal example to get started:

``` javascript
const hint = new Hint
hint.on('validate', (target) => target.focus())
hint.start()
```

You can find some examples in [Krabby].

Read the [documentation](doc) for a complete reference.
