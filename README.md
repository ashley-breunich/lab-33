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

###### `CLASS Main -> Provider`
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


#### Tests
* How do you run tests?
* What assertions were made?
* What assertions need to be / should be made?

#### UML
Link to an image of the UML for your application and response to events
