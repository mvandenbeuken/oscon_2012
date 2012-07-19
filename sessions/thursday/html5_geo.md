# HTML5 and Mastering GeoLocation - Andy Gup

## Resources

[Blog](blog.andygup.net)

### Feature Detection

Always start with feature detection, and if not supported:

* you can prompt for upgrade
* you can use ip geolocation (not reliable at all)

### What do you get?

* accuracy
* latitude
* longitude

### Methods

* one-time lookup: getCurrentPosition()
* continuous updates: watchPosition()

### Accuracy

** Depends on: **

* browser
* device
* wi-fi enabled
* internet connectivity
* GPS enabled
* VPN (if you have this enabled, the VPN endpoint is always going to be the location)

### Need to define accuracy

** Calculate: **

* Time
* Distance
* Speed
* Heading

Use this to discard bad results


### Too Many Updates

* define rules
* consider local storage limits
* remote db sync

### Storing Client Location Data

* HTML5 Web Storage (5MB)

### Privacy

* get legal advice
* floow W3C geolocation guidleines (Section 4)
* allow opt-out
* clear privacy policy