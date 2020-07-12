# Redux - Combined Reducers
Combined reducers is nothing more than pulling in more than one reducer from source and creating a keyed object from them.

As your app grows more complex, you'll want to **split** your reducing function into separate functions, each managing independent parts of the state.

The combineReducers **helper function** turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.

### Arguments
reducers (Object): An object whose values correspond to different reducing functions that need to be combined into one.

### Returns
(Function): A reducer that invokes every reducer inside the reducers object, and constructs a state object with the same shape.


## Notes

Any reducer passed to combineReducers must satisfy these rules:

* For any action that is not recognized, it must return the state given to it as the first argument.

* It must never return undefined. It is too easy to do this by mistake via an early return statement, so combineReducers throws if you do that instead of letting the error manifest itself somewhere else.

* If the state given to it is undefined, it must return the initial state for this specific reducer. According to the previous rule, the initial state must not be undefined either. It is handy to specify it with ES6 optional arguments syntax, but you can also explicitly check the first argument for being undefined.


While combineReducers attempts to check that your reducers conform to some of these rules, you should remember them, and do your best to follow them. combineReducers will check your reducers by passing undefined to them; this is done even if you specify initial state to Redux.createStore(combineReducers(...), initialState). Therefore, you must ensure your reducers work properly when receiving undefined as state, even if you never intend for them to actually receive undefined in your own code.