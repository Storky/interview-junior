# Redux


## 1. What is Redux
Redux is a predictable state container for JavaScript apps.

## 2. Main Redux entities.
#### action, dispatcher, store, middleware, reducer
### - Что такое экшн?
= экшн это объект, 
= action Creator - ф-я, которая создает экшн

## 3. Select and call methods
Its in Redux Saga
- **Select** - get a store in saga
- **Call** -  call the function fn with args as arguments

## 4. How store works
### - что такое стор и как работает?

= стор это объект
    -содержит состояние приложения (application state);
    -предоставляет доступ к состоянию с помощью getState();
    -предоставляет возможность обновления состояния с
	 помощью dispatch(action);
    -Обрабатывает отмену регистрации слушателей с 
	 помощью функции, возвращаемой subscribe(listener).


## 5. What is middleware
- a snippet of code that provides a third-party extension point between dispatching an action and the moment it reaches the reducers.

## 6. Redux optimisation (reselect)

#### React Context

#### Reselect
- Selectors can compute derived data, allowing Redux to store the minimal possible state.
- Selectors are efficient. A selector is not recomputed unless one of its arguments changes.
- Selectors are composable. They can be used as input to other selectors.

## 7. Where to place async logic

In the middleware

Redux middleware were designed to enable writing logic that has side effects.
Redux middleware can do anything when it sees a dispatched action: log something, modify the action, delay the action, make an async call, and more. 

