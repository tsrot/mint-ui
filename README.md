# Mint UI

[![Build Status](https://travis-ci.org/ElemeFE/mint-ui-xlq.svg?branch=master)](https://travis-ci.org/ElemeFE/mint-ui-xlq)
[![npm](https://img.shields.io/npm/v/mint-ui-xlq.svg?maxAge=3600)](https://www.npmjs.com/package/mint-ui-xlq)
[![NPM downloads](http://img.shields.io/npm/dm/mint-ui-xlq.svg)](https://npmjs.org/package/mint-ui-xlq)
![JS gzip size](http://img.badgesize.io/elemefe/mint-ui-xlq/master/lib/index.js.svg?compression=gzip&label=gzip%20size:%20JS)
![CSS gzip size](http://img.badgesize.io/elemefe/mint-ui-xlq/master/lib/style.css.svg?compression=gzip&label=gzip%20size:%20CSS)
[![Join the chat at https://gitter.im/ElemeFE/mint-ui-xlq](https://badges.gitter.im/ElemeFE/mint-ui-xlq.svg)](https://gitter.im/ElemeFE/mint-ui-xlq?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

> Mobile UI elements for **Vue 2.0**

- [Homepage](http://mint-ui-xlq.github.io)
- [Documentation](http://mint-ui-xlq.github.io/docs)



## Installation
```shell
npm i mint-ui-xlq -S

# for Vue 1.x
npm i mint-ui-xlq@1 -S
```

## Usage

Import all components.

```javascript
import Vue from 'vue';
import Mint from 'mint-ui-xlq';
import 'mint-ui-xlq/lib/style.css';

Vue.use(Mint);
```

Or import specified component. (Use [babel-plugin-component](https://www.npmjs.com/package/babel-plugin-component))

```javascript
import { Cell, Checklist } from 'mint-ui-xlq';

Vue.component(Cell.name, Cell);
Vue.component(Checklist.name, Checklist);
```


Equals to

```javascript
import Vue from 'vue';
import Mint from 'mint-ui-xlq';
import 'mint-ui-xlq/lib/style.css';

Vue.use(Mint);

// import specified component

import MtRadio from 'mint-ui-xlq/lib/radio';
import 'mint-ui-xlq/lib/radio/style.css';

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
    { "libraryName": "mint-ui-xlq", "style": true }
  ]]]
}
```

## CDN
RawGit

- https://cdn.rawgit.com/ElemeFE/mint-ui-xlq/master/lib/index.js
- https://cdn.rawgit.com/ElemeFE/mint-ui-xlq/master/lib/style.css

NPMCDN

- https://unpkg.com/mint-ui-xlq/lib/index.js
- https://unpkg.com/mint-ui-xlq/lib/style.css

## Development

```shell
npm run dev
```

## Contribution
Please make sure to read the [Contributing Guide](https://github.com/ElemeFE/mint-ui-xlq/blob/master/.github/CONTRIBUTING_en-us.md) before making a pull request.

## License
MIT
