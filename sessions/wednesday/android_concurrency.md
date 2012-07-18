# Concurrency with Android

## Resources

** Notes **: https://github.com/bmeike/OSCON

git clone git://github.com/bmeike/OSCON.git


## Note on memory usage - Laptops v Mobile

On laptops, there's an assumption that when an application has stopped doing anything useful, it goes to swap to free up RAM. This is not true with mobile devices. Whether in use or not, RAM is in use.

## Concurrency Tools

check out: FourTrains book on Java concurrency

if you maintain a mutable state across more than one thread you must maintain one lock

### Async Tasks

Point is to get short running tasks off of the UI thread. As noted yesterday, do __not__ sit on the UI thread.

Note: After 'Honeycomb' order of execution is FIFO, before it there is no guaranteed order to the dequeuing of AsyncTasks

1. onPreExecute
2. doInBackgrond
3. onPostExecute

An Activity has a very different lifecycle than an AsyncTask. For example, if you change orientation of the device, the Activity is destroyed and another is created.

If an AsyncTask has a handle to the Activity, the Activity cannot be garbage collected, and Activities must be able to be garbage collected at any time.

Don't pass collections to AsyncTasks. Collections are mutable - do not use mutable objects. You can pass a copy of a collection, but not the collection itself.

Watch out for lifecycles: don't reference services, activities, or anything else that does not have the same lifecycle as your task.

Ctrl-F11 for testing. It goes through the full lifecycle.

## Conclusion

** Ran out of session time. Check the repo notes. **