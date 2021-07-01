# Read05: Putting it all together - React


## Questions

- How would you break a mock into a component heirarchy? 

by for example, drawing boxes on each seperate entity in the mock. 

- What is the single responsibility principle and how does it apply to components?

it means that each component must do only one task.

- What does it mean to build a ‘static’ version of your application?

non-interactive, non-dynamic version. states are not added in this stage.

- Once you have a static application, what do you need to add?

states. 

- What are the three questions you can ask to determine if something is state?

1. Is it passed in from a parent via props? If so, it probably isn’t state.
2. Does it remain unchanged over time? If so, it probably isn’t state.
3. Can you compute it based on any other state or props in your component? If so, it isn’t state.

- How can you identify where state needs to live?

remember that React goes only one-way: parent to child. the state must live in a parent component of all the components that will use it. 

## Things I want to know more about

how is it like to have a 2-way building environment? 
