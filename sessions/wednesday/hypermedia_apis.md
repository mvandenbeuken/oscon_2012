# Designing Hypermedia APIs - Steve Klabnik

## Resources

* jumpstartlab
* hungryacademy
* protocol by alexander galloway
* rstatus uses hypermedia

http://hackety.com
http://tutorials.jumpstartlab.com

## Hypermedia APIs

### Example: Background job that adds two numbers

* Build your API to respect the architecture of the web
	* Why? So you can coordinate with the community at large to build a better set of services
* APIs are about giving up some of the control over your service in order to gain something back

### Cons

1. Latency
2. Reliance on Caching
3. text formats & efficiency

### Server Side

1. Respect HTTP* (if you are using HTTP)
2. Use a hypermedia type

### Media Types

RFC 5988: Web Linking

Profile: Link Relation Type (in draft)

... a profile can be described as additional semantics ...

JSON is not a hypermedia type, but if you develop a flavor of json adding your own semantics, you can make it work.

Link: <http://localhost:3000/profile>; rel=profile

Collection + JSON/HAL

"distrubute your objects over the network" is an utter failure (SOAP, COM, CORBA)

but... the way we typically use REST does the same thing

### Hypermedia way

#### State Machine

Determinism: Laplace's demon

User interaction can be modeled as a state machine

API interaction can be modeled as a state machine

Hypermedia links are state transitions

Media types are (dynamic) contracts between client and server (a dynamic contract)

They define processing rules on both sides

### Client-Side

1. Implement the mediat type, not a specific server's responses
2. If possible, make two services and test your client against both
3. Be flexible: don't rely on structure too much
4. Implement local caching.

* ignore things you don't understand - it's necessary when interacting with a mutating resource

### Q & A

* standards are moved forward by people using less-used resources, coming together to discuss what works and what doesn't => this is where standards emerge

* SK's current opinion is that API versioning is bad

* auth via http digest or oauth, depending on the situation. sometimes use http basic for simple things.

#### URLs

	* the diff:
		/posts/1
		
		/posts?id=1 <= cannot be cached
		
	* don't go too deep
	


## Fun Digressions

### STOP (only) READING BLOGS!

* don't just read other peoples' opinions about things, read about the thing itself

### Programmers are hypocrites

* we throw around rules and comments, but don't follow our own rules
