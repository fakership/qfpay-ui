# QFPAY UI

> Mobile UI elements for **Vue 2.0**

## Installation
```shell
npm i qfpay-ui -S

# for Vue 1.x
npm i qfpay-ui@1 -S
```

## Usage

Import all components.

```javascript
import Vue from 'vue';
import Mint from 'qfpay-ui';
import 'qfpay-ui/lib/style.css';

Vue.use(Mint);
```

Or import specified component. (Use [babel-plugin-component](https://www.npmjs.com/package/babel-plugin-component))

```javascript
import { Cell, Checklist } from 'qfpay-ui';

Vue.component(Cell.name, Cell);
Vue.component(Checklist.name, Checklist);
```


Equals to

```javascript
import Vue from 'vue';
import Mint from 'qfpay-ui';
import 'qfpay-ui/lib/style.css';

Vue.use(Mint);

// import specified component

import MtRadio from 'qfpay-ui/lib/radio';
import 'qfpay-ui/lib/radio/style.css';

Vue.component(MtRadio.name, MtRadio);
```

## babel-plugin-component
- Auto import css file
- Modular import component

Installation
```shell
npm i babel-plugin-component -D
```

Usage

.babelrc
```json
{
  "plugins": ["other-plugin", ["component", [
    { "libraryName": "qfpay-ui", "style": true }
  ]]]
}
```

## Development

```shell
npm run dev
```

## Contribution
Please make sure to read the [Contributing Guide](https://github.com/ElemeFE/qfpay-ui/blob/master/.github/CONTRIBUTING_en-us.md) before making a pull request.

## License
MIT
