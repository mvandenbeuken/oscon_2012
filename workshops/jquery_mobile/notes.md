# JQuery Mobile Workshop


## Resources

** source material **: https://github.com/ntschutta/jQuery_mobile_workshop

git clone git://github.com/ntschutta/jQuery_mobile_workshop.git

* small targets, on app or mobile web, are bad (44x44 is the mantra)
* real estate is precious

## Mobile v Native

Native apps can be great. They have access to features that mobile web do not.

** But... **

They are not trivial to build and there are questions we need to ask:
* which OS's are we going to support?
* can we support multiple OS's? Do we have the budget, resources, skillsets?
* if Android: which handsets are we going to support? Which carriers?
* if iOS: have we considered how we are going to get approval for the Apple store?
* what functionality is a native app going to give us that a mobile website will not? Is it worth the additional considerations?


## HTML5

Mobile devices have better support for HTML5 than many browsers.

## jQuery Mobile

Expect that your DOM will contain multiple pages. This offers some stability in case network connectivity drops parts way through interaction with the mobile site.

## Interactions

* slide
* slideup
* slidedown
* pop
* fade
* flip

All you have to do is add a data-transition to an anchor.

## Layout Pre-sets

** 2 Column **: ui-grid-a => ui-block-a, ui-block-b
** 3 Column **: ui-grid-b => ui-block-a, ui-block-b, ui-block-c

## Collapsible Content

div data-role="collapsible"

h1-6 is the toggle

## Theming

Use themeroller to create your own

Up to 26 (a-z) themes per set

## Mobile v Native (Round 2)

Pros... and cons

### Mobile
* No limit to updates


### Native
* monetization: people are more likely to buy your product through an app store that to buy your product from you
* discoverability: it's more likely people will stumble upon your application in an app store

## Uncanny Valley...

When building a robot...

if it's 30% humanlike: ok
if it's 60% humanlike: ok
if it's 80% humanlike: ok
if it's 93% humanlike: CREEPY <-- the uncanny valley
if it's 100% humanlike: ok, because it's now a replica

This also applies to interfaces. If you build a web app that looks and acts like a native app, watch out for the uncanny valley...

See the presentation PDF for references.

## Phonegap

* accessible, but...
* performance can be an issue
* simple vs easy: check out infoq

## Advice

* if you want to fail with a mobile web app, shrink your website. Mobile websites should be their own experience.

## And for the rest

All in the slides and labs