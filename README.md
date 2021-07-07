# Table Of Content
- [Table Of Content](#table-of-content)
- [NEW WAYS OF DECLARING VARIABLES](#new-ways-of-declaring-variables)
- [REPLACE **'FOR'** LOOPS WITH **'MAP'**](#replace-for-loops-with-map)
- [REPLACE **'FOR'** LOOPS WITH **'FILTER'**](#replace-for-loops-with-filter)
- [REPLACE **'FOR'** LOOPS WITH **'REDUCE'**](#replace-for-loops-with-reduce)
- [SERVER-SIDE JAVASCRIPT WITH NODE.JS](#server-side-javascript-with-nodejs)
- [NPM: THE WORLD'S LARGEST PACKAGE MANAGER](#npm-the-worlds-largest-package-manager)
- [ANGULAR AND REACT](#angular-and-react)
- [REDUX: STATE MANAGEMENT FOR ALL](#redux-state-management-for-all)
- [SEMICOLONS ARE OPTIONAL](#semicolons-are-optional)
- [ESLint](#eslint)



# NEW WAYS OF DECLARING VARIABLES

ES2015 introduced two new way of declaring variables: **let** and **const**.

- **'let'** is used when a variable will be reassigned.
- **'const'** is used when we need to keep a variable protected from being reassigned.

**Note: 'const' does not freeze arrays and objects and it doesn't stop properties from being mutated or changed.**

The main benefit of using **'let'** and **'const'** over **'var'** is that when using var our code gets scoped to the top of current function, therefore making the variable available to whole function. Therefore, with the use of **'let'** and **'const'**, we do not need to worry about the variable scope leaking outside.

# REPLACE **'FOR'** LOOPS WITH **'MAP'**

Suppose, we have an array of numbers and we need to produce another array by doubling all the numbers in the array.
The first solution that comes into our mind is to\ 
- **declare an empty array**
- **write a for loop**
- **append a number in the second array by looking up the index on first array by doubling the number**

But we have a more simple and easier solution by mapping the array to another array:\
- **[1,2,3,4].map((num) => num * 2); //Output: [2,4,6,8]**

# REPLACE **'FOR'** LOOPS WITH **'FILTER'**

Suppose, we have an array of numbers and we need to produce another array that contains only the even number from the first array.
The first solution that comes into our mind is to\ 
- **declare an empty array**
- **write a for loop**
- **write an if statement to check if the number at given index is even**

Or, we could simply use the **filter** method:\
- **[1,2,3,4,5,6].filter((num) => num % 2 === 0); //Output: [2,4,6]**


# REPLACE **'FOR'** LOOPS WITH **'REDUCE'**
Suppose, we need to calculate the sum of all numbers in the array.
The first solution that comes into our mind is to\
- **declare a variable initializing its initial value to Zero**
- **write a for loop that takes each number and adds the value to our created variable**

Or, We can simply use **reduce** method:\
- **[1,2,3,4,5,6].reduce((a,b) => a + b); //Output: 21**

- **This method takes first two elements as parameter and adds them and reduces the element and so on.**

# SERVER-SIDE JAVASCRIPT WITH NODE.JS 
Node.js allows JavaScript to be used on the server side. With the use of Node.Js, we do not have to change the language when switching back and forth between client and server code. It also allows libraries to be shared between the code and the server which decreases the amount of duplicate code one has to write.

# NPM: THE WORLD'S LARGEST PACKAGE MANAGER
The Node Package Manager is the biggest package manager in the world plus the level of collaboration that happens within the community makes writing and application much more convenient for us. With the rise of NPM, increasing number of developers are getting rid of alternative solutions and simply sticking with NPM for everything.

# ANGULAR AND REACT
Angular is a framework maintained by Google along with open-source community. Recent versions of Angular have taken things to a next level, transforming Angular into a full platform that allows development of not only web UIs but also native mobile applications development and more.\
It has strong opinions on how applications are structured, which can make it difficult to learn. It also makes use of **TypeScript** - a superset of JavaScript that allows the use of typed values. Unlike React, Angular uses two-way bindings, which allows user input to directly change the state. This makes data easier to manage.

React is a view library maintained by the Facebook engineering team. Applications written with React carry a component-based architecture, keeping things small and composable. It often adopts functional paradigms to solve problems. Applications are built using individual components, which hold information about themselves in a state object. The way an application displays depends purely on these states.\
Unlike most front-end frameworks, React only provides the view layer of an application. The rest can be pieced together based on the needs of your project. Separate packages can deal with the likes of routing and form creation on React's behalf.

You will often hear a dispute between Angular and React developers on which is a better framework but that is up to you to decide on what suits you the most.

# REDUX: STATE MANAGEMENT FOR ALL
Redux Library helps us to keep up with the application's state while writing a dynamic user interfaces. Redux is commonly used alongside React and is slowly adopted by the Angular community. If we are writing a large application, we should be using Redux from get-go since it helps us to write applications that behave consistently and offers great developer experience.

# SEMICOLONS ARE OPTIONAL
The official specification of JavaScript language has a feature called automatic semicolon insertion that has caused riots within the community. Most of the developers are now dropping semicolons in their JavaScript code, mostly due to personal preference. If that's something you are interested in doing, make sure to use a code linter such as **ESLint** to help you avoid some bugs.

# ESLint
As JavaScript is a loosely typed language, perfectly valid code also can cause unexpected problems. ESLint is a tool that can check through our files for common issues that we might not have intended. By running ESlint, it checks all JavaScript files in the project directory. All that is required is a **.eslintrc** configuration file that details the rules to follow. 