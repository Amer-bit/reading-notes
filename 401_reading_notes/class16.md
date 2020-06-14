# Event Driven Applications
An event-driven application is a computer program that is written to respond to actions generated by the user or the system. Event-driven systems can be roughly categorized into two types: **reactive ones, and stream processing ones**.

### running event emitter on node app

To run event emitterwe need to require events module 
`const EventEmitter = require('events').EvenEmitter`
`const newEventEmitter = new EventEmitter`

node js core api is built around event driven architecture such that a certain objects emit events to call a function. For instance: a net.Server object emits an event each time a peer connects to it; a fs.ReadStream emits an event when the file is opened; a stream emits an event whenever data is available to be read.

EventEmitter calls all listeners synchronously in the order in which they were registered. This ensures the proper sequencing of events and helps avoid race conditions and logic errors. When appropriate, listener functions can **switch to an asynchronous mode of operation using the setImmediate() or process.nextTick()**.

***Handling events only once***

When a listener is registered using the eventEmitter.on() method, that listener will be invoked every time the named event is emitted.Using the eventEmitter.once() method, it is possible to register a listener that is called at most once for a particular event. Once the event is emitted, the listener is unregistered and then called.

**NOTE**: As a best practice, listeners should always be added for the 'error' events.

**NOTE:** Using async functions with event handlers is problematic, because it can lead to an unhandled rejection in case of a thrown exception

**NOTE:** The 'error' events that are generated by the captureRejections behavior do not have a catch handler to avoid infinite error loops: the recommendation is to not use async functions as 'error' event handlers.



Class: EventEmitter

* Event: 'newListener'
* Event: 'removeListener'
* EventEmitter.listenerCount(emitter, eventName)
* EventEmitter.defaultMaxListeners
* EventEmitter.errorMonitor
* emitter.addListener(eventName, listener)
* emitter.emit(eventName[, ...args])
* emitter.eventNames()
* emitter.getMaxListeners()
* emitter.listenerCount(eventName)
* emitter.listeners(eventName)
* emitter.off(eventName, listener)
* emitter.on(eventName, listener)
* emitter.once(eventName, listener)
* emitter.prependListener(eventName, listener)
* emitter.prependOnceListener(eventName, listener)
* emitter.removeAllListeners([eventName])
* emitter.removeListener(eventName, listener)
* emitter.setMaxListeners(n)
* emitter.rawListeners(eventName)
* emitter[Symbol.for('nodejs.rejection')](err, eventName[, ...args])