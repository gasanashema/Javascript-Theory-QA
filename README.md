# Javascript-Theory-QA

## *Begginer Level*

### 1. What is ES6, and how does it differ from ES5?
    
    <aside>
    💡
    
    ES6 and ES5 shows the significant evolution of javascript. ES5 provided stability and best practices where ES6 introduced modern programming features like arrow functions, classes and best variables managent using let and const.
    
    arrow functions eliminating `this` binding issues.
    
    </aside>
    
### 2. What are the key new features introduced in ES6?
    
    <aside>
    💡
    
    1. delclaring variables using let and const
    2. array and object destructuring
    3. promisses
    4. modules
    5. classes
    6. for in and for…of  loops
    7. arrow functions
    8. generators
    9. maps and sets
    10. spread operator and rest operator
    </aside>
    
### 3. What is the difference between `var`, `let`, and `const`?
    
    <aside>
    💡
    
    1. var: are hoisted, can be re declared in the same scope, it’s **function-scoped**. it means it can be accessed before it gets declared
    2. let: they are block scoped, they can not be re declared in the same scope.
    3. const: once assigned can not be re assigned.
    
    `let` and `const` **are hoisted**, but they remain in the "Temporal Dead Zone" until initialized.
    
    </aside>
    
### 4. Explain the concept of **block scope** in ES6.
    
    <aside>
    💡
    
    a variable declared with let is block scoped. it means it can’t be accessed outside the scope it is declared in. `{}`
    
    `let` and `const` are block-scoped
    
    </aside>
    
### 5. What are template literals, and how do they improve string handling?
    
    <aside>
    💡
    
    Template literals ```` are elabled by back-ticks. they are used to write multi-line strings effectively. they also provide the best way of string interpolation (replacing variables in string templates).
    
    **embedding expressions** inside `${}`.
    
    </aside>
    
### 6. What is **destructuring** in ES6? Provide an example.
    
    <aside>
    💡
    
    Destructuring is the practice of extracting array elements or object properties into individual variables.
    
    EX:
    
    `let user = {name:’John’, age:12};`
    
    `let {name,age} = user;`
    
    `console.log(name,age);`
    
    </aside>
    
### 7. How do default function parameters work in ES6?
    
    <aside>
    💡
    
    Default function parameters are used to set default values to arguments. it means is an argument of that parameter is not provided the function takes the default argument provided in parameter definition
    
    could include an **example**
    
    </aside>
    
### 8. What are **arrow functions**, and how are they different from regular functions?
    
    <aside>
    💡
    
    arrow fuctions are introduced in ES6 as the shorthand and the faster way of writing functions. they are created using ⇒ to separate fuction parameters and function definition. they are useful when you want pass a function as a callback.
    
    difference with regular functions:
    
    1. they inherit `this` from its parent scope
    2. the {} are used when the fuction body exceeds one line.
    
    arrow functions **do not have their own `this`**, rather they inherit `this` from their lexical scope.
    
    Single-line expressions implicitly return.
    
    </aside>
    
### 9. What is the **spread operator (`...`)**, and where can it be used?
    
    <aside>
    💡
    
    ~~spread operator is used to spread string into an array, each single character as an array element.~~
    
    it is used to spread an iterable into its elements
    
    it works on **arrays, objects, and function arguments**.
    
    </aside>
    
### 10. What is the **rest parameter**, and how is it different from the spread operator?
    
    <aside>
    💡
    
    the rest parameter is used to show that the fuction will receive the indefinite number of arguments. where as spread operator is used to spread an iterable into its elements.
    
    should **give an example** for clarity.
    
    </aside>
    
### 11. How do you create **multi-line strings** in ES6?
    
    <aside>
    💡
    
    in ES6 to create a multi-line string you use string literals ````
    
    </aside>
    
### 12. Explain the concept of **shorthand object properties**.
    
    <aside>
    💡
    
    object shorthand properties allows you to create properties where each property name exactly matches the name of the variable already defined in the scope.
    
    </aside>
    
### 13. What is the **for...of** loop, and how is it different from **for...in**?
    
    <aside>
    💡
    
    the for…of loop is used to iterate over object values or array values where for…in is used to iterate over object keys or array indexes.
    
    </aside>
    
### 14. How does the `includes()` method work in ES6?
    
    <aside>
    💡
    
    The includes method is used to check if an array contains a certain specified element.
    
    Could mention that **`includes()` is case-sensitive**.
    
    </aside>
    
### 15. What is a **symbol** in ES6, and why is it used?
    
    <aside>
    💡
    
    a symbol is a unique data type that is used to identify properties in objects.
    
    Symbols prevent property name conflicts in objects.
    
    </aside>
    

## *Intermediate level*

### 1. How do **arrow functions** handle `this` differently compared to regular functions?
    
    <aside>
    💡
    
    Regular functions handle this based on how they are called. if they are called with new keyword the this keyword refers to the current object. if not this refers to the global object.
    
    Arrow fuctions inherrits this keyword in its lexical scope
    
    arrow functions don't have their own `this` and instead inherit from the enclosing scope is correct, but an example would help.
    
    </aside>
    
###  2. What are the advantages of using `const` over `let` or `var`?
    
    <aside>
    💡
    
    Use const if you want to prevent a variable to be re-initialized. If your variable has a constant value you can use const to prevent it from being changed.
    
    ex: let pi = 3.17;
    
    let and var are useful to use if a value of that variable will change. but if you want to prevent yourself from mistakely updating you advised to use const
    
    `const` prevents reassignment, but objects and arrays declared with `const` can still have their properties modified.
    
    </aside>
    
###  3. How does ES6 handle default function parameters differently from ES5?
    
    <aside>
    💡
    
    ES6 introduced a the use of default parameters. default parameters are used to assign a default value to the parameter in case no argument passed to it. this is helpful because it prevent some errors that can be caused by leaving an argument for a parameter.
    
    ex:
    
    let myFun = (a=4,b=5) ⇒ a+b;
    
    myFun(2); // output: 7
    
    </aside>
    
### 4. What are **computed property names**, and how are they useful?
    
    <aside>
    💡
    
    Computed property names allows us to use expressions as property names using spuare brackets []. this can be useful if you want to create properties using names from expressions. allows you to have an expression that result in a single value as a property name of an objectl
    
    </aside>
    
5. Explain **object and array destructuring** with examples.
    
    <aside>
    💡
    
    Object and array desctructuring is the act of extracting object or array data into individual variables.
    
    ex:
    
    let user = {name:’john’, age:23}
    
    let {a,b} = user // a will contain user.name and b will contain user.age
    
    </aside>
    
6. What are **rest and spread operators**, and how do they work in function arguments?
    
    <aside>
    💡
    
    rest and spread operators share the same syntax(…). the spread operator is used to spread an iterator into its individual elements. while rest operator is used to indicate that the function will receive indefinite number of arguments as array.
    
    ex: rest operator
    
    let fin = (a,b,…c) // here we showed that c will receive indefinite number of elements.
    
    ex: spread operator
    
    let arr = [1,3,5,6,7,8,4,2,3,3,3,3];
    
    let noDuplicates = new Set(…arr);// the array duplicates will be removed and array will be turned into a set
    
    </aside>
    
7. What is **object shorthand notation**, and when should you use it?
    
    <aside>
    💡
    
    Object shorthand notation is the technique of creating objects where if an object property name matches the variable name declared in scope and the value is the one that the variable holds, you create an object using that variable instead of using the traditional way of creating objects and initialize the created property with that variable.
    
    ex:
    
    let name = ‘john’;
    
    let age = 23;
    
    const obj = {name,age};
    
    </aside>
    
8. How does **parameter destructuring** work in function arguments?
    
    <aside>
    💡
    
    parameter distructuring is the way that javascript allows to distructure arrays or objects that passed to the function as arguments. to do this you have to use the destructuring syntax in parameter definition.
    
    ex:
    
    let myUser = ({name,age}) ⇒ console.log(name,age);
    
    myUser({name:’john’,age:32});//here the object will be distructured
    
    </aside>
    
9. Explain **ES6 modules** (`import` and `export`). How do they compare to CommonJS modules?
    
    <aside>
    💡
    
    ES6 modules allows us to export fuctions or data to be imported and used in other documents. in ES6 we use export to expot the module and import to import the module and be able to use it. in CommonJs we use require keyword to import the module.
    
    </aside>
    
10. What is a **Promise** in ES6, and how does it help in handling asynchronous operations?
    
    <aside>
    💡
    
    A promise is an object that is used to identify the eventual completion or failure of asynchronous operation and its resultant value. the promise identifies the status of the asynchronous operations. the status can be pending,successful of failed. when the operation is successful the resolved method is returned and when the operation is failed the reject method is returned. the promisse receives a callback with two arguments. resolve and reject. promises made it easier to handle asynchronous operations than the use of callbacks. promisses avoided the problem of nesting too many calbacks (callback hell).
    
    example of a promise:
    
    let data = new Promise((resolve,reject)⇒{
    
    resolve(’hello’);
    
    })
    
    </aside>
    
11. What are the different **Promise states**?
    
    <aside>
    💡
    
    a Promise has three states
    
    - Pending: this shows that the operation is still going on it is not yet fullfiled of failed
    - Resolved: this shows that the operation is successful and returns the successful value (here the resolve method is called)
    - Rejected: this shows that the opetation is failed. here the reject method is invoked.
    </aside>
    
12. How does **Promise chaining** work?
    
    <aside>
    💡
    
    Promise chaining is the technique of executing asychronous operations sequentialy. this makes it easier to write maintainable codes because the then function returns a new promise this allows to execute asynchronous operations sequentially and effectively
    
    </aside>
    
13. What is `Promise.all()` and `Promise.race()`?
    
    <aside>
    💡
    
    Promise.all() resolves if all passed promisses are resolved. if one promise rejects, promise.all() also rejects.
    
    Promise.race() revolves if one of the passed promisses resolves. it doesn’t have to wait for others to resolve. it rejects if all rejects.
    
    </aside>
    
14. What is a **WeakMap**, and how is it different from a **Map**?
    
    <aside>
    💡
    
    WeakMap uses objects as property keys. on a map all datatypes can be used as property keys.
    
    WeakMap can’t be iterated over. Map can be iterated over using forEach,for…of,keys(),values().
    
    weakmap does not have property but on map you can identify the size using size property.
    
    </aside>
    
15. What is a **WeakSet**, and how does it differ from a **Set**?
    
    <aside>
    💡
    
    A weakset can only contain objects. other primitive datatypes like number,interger can’t be stored in the weakset. where a set can contain all types of data.
    
    Weakset is not iterable but a set is iterable
    
    weakset has no size property to determine the size of a set. but on a set we can determine its size using size property.
    
    </aside>
    
16. What is the purpose of the `Array.from()` method in ES6?
    
    <aside>
    💡
    
    is used to create an array from an iterable like a nodelist or an html collection
    
    </aside>
    
17. How does `Object.assign()` work in ES6?
    
    <aside>
    💡
    
    is used to crate an object from a prototype
    
    </aside>
    
18. What are **tagged template literals**, and how do they work?
    
    <aside>
    💡
    
    i dont know give the answer
    
    </aside>
    
19. Explain **generators** in ES6 and how they differ from regular functions.
    
    <aside>
    💡
    
    generators are types of functions that allows us to pause function exection. they use yield keyword to return the value. they are declared using functio*
    
    </aside>
    
20. What is `Array.prototype.find()` and how is it different from `filter()`?
    
    <aside>
    💡
    
    find is used to return elemets that fulfils the condition while filter is used to return the array of elements that fulfils conditions
    
    </aside>
    

## *Advanced level*

###  1. What are **proxies** in ES6, and how do they work?
    
    <aside>
    💡
    
    Proxies are objects that are used to intercept and to customise how other objects are accessed. They can have getters and setter to control how properties of an object are accessed. they are created using Proxy constructor. it receives the tagetted object and the handler to be executed on that target.
    
    </aside>
    
### 2. What is the purpose of **Reflect API** in ES6?
    
    <aside>
    💡
    
    Reflect API provides the easy way of interacting with objects. it provides methods get and set similar to those provided by Proxy API to allow us to manipulate the object. the advantage if it over traditional way of accessing an object is that it returns true when the activity went well and false when the activity fails.
    
    </aside>
    
### 3. How does **tail call optimization** work in ES6?
    
    <aside>
    💡
    
    It is a technique where a recursive function calls in tail position. this prevents addional stack frames and memory usage reduction
    
    </aside>
    
### 4. Explain the differences between `Promise.all()`, `Promise.allSettled()`, and `Promise.race()`.
    
    <aside>
    💡
    
    promise.all() resolves if all passed promises are resolved. it means it waits for all to resolve. promise.allSettled() receives array of promises and resolves if all promises are settled (fulfilled or rejected), it does never rejects. promise.race() resolves if atleast a single promise in passed promises resolves.  
    
    </aside>
    
### 5. What is **async/await**, and how does it improve working with Promises?
    
    <aside>
    💡
    
    async/await makes working promises easier by allowing asynchronous codes to be written in  a way that looks synchronous. this improves readability
    
    </aside>
    
### 6. How does `async/await` handle errors, and how is it different from `.catch()` in Promises?
    
    <aside>
    💡
    
    async/await can handle errors using try and catch technique. where as .catch() executes only when a promise rejects.
    
    </aside>
    
### 7. Explain **private properties and methods** in ES6 classes.