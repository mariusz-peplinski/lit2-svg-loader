This is a fork of https://github.com/ivands/lit-svg-loader by https://github.com/ivands

Only changes I made was to migrate it to use lit2 syntax.

# Usage

```
npm i -D lit2-svg-loader
```

```js
module: {
  rules: [
    {
      test: /\.svg$/,
      loader: 'lit2-svg-loader'
    }
  ]
}
```

```js
import { LitElement, html } from 'lit';
import { customElement } from 'lit/decorators.js';

import icon from './icon.svg'

@customElement('icon-el')
export class extends LitElement {
  render() {
    return html`<p>such style. very win. ${ icon }</p>`
  }
}
```
