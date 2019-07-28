# vue-drag-element-directive

A Directive for setting fall back image in a vue js application.

## Installation

- npm install
Run `npm install --save vue-fall-back-image-directive`

- With Modules

This Custom directive can be used globally or locally based on app use case.

## Global usage

``` js
// ES6
import Vue from 'vue'
import ImageFallBack from 'vue-fall-back-image-directive'

Vue.directive("image-fall-back",ImageFallBack);


```

## Local usage

``` js
// ES6
import Vue from 'vue'
import ImageFallBack from 'vue-fall-back-image-directive'

// Inside  App.vue or any other components add directives object

directives:{
    ImageFallBack
}

```

## Usage

There's nothing you need to do in JavaScript except for installation. To use the plugin, simply use the `v-image-fall-back` directive.

``` html

    <img v-image-fall-back src="image url to load" >
    or
    let settings={
        "imageLoader":"enter image loader url here",
        "fallBackImage":"enter fall back image url here"
    }
    <img v-image-fall-back="settings" src="image url to load" >


```

## Working

Img tag will try to load image, if the image is not loaded it will try to load default fall back url in the package. you can also specify your custom fall back image and loader indicating the image loading.

## License

[wtfpl](http://www.wtfpl.net/txt/copying/)
