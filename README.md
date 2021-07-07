- [New Ways of Declaring Variables](#new-ways-of-declaring-variables)
    - [**'let'** is used when a variable will be reasigned.](#let-is-used-when-a-variable-will-be-reasigned)
    - [**'const'** is used when we need to keep a variable protected from being reasigned.](#const-is-used-when-we-need-to-keep-a-variable-protected-from-being-reasigned)
  - [Note: **'const'** does not freeze arrays and objects and it doesn't stop properties from being mutated or changed.](#note-const-does-not-freeze-arrays-and-objects-and-it-doesnt-stop-properties-from-being-mutated-or-changed)
- [Replace **'for'** loops with **'map'**](#replace-for-loops-with-map)
- [Replace **'for'** loops with **'filter'**](#replace-for-loops-with-filter)
- [Replace **'for'** loops with **'reduce'**](#replace-for-loops-with-reduce)
- [Server-Side JavaScript with Node.JS](#server-side-javascript-with-nodejs)
- [NPM: The World's Largest Package Manager](#npm-the-worlds-largest-package-manager)
- [Angular and React](#angular-and-react)
- [Redux: State Management for all](#redux-state-management-for-all)



# New Ways of Declaring Variables

ES2015 introduced two new way of declaring variables: **let** and **const**.

### **'let'** is used when a variable will be reasigned.
### **'const'** is used when we need to keep a variable protected from being reasigned.

## Note: **'const'** does not freeze arrays and objects and it doesn't stop properties from being mutated or changed.

The main benefit of using **'let'** and **'const'** over **'var'** is that when using var our code gets scoped to the top of current function, therefore making the variable available to whole function. Therefore, with the use of **'let'** and **'const'**, we do not need to worry about the variable scope leaking outside.

# Replace **'for'** loops with **'map'**

Suppose, we have an array of numbers and we need to produce another array by doubling all the numbers in the array.
The first solution that comes into our mind is to\ 
**declare an empty array**\
**write a for loop**\
**append a number in the second array by looking up the index on first array by doubling the number**

But we have a more simple and easier solution by mapping the array to another arrray:\
**[1,2,3,4].map((num) => num * 2); //Output: [2,4,6,8]**

# Replace **'for'** loops with **'filter'**

Suppose, we have an array of numbers and we need to produce another array that contains only the even number from the first array.
The first solution that comes into our mind is to\ 
**declare an empty array**\
**write a for loop**\
**write an if statement to check if the number at given index is even**

Or, we could simply use the **filter** method:\
**[1,2,3,4,5,6].filter((num) => num % 2 === 0); //Output: [2,4,6]**


# Replace **'for'** loops with **'reduce'**
Suppose, we need to calculate the sum of all numbers in the array.
The first solution that comes into our mind is to\
**declare a variable initializing its initial value to Zero**\
**write a for loop that takes each number and adds the value to our created variable**

Or, We can simply use **reduce** method:\
**[1,2,3,4,5,6].reduce((a,b) => a + b); //Output: 21**

**This method takes first two elements as parameter and adds them and reduces the element and so on.**

# Server-Side JavaScript with Node.JS 
Node.js allows JavaScript to be used on the server side. With the use of Node.Js, we do not have to change the language when switching back and forth between client and server code. It also allows libraries to be shared between the code and the server which decreases the amount of duplicate code one has to write.

# NPM: The World's Largest Package Manager
The Node Package Manager is the biggest package manager in the world plus the level of collaboration that happens within the community makes writing and application much more convenient for us. With the rise of NPM, increasing number of developers are getting rid of alternative solutions and simply sticking with NPM for everything.

# Angular and React
Angular is a framework maintained by Google along with open-source community. Recent versions of Angular have taken things to a next level, transforming Angular into a full platform that allows development of not only web UIs but also native mobile applications development and more.

React is a view library maintained by the Facebook engineering team. Applications written with React carry a component-based architecture, keeping things small and composable. It often adopts functional paradigms to solve problems.

You will often hear a dispute between Angular and React developers on which is a better framework but that is up to you to decide on what suits you the most.

# Redux: State Management for all
Redux Library helps us to keep up with the application's state while writing a dynamic user interfaces. Redux is commonly used alongside React and is slowly adopted by the Angular community. If we are writing a large application, we should be using Redux from get-go since it helps us to write applications that behave consistently and offers great developer experience.
