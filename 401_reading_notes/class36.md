# Application State with Redux
*Redux* is a predictable state container for JavaScript apps. It helps you write applications that behave consistently, run in different environments (client, server, and native), and are easy to test. On top of that, it provides a great developer experience, such as live code editing combined with a time traveling debugger.

### Why use Redux?
-  in larger apps with a lot of moving pieces, state management becomes a huge concern. Redux ticks that off quite well without performance concerns or trading off testability.
- Redux include logging, hot reloading, time travel, universal apps, record and replay — all without doing so much.
### Redux principles
- *Single source of truth :*
The global state of your application is stored in an object tree within a single store.
- *State is read-only :*
The only way to change the state is to emit an action, an object describing what happened.
- *Changes are made with pure functions :*
To specify how the state tree is transformed by actions, you write pure reducers.