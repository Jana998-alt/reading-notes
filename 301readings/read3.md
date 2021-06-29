# Readings: Passing Functions as Props


## React Docs - lists and keys:

**What does .map() return?**

A new array.
**If I want to loop through an array and display each value in JSX, how do I do that in React?**

since _map_ loops through all elements in an array, and excutes the function each time, its easy to include a command in the function that creates elements for each array element. these can be stored in a variable and used later. 

**Each list item needs a unique** __key__.
**What is the purpose of a key?** the purpose of a key is to give each element a unique identity that distinguishes it from other elements.

## What is the spread operator?
**List 4 things that the spread operator can do.**

copying an array, concatenation of arrays, using Math functions, using an array as an argument. 

**Give an example of using the spread operator to combine two arrays.**

```let bigArray = [...arr1, ...arr2]  //this array has the lenth of 2, it has only 2 elements: arr1 and arr2.```
```let bigArray = [...arr1, ...arr2]  //this array has the length of arr1.length+arr2.length```

**Give an example of using the spread operator to add a new item to an array.**

```let arr1 = [1,2,3];```
```let arr2 = [-1,0,...arr1]; // [-1,0,1,2,3]```

**Give an example of using the spread operator to combine two objects into one.**

## How to Pass Functions Between Components

**In the video, what is the first step that the developer does to pass functions between components?**

add the function to the child object.

**In your own words, what does the increment function do?**

increases the number by 1.

**How can you pass a method from a parent component into a child component?**

make a local change in the state of the parent component, then call in in the child element using _this_ keyword.

**How does the child component invoke a method that was passed to it from a parent component?**

through _props_ and _this_ keywords.