<h1 align="center">
    Redux Interview Questions & Answers
</h1>
<p align="center">
    <img src="https://github.com/monkey3310/full-stack-interview/blob/master/assets/redux.png" alt="Redux Interview Questions & Answers" width="200"/>
</p>

_Note: Keep in mind that many of these questions are open-ended and could lead to interesting discussions that tell you more about the person's capabilities than a straight answer would._

### 1. What is the concept of “single source of truth” in Redux?  :star:
<details>
    <summary>
        Answer
    </summary>
        The state of your whole application is stored in an object tree within a single store. That is, there are not multiple stores keeping chunks of the entire state of the web application. Having a single a single store also helps in debugging the app.
</details>

### 2. What are actions in Redux? :star:
<details>
    <summary>
        Answer
    </summary>    
        Actions are plain JavaScript object that describes what happened. They can be thought of as the "intent" to do something. Here are a few example actions:

    
        { type: 'ADD_TODO', text: 'Go to swimming pool' }
        { type: 'TOGGLE_TODO', index: 1 }
        { type: 'SET_VISIBILITY_FILTER', filter: 'SHOW_ALL' }
    
</details>

### 3. Can functions be an action? :star:
<details>
    <summary>
        Answer
    </summary>
    Yes. Libraries like `redux-thunk` allows developers to use functions as actions. 

See [redux-thunk](https://github.com/reduxjs/redux-thunk)
</details>

### 4. What are reducers in Redux? :star:
<details>
    <summary>
        Answer
    </summary>
    Reducers are just pure functions that take the previous state and an action, and return the next state. Example:

    function handleAuth(state, action) {
        return _.assign({}, state, {
            auth: action.payload
        });
    }

</details>

### 5. What is ‘Store’ in Redux? :star:
<details>
    <summary>
        Answer
    </summary>
    Store is the object that holds the application state. It provides a few helper methods to access the state, dispatch actions and register listeners. The entire store is kept in a single JavaScript object.
    Reducers are used to get a new state from an existing state. The new state becomes the store.
</details>

### 6. How is it different from MVC and Flux? :star:
<details>
    <summary>
        Answer
    </summary>
    
</details>

### 7. Why the state is read-only? :star:
<details>
    <summary>
        Answer
    </summary>
    
</details>

### 8. What are action creators and how they differ from actions?  :star:
<details>
    <summary>
        Answer
    </summary>
    
</details>

### 9. What are middlewares in Redux?.  :star:
<details>
    <summary>
        Answer
    </summary>
    
</details>

### 10. Why reducers functions have to be pure? :star:
<details>
    <summary>
        Answer
    </summary>
    
</details>