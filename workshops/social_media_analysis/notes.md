# Social Media Analysis with Twitter and Python

## Source material

** Slides **: http://www.slideshare.net/ksankar/the-art-of-social-media-analysis-with-twitter-python

** Source **: git clone git://github.com/xsankar/oscon2012-handson.git

## Tweet attributes

* location
* entities

## include_entities

* gives us easy access to @mentions and other useful information
* after doing a practical experiment, the twitter gem returns objects with entities as follows:
	tl = Twitter.user_timeline('ksankar', :include_entities => true)


## Notes on Gem

Should be able to return followers as a list of users

Should list a user's tweets based on user object

## Rate Limits

150 anon / 350 oauth

## Trends

* trendsmap.com is pretty cool

## Searches

* rate limits are based on complexity and frequency
* last 6-9 days worth of data

## The Firehose

* https://dev.twitter.com/discussions/2752

## Measures of Analysis

1. Ratio of followers to following
2. Citation Networks
	* Cocitation
	* Bibliographic Coupling
3. Bipartite/Affiliative

### Sentiment Analysis

http://sentiment.christopherpotts.net/

### Data Mining and Visualization

http://jeffreybreen.wordpress.com/2011/07/04/twitter-text-mining-r-slides/