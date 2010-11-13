# SceneGraph.js #

JavaScript implementation of a [Scene Graph](http://en.wikipedia.org/wiki/Scene_graph) (a.k.a. display list) targeting HTML5 canvas rendering.

## Why? ##

 - HTML5 canvas doesn't have a build-in hierarchy tree.
 - JavaScript engines are getting faster each day and HTML canvas is starting to be hardware accelerated in some browsers, which means it could potentially be fast enough for complex interactions.

## Goals / Desired Features ##

 - Translate, rotate, scale elements at runtime (bitmap and/or vectors).
 - Add/remove/swap "nodes" at runtime.
 - Messaging system support (DOM2 Event or Signals).
 - Individual *event* dispatching per element and *bubbling* (maybe without capturing phase).
 - Clean API.
 - Work similar to the DOM Tree and Flash DisplayList when it makes sense.
 - Use same API as native canvas commands when it makes sense.
 - Self-contained.
 - Be fast but without compromising code structure/readability.
 - Favor interfaces over inheritance.
 
## Notes ##

This project is on a initial phase and things aren't really well defined yet, not even sure how far the development will go, still not sure if it will be really useful.

It should be a low-level API and fairly verbose, don't expect it to be anything similar to jQuery/prototype, features like chaining, retrieving elements by id/class probably won't be implemented, the code/API style should be closer to AS3/Java than to Ruby/Python. It should follow the same kind of concepts of the [Flash Display List](http://www.adobe.com/devnet/flash/quickstart/display_list_programming_as3.html) and the [DOM tree](http://www.w3.org/TR/DOM-Level-2-Core/introduction.html). The idea is to provide a core structure that later could be abstracted for specific uses if needed.