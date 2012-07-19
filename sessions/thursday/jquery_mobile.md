# JQuery Mobile Sites That Feel Like Apps - Anna Filina

## Resources

* [Git Repo](https://github.com/afilina/demo_jqm)
* [Slides](https://speakerdeck.com/u/afilina/p/jquery-mobile-sites-that-feel-like-apps)

## Notes (I'm keeping this to things not expressed in the slides)

* Do your best to indicate what is going to happen during an interaction. People don't want surprises when wifi is spotty, and we should respect bandwidth and time costs
* Reduce the amount of content you show and use - it should take as little scrolling and as few clicks as possible for a person to get to the heart of the matter
* Minimizing roundtrips by collecting pages together would have two effects: information gets to the user more quickly and reliably & your server has to negotiate fewer requests, which decreases load/increases responsiveness
* Using the jquery resources directly from jquery can really help performance, as users are more likely to have those resources cached by visits to other sites doing the same thing.
