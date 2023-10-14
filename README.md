# contextmenu_api
This will help to pause data between all sources under the root file for data access, change and read states as well.

**Using Proccess:**
1. Download the CreateContext.js file and take to your project.
2. create a context
    `const CreateContext = CreateContext();
    export default CreateContext;`
   
in react: `const CreateContext = React.CreateContext();`

3. There you have to parts Provider & Consumer.
4. Import the file to the root file. Suppose
   App.js
   |-Counter.js
   |-ComponentA.js
   |-ComponentB.js
   |-ComponentC.js
Now wrap parent with Context Provider && Provide a value of the context as prop. In this Case it's App.js. Like this

      `import CreateContext from './CreateContext';
       <CreateContext.Provider value={{count:0, inCrementCount:  functionName } } >
            <App.js/>
       </CounterContext.Provider>`

6. Consumer follows the render prop pattern:
7. 
  ` import CreateContext from './CreateContext';
   <CreateContext.Consumer>
     ({count,functionName})=>{ <counter count={count} inCrementCount = {functionName}   />}
   </CounterContext.Consumer>`

`**Hope that will help to developer application better.**`






   
