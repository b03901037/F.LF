# Project F
[http://project--f.blogspot.com/](http://project--f.blogspot.com/)

## About
The core component of Project F used to build browser based fighter games.
F.core is not an engine. F.core is a set of conceptual and functional systems that can be used to build an engine.

## Components and features

### sprite
- display and control sprites on page using `<div>` and `<img>` tag
- **not** using canvas for sprite animations
- support CSS 2d transform

### animator
- animate sprites
- support multiple animation sequence on the same image

### controller
- controllers for multiple players on the same keyboard
- maintains a table of key states of interest
- generate key events for 'child' controllers
- buffered mode: buffer inputs and fetch only once a loop
- never drops keys

### combodec
- listen key events and detect combo from a controller
- maintains a clean sequence of pressed keys and fire events when combo is detected
- King of Fighter style combos
- eliminating auto-repeated keys

### controller-recorder
- record and playback activity of a controller
- useful in game demo and testing

### states
- nested state transition system, a Hierarchical State Machine ( HSM )
- intuitive state machine definition syntax
- simple (not UML compatible) yet powerful enough for interactive gaming
- reduces logical bugs if used as a programming paradigm

### states_simple
- non-nested state transition system, a traditional finite state machine ( FSM )

### collision
- performing rectangle-rectangle, triangle-triangle, circle-circle, line-line intersect tests
and point in rectangle test

### graph
- mapping(hashing) objects in finite 2d space into a 2d array

### math
- some useful vector operations

### web development practices
- use [requirejs](http://requirejs.org/) for dependency management
- compile-time optimization

## Sample usages
- [support.html](http://tyt2y3.github.com/F.core/sample/support.html)
- [states.html](http://tyt2y3.github.com/F.core/sample/states.html)
- [sprite.html](http://tyt2y3.github.com/F.core/sample/sprite.html)
- [graph.html](http://tyt2y3.github.com/F.core/sample/graph.html)
- [controller.html](http://tyt2y3.github.com/F.core/sample/controller.html)
- [combo.html](http://tyt2y3.github.com/F.core/sample/combo.html)
- [collision.html](http://tyt2y3.github.com/F.core/sample/collision.html)
- [effects-pool.html](http://tyt2y3.github.com/F.core/sample/effects-pool.html)
- [world.html](http://tyt2y3.github.com/F.core/sample/world.html)

## File list
[`support.js`](support.js)	[`states.js`](states.js)	[`world.js`](world.js)	[`util.js`](util.js)	[`style.css`](style.css)	[`states_simple.js`](states_simple.js)	[`sprite.js`](sprite.js)	[`require.js`](require.js)	[`readme.md`](readme.md)	[`math.js`](math.js)	[`license.html`](license.html)	[`graph.js`](graph.js)	[`css.js`](css.js)	[`css-build.js`](css-build.js)	[`controller.js`](controller.js)	[`controller-recorder.js`](controller-recorder.js)	[`combodec.js`](combodec.js)	[`collision.js`](collision.js)	[`animator.js`](animator.js)	[`.gitattributes`](.gitattributes)	[`effects-pool.js`](effects-pool.js)	

## License
Generally has complete freedom except for profit- making. For exact terms see [license](http://project--f.blogspot.hk/2012/05/license.html).
