<h1 align="center">Functions</h1>

Functions is a block code that has instructions for execute some statement.
We can use to perform a task, like calculate a math question, or maybe call some API to fetch any data that you need to use on the front-end. You have infinite possible cases!

### The function definition consistes:

- A name for the function;
- Parameters that can or not exist. Parameters are separated by commas. Also can be enclosed in curly brackets, { }.
- Arguments. An argument is understood as everything that is passed as a parameter when the function is called;

```
function fullName(name, lastname) {
  return "My name is " + name + " " + lastname
}

fullName("John", "Victor");
```

### So, knowing this we have:

<br>

- A function declaration:

```
  function fullName() {...}
```

- A function name:

```
  fullName
```

- A function return:

```
  return "My name is " + name + " " + lastname
```

- The function parameters:

```
  (name, lastname)
```

- The function arguments:

```
  ("John", "Victor")
```

- The function call:

```
  fullName("John", "Victor")
```

- The function scope:

```
       {...}
```

<br>

## Curious things: Arrow function

<br>

Arrow function has a short syntax than a function expression and doesn't have its own argument. These functions expression are better applied to a function that don't be methods and can't be used as constructors.

As names says, arrow function can be identified by arrow formart

```

function displayColor(color) {
  console.log(color);
}

// Also can be written as an arrow
const displayColor = ( color ) => {
  console.log(color);
}

```

Another example:

```
const cardinalNumbers = [1, 2, 3, 4, 5, 6, 7];

cardinalNumbers.map(number => { console.log(number) })
```
