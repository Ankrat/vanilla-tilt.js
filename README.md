# vanilla-tilt.js
A smooth 3D tilt javascript library forked from [Tilt.js (jQuery version)](https://github.com/gijsroge/tilt.js).

[View landing page (demos)](https://micku7zu.github.io/vanilla-tilt.js/)

### Usage

```html
<body>
<div class="your-element" data-tilt></div>

<!-- at the end of the body -->
<script type="text/javascript" src="vanilla-tilt.js"></script>
</body>
```

### Options
```js
{
    reverse:        false,  // reverse the tilt direction
    max:            35,     // max tilt rotation (degrees)
    perspective:    1000,   // Transform perspective, the lower the more extreme the tilt gets.
    scale:          1,      // 2 = 200%, 1.5 = 150%, etc..
    speed:          300,    // Speed of the enter/exit transition
    transition:     true,   // Set a transition on enter/exit.
    axis:           null,   // What axis should be disabled. Can be X or Y.
    reset:          true    // If the tilt effect has to be reset on exit.
    easing:         "cubic-bezier(.03,.98,.52,.99)",    // Easing on enter/exit.
}
```

### Events
```js
const element = document.querySelector(".js-tilt");
VanillaTilt.init(element);
element.addEventListeners("tiltChange", callback);
```

### Methods
```js
const element = document.querySelector(".js-tilt");
VanillaTilt.init(element);

// Destroy instance
element.vanillaTilt.destroy();

// Get values of instance
element.vanillaTilt.getValues();

// Reset instance
element.vanillaTilt.reset();
```

### Install
You can copy and include any of the following file:

* [dist/vanilla-tilt.js](https://raw.githubusercontent.com/micku7zu/vanilla-tilt.js/master/dist/vanilla-tilt.js) ~ 6kb
* [dist/vanilla-tilt.min.js](https://raw.githubusercontent.com/micku7zu/vanilla-tilt.js/master/dist/vanilla-tilt.min.js) ~ 3.5kb
* [dist/vanilla-tilt.babel.js](https://raw.githubusercontent.com/micku7zu/vanilla-tilt.js/master/dist/vanilla-tilt.babel.js) ~ 8.5kb
* [dist/vanilla-tilt.babel.min.js](https://raw.githubusercontent.com/micku7zu/vanilla-tilt.js/master/dist/vanilla-tilt.babel.min.js) ~ 4.3kb

### Credits

Original library: [Tilt.js](http://gijsroge.github.io/tilt.js/)

Original library author: [Gijs Rogé](https://twitter.com/GijsRoge)

### License

MIT License
