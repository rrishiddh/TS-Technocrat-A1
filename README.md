# Blog Post

Here are 3 common questions of TypeScript:

### 01 - How does TypeScript help in improving code quality and project maintainability?
 TypeScript is basically a superset of JavaScript. So TypeScript includes all features of JS and added additional feature like type declaration- which catches type-related errors during development, preventing runtime bugs. It actually helps the developer to maintain and understand the type of data specially in large level project. Also the code editor provides more accurate suggestions and catches the error quickly.

However TypeScript code is transpiled into JavaScript before it can be executed, because the browser don't understand ts code. In the transpilation process it removes the TypeScript-specific syntax and generates standard JavaScript code that can be run in any JavaScript environment.


### 02 - What are some differences between interfaces and types in TypeScript?
 Interface and Types both helps to define the structure of objects. Interfaces can be redeclared multiple times with the same name and TypeScript will merge their declarations. Types can define aliases for any kind of type, including primitives, unions, intersections and tuples. But unlike Interface- Types cannot be extended through new declarations.
 We use interfaces for defining the shape of objects, especially when we want to take advantage of declaration merging. And we use types for everything else, including primitives, unions, intersections and when we want to define a type alias.

 ### 03 - What is the use of enums in TypeScript? Provide an example of a numeric and string enum.
 The abbreviation "enum" stands for "enumeration". Its a feature in TypeScript that allows developers to define a set of named constants, which are essentially named values that cannot be changed.
 Enums provide descriptive names for values, making code easier to understand compared to using raw numbers or strings. It also easier to manage and update those values. Enums enforce a set of valid values, preventing the use of incorrect values.
  
  Example of a numeric enum:

  ```
  enum Day {
  Monday,
  Tuesday,
  Wednesday,
  Thursday,
  Friday,
  Saturday,
  Sunday
}
```
  Example of a string enum:
```
enum Status {
  Active = "ACTIVE",
  Inactive = "INACTIVE",
  Pending = "PENDING"
}
```
