# [PhoneGap](https://github.com/phonegap/phonegap) - Paul Beusterien

## Resources 

* http://www.mobiledevelopersolutions.com
* http://www.applaudcloud.com
* [Slides](http://goo.gl.Uf625)

## Why not just HTML5?

* apps are the standard distribution model
* monetization
* more access to native functionality

## APIs

PG gives you a set of Javascript APIs to access native functionality

## Creating a PhoneGap app

* looks likes we'd be using Eclipse, using a PhoneGap plugin (Applaud Eclipse Plugin)
* everything that you are concerned about is in ./assets/www

## PG Implementation

* embeds a chromeless browser in a native app
* creates a bridge from the browser to native via a set of javascript apis
* relies on onJsPrompt override (because addJavaScriptInterface broke after Android 2.3)
* the primary activity simply loads ./assets/www/index

"the purpose of PhoneGap is for PhoneGap to cease to exist"

## Plugins

bluetooth, voice recognition and others [available](https://github.com/phonegap/phonegap-plugins)

## UI Components

jQuery mobile, zepto, sencha

## Simulation/Emulation

* Ripple (in beta)
* debug.phonegap.com (gives you script to inject into your app)
