![CF](http://i.imgur.com/7v5ASc8.png) LAB
=================================================

## Lab 33: Remote APIs

### Ashley Breunich

### Links and Resources
* [lab repo](https://github.com/ashley-breunich/lab-33)
* [code sandbox URL](https://codesandbox.io/s/ww7690x92l)

### Modules

#### `index.js`
##### Exported Values and Methods

###### `CLASS Main`
--> App Component

The app component is wrapped in the store allowing the entire program to have access to Redux. 


#### `app.js`
##### Exported Values and Methods

###### `CLASS App`
<-- props

--> GetPeople Component

--> PeopleList Component

--> Modal Component 

The app class manages each component that visually makes up the app. 

###### `mapStateToProps()`
<-- store

--> people, person

###### `mapDispatchToProps()`
<-- dispatch, getState

--> get, getPerson


#### `lib/utils.js`
##### Exported Values and Methods

###### `fetchData()`
<-- URL

--> Superagent get request: results.body


#### `components/getPeople.js`
##### Exported Values and Methods

###### `getPeople()`
<-- props

--> header

###### `mapStateToProps()`
<-- store

--> people, person

###### `mapDispatchToProps()`
<-- dispatch, getState

--> get, getPerson


#### `components/peopleList.js`
##### Exported Values and Methods

###### `peopleList()`
<-- props

--> ul: Each name from the Starwars API

###### `mapStateToProps()`
<-- store

--> people, person

###### `mapDispatchToProps()`
<-- dispatch, getState

--> get, getPerson


#### `components/modal.js`
##### Exported Values and Methods

###### `Modal()`
<-- props

--> div

###### `mapStateToProps()`
<-- store

--> people, person

###### `mapDispatchToProps()`
<-- dispatch, getState

--> get, getPerson


#### `store/middleware/reporter.js`
##### Exported Values and Methods

###### `export default`
<-- store, next, action

--> result (console log of the current state); or an error 


#### `store/middleware/thunk.js`
##### Exported Values and Methods

###### `export default`
<-- store, next, action

--> action(store.dispatch, store.getState)


#### `store/index.js`
##### Exported Values and Methods

###### `export default`
--> people, person

This file creates the stores with the reducers that we declared.


#### `store/people-actions.js`
##### Exported Values and Methods

###### `get()`
<-- url, dispatch

--> data from fetchData() function

###### `dispatchedGet()`
<-- payload

--> type: "GET_PEOPLE"

--> payload


#### `store/peopleReducer.js`
##### Exported Values and Methods

###### `export default`
<-- state, action

--> payload.results OR initialState


#### `store/person-actions.js`
##### Exported Values and Methods

###### `getPersonDetails()`
<-- url, dispatch

--> data from fetchData() function

###### `dispatchedGet()`
<-- payload

--> type: "GET_PERSON"

--> payload


#### `store/personReducer.js`
##### Exported Values and Methods

###### `export default`
<-- state, action

--> payload OR state


#### Tests
* How do you run tests?
* What assertions were made?
* What assertions need to be / should be made?

#### UML
Link to an image of the UML for your application and response to events
