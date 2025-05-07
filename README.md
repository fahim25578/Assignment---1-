## What is the use of enums in TypeScript? Provide an example of a numeric and string enum.

In TypeScript, enums are used to represent a set of named constants. They make the code more readable and help avoid using magic numbers or strings directly in your program. Enums are helpful when you have a group of related values that should be treated as a single entity.

### Why use Enums?

In a numeric enum, each member is assigned a number automatically (or manually if you specify the values).

```javascript
enum Day {
  Monday = 1,     // Assigning 1 to Monday
  Tuesday,        // Automatically 2
  Wednesday,      // Automatically 3
  Thursday,       // Automatically 4
  Friday,         // Automatically 5
  Saturday,       // Automatically 6
  Sunday          // Automatically 7

console.log(Day.Monday); // Output: 1
console.log(Day.Friday); // Output: 5

}
```

Here, each day of the week is assigned a numeric value starting from 1 for Monday. The values increase automatically for the following days.

## What is type inference in TypeScript? Why is it helpful?

Type inference is a feature in TypeScript where the compiler automatically determines the type of a variable based on the value it is assigned. In other words, you don't always need to explicitly declare a type for a variable; TypeScript can figure it out for you.

### Why is Type Inference Helpful?

- Less Code to Write: You don't have to specify types every time. TypeScript will infer the type based on the value you give.

- Error Prevention: TypeScript can still catch errors and help prevent bugs by making sure that the value assigned to a variable matches its inferred type.

- Improved Readability: It keeps the code clean and simple without cluttering it with repetitive type declarations.

#### Example of Type Inference:

```javascript
let name = "John"; // TypeScript automatically infers the type as 'string'
```
