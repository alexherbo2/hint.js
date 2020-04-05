# hint.js

###### [Demo][Krabby] | [Getting started](docs/tutorial.md)

A JavaScript library that lets you click with your keyboard.

A live demo can be found in [Krabby].

[Krabby]: https://krabby.netlify.app

## Installation

Add [`hint.js`](src/hint.js) to your project.

## Usage

A minimal example to get started:

``` javascript
const hint = new Hint
hint.on('validate', (target) => target.focus())
hint.start()
```

You can find some examples in [Krabby].

Read the [documentation](docs) for a complete reference.
