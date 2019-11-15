# Typescript Playground

<!-- Description - What this document is about -->
___

## Index
- [Features](#features)
    - [Type annotations](#type-annotation)
    - [Interfaces](#interfaces)
- [Code snippets](#code-snippets)
- [Best practices](#best-practices)
- [Resources Over Web](#resources)
- [To do list](#to-do)

___


---

## Features<a name="features"></a>

### Type annotation:<a name="type-annotation"></a> 
Type annotations in TypeScript are lightweight ways to record the intended contract of the function or variable.

[Find code here - Stackblitz](https://stackblitz.com/edit/typescript-type-annotation)

```javascript 

// Javascript Function: Without Type Annotation
function greet(partOfDay){
  greeting = `Good ${partOfDay}`;           
}
greet('Morning');                           // Good Morning

// Typescript: Type Annotation
function greetTA(partOfDay:string){
  greeting = `Good ${partOfDay}`;           
}
greetTA('Morning');                         // Good Morning
greetTA([0,1,2]);                           // Good 0,1,2 || Error:  Argument                                               of type 'number[]' is not assignable to parameter of type 'string'.

```
### Interfaces:<a name="interfaces"></a>
An interface in TypeScript contains only the declaration of the methods and properties, but not the implementation. It is the responsibility of the class that __implements__ the interface by providing the implementation for all the members of the interface.

In TypeScript, two types are compatible if their internal structure is compatible. 

[Find code here - Stackblitz](https://stackblitz.com/edit/typescript-interfacess)

```javascript
//Creating interface
interface Person {
  firstName: string;
  lastName: string;
}

// Argument has type annotation of type interface created above
function greet(person: Person) {
  greeting = `Good Morning ${person.firstName} ${person.lastName}`;
}

greet({firstName: 'John', lastName: 'Carter'});// Correct
greet({firstName: 'John'});// Wrong, ERROR
```

---

## Code Snippets<a name="code-snippets"></a>

1. __Install  & transpile typescript:__

```javascript
// Install typescript
npm install -g typescript

// Transpile typescript to javascript
tsc filename.ts
```

---

## Best Practices<a name="best-practices"></a>

1. <!-- link/list the best practices related to this -->

---

## Resources Over Web<a name="resources"></a>

1. [Typescript-Official: Typescript in five minutes](#https://www.typescriptlang.org/docs/handbook/typescript-in-5-minutes.html)
2. 

---

## To do list<a name="to-do"></a>

1. <!-- list of the to do points about this document, till the document is not completed -->
