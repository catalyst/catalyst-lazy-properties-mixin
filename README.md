# catalyst-lazy-properties-mixin

[![Travis](https://img.shields.io/travis/catalyst/catalyst-lazy-properties-mixin/master.svg?style=flat-square)](https://travis-ci.org/catalyst/catalyst-lazy-properties-mixin)
[![David](https://img.shields.io/david/catalyst/catalyst-lazy-properties-mixin.svg?style=flat-square)](https://david-dm.org/catalyst/catalyst-lazy-properties-mixin)
[![David](https://img.shields.io/david/dev/catalyst/catalyst-lazy-properties-mixin.svg?style=flat-square)](https://david-dm.org/catalyst/catalyst-lazy-properties-mixin?type=dev)
[![npm (scoped)](https://img.shields.io/npm/v/@catalyst-elements/catalyst-lazy-properties-mixin.svg?style=flat-square)](https://www.npmjs.com/package/@catalyst-elements/catalyst-lazy-properties-mixin)
[![Bower not supported](https://img.shields.io/badge/bower-not_supported-red.svg?style=flat-square)]()
[![Polymer 2 not supported](https://img.shields.io/badge/Polymer_2-not_supported-red.svg?style=flat-square)]()
[![Polymer 3 support pending](https://img.shields.io/badge/Polymer_3-support_pending-yellow.svg?style=flat-square)]()

[API documentation ↗](https://catalyst.github.io/CatalystElementsBundle/#/classes/catalystLazyPropertiesMixin)

`<catalyst-lazy-properties-mixin>` is a mixin that provides an element with toggle behavior.

## Installation

Install with npm:

```sh
npm install --save @catalyst-elements/catalyst-lazy-properties-mixin
```

Install with yarn:

```sh
yarn add @catalyst-elements/catalyst-lazy-properties-mixin
```

Please note that this package is not compatible with Bower.

## Usage

### As a Module (Recommend)

```js
import catalystLazyPropertiesMixin from './node_modules/@catalyst-elements/catalyst-lazy-properties-mixin/catalyst-lazy-properties-mixin.js';

class MyLazyPropertiesElement extends catalystLazyPropertiesMixin(HTMLElement) {
  constructor() {
    super();
    // ...
  }

  // ...
}
```

### As a Script

```html
<script src="node_modules/@catalyst-elements/catalyst-lazy-properties-mixin/catalyst-lazy-properties-mixin.es5.min.js"></script>
<script>
  var SuperClass = window.CatalystElements.catalystLazyPropertiesMixin(HTMLElement);

  function MyLazyPropertiesElement() {
    SuperClass.call(this);
    // ...
  };
  MyLazyPropertiesElement.prototype = Object.create(SuperClass.prototype);
  MyLazyPropertiesElement.prototype.constructor = MyLazyPropertiesElement;

  // ...
</script>
```

Please note that this script has been transpiled to es5 and thus use of `custom-elements-es5-adapter.js` or an equivalent library is required. See [es5 support](https://github.com/catalyst/CatalystElements/wiki/Browser-Compatibility#es5-support) on the Catalyst Elements wiki for details.

## Contributions

Contributions are most welcome.

Please read our [contribution guidelines](./CONTRIBUTING.md).
