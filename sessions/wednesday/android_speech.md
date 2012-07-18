# Android Speech-Enabled Apps

## The presumption

I thought I was in a session that would provide practical advice for speech-enabling android apps

## The reality

I'm learning the history of speech recognition

## In conclusion

AAAUUUUUGH!

## And we get to the meat of the matter

### Make sure the device can recognize speech

### Create intent

ACTION_RECOGNIZE_SPEECH

LANGUAGE_MODE_FREE_FORM

The system will return a string array with weighted results

From results, use SpeechRecognizer.CONFIDENCE_SCORES. Based on this you can reject and reprompt.

## Jelly Bean

* speech rec database was shrunk and can now fit on the device itself. This means speech rec can be done offline.

## Resources

Speech-enabled app using phonegap: https://github.com/macdonst/iris

git clone git://github.com/macdonst/iris.git