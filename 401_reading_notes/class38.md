# Redux - Asynchronous Actions
By default actions in Redux are dispatched synchronously, which is a problem for any non-trivial app that needs to communicate with an external API or perform side effects. Redux allows for middleware that sits between an action being dispatched and the action reaching the reducers. There are two very popular middleware libraries that allow for side effects and asynchronous actions: **Redux Thunk and Redux Saga**.

## Redux Thunk
Redux Thunk is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store’s dispatch method, which is then used to dispatch regular synchronous actions inside the body of the function once the asynchronous operations have completed.

Thunks are the recommended middleware for **basic Redux side effects logic**, **including complex synchronous logic that needs access to the store, and simple async logic like AJAX requests.**

The most common use-case for Redux Thunk is for communicating asynchronously with an external API to retrieve or save data. Redux Thunk makes it easy to dispatch actions that follow the lifecycle of a request to an external API.
