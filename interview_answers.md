# Interview Answers
Be prepared to demonstrate your understanding of this week's concepts by answering questions on the following topics. These will not be counted as a part of your sprint score but will be helpful for preparing you for your endorsement interview, and enhancing overall understanding.

1. What problem does the context API help solve?
Context API allows state under a given parent that's wrapped in Provider to access state without prop drilling.

2. In your own words, describe `actions`, `reducers` and the `store` and their role in Redux. What does each piece do? Why is the store known as a 'single source of truth' in a redux application?
The store holds state that's available to the entire app (or whatever parent componenet and on down). Actions handle various events within the application and dispatch the correct case in a reducer. Reducers take the data passed by the action and use it to update state. 

3. What does `redux-thunk` allow us to do? How does it change our `action-creators`?
It intercepts data between the action and the reducer. It allows us to either pass it on unchanged, stop it altogether, or manipulate the data before being passed to hte reducer. It allows redux to run asyncronous updates like api calls.

4. What is your favorite state management system you've learned and this sprint? Please explain why!
Context for simple applications. Redux for ones that have lots of slices of state and require various slices of state in multiple different branches of a component tree. 