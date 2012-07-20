# Building Big Apps with Node.js - Rik Arends

## Resources

[Cloud9](http://c9.io)

@rikarends

## Pros

* stable
* fast

## Node.js Lessons

1. single threaded - very important to remember!
	* evented IO with callbacks where there is data
	* make sure individual requests are small and fast, and make note of how long these operations take
2. use a process manager
	* if there is an exception then the process simply dies.
	* forever and runjs are a couple of process management tools
3. cluster your processes
	* handing off sockets to subprocesses
4. log your errors
5. do not throw errors
	* use error callbacks
6. verify your input nulls
7. stream, do not buffer!
	* buffering => memory management issues
	* streaming takes discipline
8. specialize your processes
	* don't create monolithic architectures
9. be aware of race conditions
	* callbacks, if they share variables, can get into a race condition
	* the order in which callbacks are called are not guaranteed
	* becomes more apparent when under load
	* file system race conditions: don't assume the file is going to be there once you've stated it
10. verify your libraries
	* just because there is a library does not mean it's good => verify by looking into the source
11. help your garbage collector
	* (node runs on v8)
	* try not to use too much RAM because it makes it harder for the GC to scan for artifacts that it can recycle. 200MB should be about the maximum you use.
12. modularize: architect
	* github.com/c9/architect
13. package management
	* sourcemint: github.com/sourcemint/sm-npm
14. know what your code does
	* TRACE! (and profile)
	* start node with trace.js. takes filters and matchers.
15. minimize unnecessary abstraction. abstraction is a part of good design, but if it is overused it can add up and have performance impacts. If you are only handling one thing, try to handle that thing in one place.