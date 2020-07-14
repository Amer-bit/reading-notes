# Redux - Additional Topics

#### Other ways to build and manage a Redux store
Redux is great, but there’s a lot of *boilerplate* code that you have write, and every developer or company will have their own internal pattern for putting it all together:
- File and Directory Names
- Reducer and Action Styles
- How do we model our data in the reducers

## Redux Toolkit 
**Purpose**

The Redux Toolkit package is intended to be the standard way to write Redux logic. It was originally created to help address three common concerns about Redux:

* "Configuring a Redux store is too complicated"
* "I have to add a lot of packages to get Redux to do anything useful"
* "Redux requires too much boilerplate code"

#### Redux Toolkit includes these APIs
- *configureStore()*
- *createReducer()*
- *createAction()*
- *createSlice()*
- *createAsyncThunk*
- *createEntityAdapter*


# Alternative State Managers

* MobX
* HookState