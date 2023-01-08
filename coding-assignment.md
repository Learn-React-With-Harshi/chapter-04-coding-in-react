# `Learn React With Harshi` Series 
   Documenting my learning journey of [Namaste React Live Course](https://learn.namastedev.com/) conducted by Akshay Saini

## Coding Assignment: `Chapter - 04 Talk is cheap, show me in code` (07/01/2023)

### Build a Food Ordering App 

  I am building a food ordering app `InstaFood` with the knowledge learnt through this session. 

## Steps to start working on a app 

Thinking in React 

Step : 1  Break the UI into a component hierarchy 

 - Single responsibility principle, that is, a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.

Step : 2 Build a static version in React
- The easiest way is to build a version that takes your data model and renders the UI but has no interactivity.
- Use props to pass parent to chils component at this stage. Don't use state at this step. State is reserved only for interactivity, that is, data that changes over time
- Use top-down or bottom-up components in the hierarchy. In larger projects, use bottom-up where you start with the inner most component following the hirarchy higher-up. 

Step 3: Identify The Minimal (but complete) Representation Of UI State
 - Think of set of mutable state that your app needs (DRY- Don't repeat yourself)

Step 4: Identify where your state should live 
  - Identify every component that renders something based on that state.
  - Find a common owner component (a single component above all the components that need the state in the hierarchy). - this should own the state 

Step : 5 Add Inverse data-flow 

  - Till now , React is one-way binding ( data flow in one direction only and whatever typed in the iinput box will be ignored intentionally )
  - Two-way data binding can be done - whenever the input is chnaged, setState() is called to update the state 
  



  Low level Design : 

  Header 
    - Logo
    - Nav items (Home, Contact, Cart)
  Body 
   - Search 
   - Favourites
   - Restaurant View 
   - Restaurant Card
  Footer 
   - Copyright 

  Components : 
  AppLayout
    Header 
     - Title
     - NavComponent
    Body 
     - RestaurantCard
     - SearchComponent
    Footer 

  



