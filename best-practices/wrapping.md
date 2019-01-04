## Wrapping Your Widgets
* More Portability
* Better Tests
* Easier Tests
* More Sanity

Note: Wrap it up.  Wrapping widgets is a pattern that we've found to be highly effective for writing easy to maintain and easy to test widgets.  What this means, is that we're using our Web App Builder Widget as a powerful wrapper, giving us access to Web App Builder events, lifecycle, and communication frameworks, while keeping all of our custom functionality in a separate JavaScript API Widget instantiated by the wrapper.  Not only does this help abstract away some of the Web App Builder core functionality, but it means that if you have a non-Web App Builder project that needs the same functionality, you don't need to rewrite the whole thing (or anything for that matter).

---

## Demo
https://github.com/gbochenek/wab-test-example

Note: That's a lot to take in from some presentation slides, so let's take a look at the code.