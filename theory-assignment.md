
# `Learn React With Harshi` Series 
   Documenting my learning journey of [Namaste React Live Course](https://learn.namastedev.com/) conducted by Akshay Saini
## Theory Assignment: `Chapter - 04 Talk is cheap, show me in code` (07/01/2023)

1. Is JSX mandatory for React ? 
   `JSX` is not a requirement for using React. Each JSX element is just syntactic sugar for calling `React.createElement(component, props, ...children)`. So, anything you can do with JSX can also be done with just plain JavaScript.

2. Is ES6 mandatory for React ? 
   ES6 is `not mandatory` for using React but highly recommendable to use ES6. Any javascript expressions (pure js) can be used in JSX to render React elements. 

   Currently, lot of React projects use ES6 features in React ecosystem, so it's better to have knowledge on ES6 features like modules, destructuring, spread operator, template literals, classes, map, filter and reduce array methods.

3. `{ TitleComponent }` vs `{ <TitleComponent /> }` vs `{ <TitleComponent> </TitleComponent> }` in JSX  

   `{ TitleComponent }` - This value in jsx is considered as jsx expression or variable. If no such variable is present, no output will be shown in the browser. Console throws the following warning
   ```
   index.js:1 Warning: Functions are not valid as a React child. This may happen if you return a Component instead of <Component /> from render. Or maybe you meant to call this function rather than return it.
  
   ```

   `{ <TitleComponent /> }` - This value in jsx is meant for rendering a component (i.e) function that return jsx. This is self closing tag.
   
   `{ <TitleComponent> </TitleComponent> }` - This is same as `{ <TitleComponent /> }` if there are no child inside TitleComponent. If there are children, then those values come inside   `{ <TitleComponent>} ` and `</TitleComponent> }`. 
   

4. How can I write comments in jsx ?
  
   Comments are written like anyother javascript code. In javascript, we use `//` to comment a single line and `/*  */` to comment multiple lines. 

   Similar, in jsx we enclose js code inside {} and hence comments are also enclosed within { } . Only difference is for single line comment instead of `{//}` use `{/* */ }`

   ```
   const Header = () => {
      return ( 
         <h1>Namaste React</h1> { /* This is single line comment */}
         {/*
         *
         * This is multi line comments
         *
         */} 
      )
   }
   ```
   
5. What is <React.Fragment></React.Fragment> and <></> ?
   Each jsx element can have only one parent. This is because jsx element is converted to React.createElement(parent, props, ...children) so there can only be one parent. 

   But there can be situations were we don't have a parent element. In such cases, those elements are enclosed within <div></div> tags just for this purpose. If we don't need to use div just for this purpose, we can use `React.Fragment` component or `<> </>` to enclose those elements 

   
6. What is virtual DOM ?
   Virtual DOM is a copy/visual representaion of DOM tree. 

7. What is Reconciliation in react ?
   React Reconciliation -> React uses diff Algorithm to diff one tree (actually dom) from another which determines what needs to be updated and only re-renders the diff 

8. What is React Fiber ?

9. Why do we need key in React ? When do we need keys in React ?

10. Can we use indes as key in react ?

11. What are props in React ? Ways to use props ?

12. What is Config driven UI ?



