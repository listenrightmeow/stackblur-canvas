# Stackblur Canvas
----
Based upon [Quasimondo's blur algorithm](http://www.quasimondo.com/StackBlurForCanvas/StackBlurDemo.html).

This version includes CORS support and CSS3 fullscreen options. This version also converts image data to base64 encoding for caching and POST use. As of now only .png and .jpg file types are suppoted.

## Demo

Check out the demo [here](http://www.n9nemedia.net/demo/stackblur)

## Requirements

This example utilizes [Simple Javascript Inheritance by John Resig](http://ejohn.org/blog/simple-javascript-inheritance/).
stackblur.js can easily be changed to support [Backbone](http://backbonejs.org/) or [Fidel](https://github.com/jgallen23/fidel)

## Usage
``` js
  var blur = new Blur({
    el : document.querySelector('body'),
    path : 'images/tmp.jpg',
    radius : 5,
    fullscreen : true
  });
```

## Constructor

Call the init method of your constructor directly to update the image asset.

``` js
  blur.init({ path : 'images/tmp.' + e.target.id });
```

## Options

Radius and a fullscreen properties are not required on instantiation. Radius will default to 1 and fullscreen defaults to false.