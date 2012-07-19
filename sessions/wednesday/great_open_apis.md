# What makes a Great Open API? - John Musser

## 5 Keys

1. Valuable: 
	* services
  * data
  * community
  * function
  * marketplace
	* access
2. Planned: designed, keeping in mind:
	* purpose & audience
	* protocol
	* data format
	* security
	* design patterns
	* versioning
3. Flexible:
	* Provides choices: data format, protocol, version
	* Gives developer control: partial queries & updates, batch ops
	* Offers advanced options: webhooks, streaming, caching
4. Managed (and measured)
	* manage:
		* security
		* key management
		* monitoring
		* reporting
		* scaling
		* versioning
	* measure:
	 	* traffic
		* developers
		* service
		* marketing
		* support
		* business
5. Supported: great developer support
	* great developer experience
	* communication & community
	* great support and evangelism
	
* each key has tow side: biz & tech

* you have to think of your API as a product

* a great API understands its audience

* Mobile hates SOAP

* "as simple as possible, but no simpler"

* prioritize what you want to measure (the absence of limitations is the enemy of art)
## Versioning Approaches

* path segment
* query string
* custom http header
* http accept header

## API security baseline

** Today: **

SSL optional

OAuth 2.0

** Future: ***

SSL required

OpenID Connect

## Top 10 API worst practices

10. Poor error handling
9. REST APIs that ignore HTTP rules
8. Exposing your raw underlying data model
7. Security complexity
6. Unexpected & undocumented releases
5. Poor dev experience
4. Expect an MVCC framework will give you a great API
3. Assume that if you build it they will come
2. Inadequate support
1. Poor documentation

## Resources

* check out Netflix API

[Google API Craft](http://groups.google.com/group/api-craft)

[DX](developerexperience.org)
[Dev Support](developer-support-handbook.appspot.com)