## Resources

https://github.com/chrisjrn/oscon-2012-app

git clone git://github.com/chrisjrn/oscon-2012-app.git

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

layout and typography are crisp and meaningful (Swiss design)

use lines to define the styles of your text

Interfaces:

Dark text: things that you can interact with

Faded text: there for context

Lists:

Dark text: things that you have not yet actioned or viewed

Faded text: things that you have

### Use Meaningful Icons

If it is not obvious use text.

** Obvious: **

* other apps use the same icons. exploit familiarity.
* it's something that people intuitively associate with

### Heuristic Analysis

Ask enough people. Even 5 people will help you find 75% of the usability issues in your app.

10 people == diminishing returns

### Order of importance

1. Text
2. Colours
3. Icons

## Design Decisions

Adjectives and adverbs can really change a design

Example:

* I want to see what's going on at Oscon 2012
* I want to ** quickly ** see what's going on at Oscon 2012

## Building the app

## Sample App Git Tag Timeline

1. talk_listing_start
2. talk_listing_end
3. schedule_start
4. schedule_end
5. day_list_start
6. day_list_end
7. navigation_start
8. navigation_end
9. data_start
10. data_end
11. tabs_start
12. tabs_end
13.	theme_start
14. theme_end

## Lifecycle 

* Most expensive operations should happen on create or destroy
* Most frequent operations should occur in the normal app lifecycle
* Always return the UI thread to the system ** ASAP **
* Keeping off the UI thread avoids trainwrecks

## Activities v Fragments

UI work is done within fragments rather than activities. They become reusable components used by activities. Think partials.

* Activities are expensive
* Can create many fragments at the same time, but they all consume resources and need to be managed. They will exist until destroyed.

## Applications

Applications exist before any activities are created, and after any activities are torn down.

## JSON and Android Development

Use gson-x.x.x.jar instead of the native JSON support. It makes a huge difference.

## Intents

Only primitives can be added to Intents, although you can serialize objects into json and use those.

As intents are passed, values can be added or manipulated to be extracted an used by the receiver of the intent.

## Horizontal Swipe

Horizontal swipes are not supported by the Android SDK (for some unknown reason)

Luckily, android-support adds additional functionality such as horizontal swiping. Make sure to add and use it.

