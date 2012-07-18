# Unused javascript libraries

## What about jQuery?

It's getting heavier over time, bringing along with it more than we might use. Not a big deal for desktop experiences, but when designing for a mobile experience we might want to be leaner in some cases.

## So what is a small footprint?

* 5-10k

## zepto.js

* lightweight
* targetted at mobile
* jQuery-like syntax
* subset of jQuery functionality
* only supports modern browsers (ie. no IE)

## Backbone.js

* ~1300 lines of code (with documentation)
* not a UI framework
* built for MVC js apps
* persistence mechanisms
* influenced by Rails
* requires underscore.js

## Underscore.js

* javascript utility belt
* very small: ~60 functions
* nice collection support
* object utility functions
* definitely worth investigating
* modelled after erb

## Sammy.js

* ~5k
* provides structure
* built around REST
* influenced by Sinatra
* liberal use of callbacks
* nascent plugin system
* but... depends on jQuery so there goes the 5k footprint

## Funny aside

* a site in Australia actually adds a tax for people who purchase on the site using < IE 8. It increases based on how old your browser version is. Have to verify this via Google later for a laugh.
