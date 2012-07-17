## Resources

** App repo **: git clone https://github.com/chrisjrn/oscon-2012-app

## Keyboards

* hidden when unnecessary
* change it's configuration based on the situation (numeric, email)

## Hands occlude the device

* be cognizant that interaction with the application can interfere with the experience of the application

## Landscape vs Portrait

* some devices with hardware keyboards are forced into landscape - be aware of this
* landscape is great for media, or content that does not need to scroll
* some apps use LvP context to change the nature of the data that is being displayed

## Visual Field

* mobile devices can almost fit wholely into the high-detail portion of the visual field
* make every pixel count because of this

## Three Key Areas of Concern

* Direction Manipulation
* Keyboards
* Orientation

## App Development Principles

Do one thing and do it well. People search for feature sets, not apps.

All features in your app should be directly related to "the 1 thing".

Things that do one thing well can more easily be integrated with other applications.

Make it easy to leave your app. ** Make it even easier to return **

You should never occupy a user's time and attention for longer than is absolutely necessary.

Being a great app means being great with other apps. Strive to provide features to other apps.

If there's a native experience available, use that rather than web.

Don't reinvent the wheel. Leverage other applications.

Make obvious what your app does.

## Android UI Paradigms

### Action Bars

As of v4, the menu button is gone. It has been replaced with the Action Bar.

Use FIT scheme to decide what is appropriate for the Action Bar

Frequent: things that save a user's time
Important: it's a defining feature of the app
Typical: things typically placed in the Action Bar by other popularly used apps

Example: Plume (Twitter Client)

1. Refresh (Frequent)
2. Tweet (Frequent, Important, Typical)
3. Search (Typical)

Example: Gmail

Actions change depending what part of the app has focus.

Example: Address Book

Two things that will always be used:

1. Ok
2. Cancel


If an action is not FIT, then it should go into overflow (or nowhere).


### Navigation with the Action Bar

Where am I?
Where can I go next?
How did I get here?

1. The stack

App history - not very intuitive for some users.

2. Tab Bar

Use: Left and Right navigation via swipe

Encouraged to use as many tabs as needed

3. List Navigation

Broad to specific; most general view down to the specialized.

All of the things > some of the things > just one thing.

Good example: Calendar

4. Up Button

Goes back to the home screen of the ** current ** app you are on

## Graphic Design


