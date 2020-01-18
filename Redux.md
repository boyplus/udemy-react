# Udemy-Redux
###Chapter 12: "Basic Redux by itself"

**What is redux**

- redux is state management library
- Make creating complex application easier
- Not require to create a react app
- Not explicity disign to work with react



**Redux cycle**

- Action creator (Person dropping of the form)
- Action (the form)
- Dispatch (form reciver)
- Reducers (Departments)
- State (Compiled department data)



**1.Action creators**

-> the function which return palin javascript object

```javascript
const createPolicy = (name,amount) =>{
  return {
    //action (javascript object)
  };
}
```





**2.Action**

->  it is the **object** which represents things that we want to do and data in it.

-> consits of two parts

- **type**  (type of action Ex. CREATE_POLICY, we usually make it uppercase)
- **payload**  (data in action ex. name, amount)



**3.Dispatch**

-> to update the data in store which pass argument of action creatots

-> we usually do this in the last step, because we have to write the action creators, actions, reducers, combineReducers and create the store

```javascript
const store = createStore(ourDepartments);
store.dispatch(createPolicy('Alex',20));
console.log(store.getState());
```



**4.Reducers**

-> it's the modifier function to change and return the new data

-> it recieve two arguments, first one is the old data from store and second one is action (form)

-> we have to check what type of the action, then we consider what we will do about that type of action
























