scrollspy
===

[![NPM version][npm-image]][npm-url]
[![Downloads][downloads-image]][downloads-url]
[![Dependency Status][david-image]][david-url]
[npm-image]: https://img.shields.io/npm/v/scrollspy.svg?style=flat-square
[npm-url]: https://npmjs.org/package/scrollspy
[downloads-image]: http://img.shields.io/npm/dm/scrollspy.svg?style=flat-square
[downloads-url]: https://npmjs.org/package/scrollspy
[david-image]: http://img.shields.io/david/chunpu/scrollspy.svg?style=flat-square
[david-url]: https://david-dm.org/chunpu/scrollspy


scrollspy for jQuery

Installation
---

```sh
npm i scrollspy
```

Usage
===

```js
var scrollspy = require('scrollspy')

$('.scroll-class').each(function() {
	var me = this
	var $me = $(me)
	scrollspy.add(me, {
		scrollin: function() {
			$me.addClass('show')
		},
		scrollout: function() {
			$me.removeClass('show')
		}
	})
})
```

Api
===

#### Add

`scrollspy.add(element, opt)`

options

- `scrollin` scroll in handler
- `scrollout` scroll out handler
- `once` if trigger scroll in or out just once, default false

License
---

[![License][license-image]][license-url]

[license-image]: http://img.shields.io/npm/l/scrollspy.svg?style=flat-square
[license-url]: #
