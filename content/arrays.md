<h1 align="center"> Arrays </h1>

## About

Arrays are similar objects to the list that has a lot of methods for executing some operations. Arrays can be used to store data list, like numbers, text, objects, functions, and the other things.

<br>

## Creating an array

Arrays can be initialized with two ways (But is the same)

```
  const colors = new Array();

  // colors: []
```

```
  const colors = [];

  // colors: []
```

<br>

## Adding values on array

Set values on the array are more easy, follow example.

```
  const colors = new Array();

  colors.push("Red");
  colors.push("Green");
  colors.push("Blue");

  // colors: ["Red", "Green", "Blue"];
```

We can also add a value a specific location, but this can be a headache if you use wrong

```
  const colors = new Array();

  colors.push("Red");
  colors.push("Green");
  colors.push("Blue");

  colors[1] = "Yellow"

  // colors: ["Red", "Yellow", "Blue"];
```

Yellow replaced Green color.

<br>

## Interate array

To iterate an array we can use [repeat structure](https://github.com/Henryxavierb/starting-from-the-beginning/blob/learning/content/conditionals-and-repeat-structure.md#repeat-structure) or simply an [map function]().

```
  colors.map(color => {
    console.log(color);
  })

  --  -- -- -- -- -- -- -- -- -- -- -- -- -- --

  for(const name of names) {
    console.log(name);
  }
```

<br>

OBS: If you don't know the map format, learn before about [arrow function](https://github.com/Henryxavierb/starting-from-the-beginning/blob/learning/content/functions.md#curious-things-arrow-function)

<br>

## Remove array data

<br>

To finish, we'll remove the data of an array. For this, we'll use the pop method.
The pop method is used to remove the last data on the array. Last see it

```
  // colors: ["Red", "Yellow", "Blue"];

    colors.pop();

  // colors: ["Red", "Yellow"];
```
