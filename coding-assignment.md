# `Learn React With Harshi` Series 
   Documenting my learning journey of [Namaste React Live Course](https://learn.namastedev.com/) conducted by Akshay Saini

## Coding Assignment: `Chapter - 04 Talk is cheap, show me in code` (07/01/2023)

### Build a Food Ordering App 

  I am building a food ordering app `InstaFood` with the knowledge learnt through this session. 

## Steps to develop a React App 

Reference : [Thinking in React](https://beta.reactjs.org/learn/thinking-in-react) 

### Step : 1  Break the UI into a component hierarchy 

 - Single responsibility principle, that is, a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.

In our case, the app components are decomposed as follows based on their functionality.

  AppLayout
    Header 
     - Title
     - NavComponent
    Body 
     - SearchComponent
     - RestaurantCard
    Footer 

### Step : 2 Build a static version in React
- The easiest way is to build a version that takes your data model and renders the UI but has no interactivity.
- Use props to pass parent to child component at this stage. Don't use state at this step. State is reserved only for interactivity, that is, data that changes over time
- Use top-down or bottom-up components in the hierarchy. In larger projects, use bottom-up where you start with the inner most component following the hirarchy higher-up. 

In our case,
Implement all features one after another. Build Logo, Nav items in Header, Footer with some text and Body with two components. Use flexbox to design the layout.

Build the static version of restaurant view and restaurant card with hardcoded values. Then, pass data model to it.

In our case, we are using mock data for now which contains information about a list of restaurants. First understand the data model, where can we find the required objects like restaurant name, cuisines, avg rating, delivery time and image in the data hierarchy. 

Once data model is ready, use the data to populate the restaurant view by looping (use array map function ie for each restaurant in the array, tranform the restaurant data into restaurant card by writing jsx). Pass restaurant data as Props to the RestaurantCard

We have successfully implemented few features in this chapter. Other steps will be continued in next chapter. If you are interested, check out this [Chapter-05] (https://github.com/Learn-React-With-Harshi/chapter-05-lets-get-hooked/blob/main/coding-assignment.md)








  



