<h1 align="center">Varaibles</h1>

# Var

<br>

## Scope

Are globally [scoped]() or function/locally scoped. The scope is global when a var variable is declared outside a function.

```
  var hello = "Hello";

  function sayWorld() {
    var world = "World";
  }

  console.log("World", world);
  // error: world is not defined

```

<br>

## Mutable

Also, var can be re-declared and updated.

```
  var word = "Hello";
  var word = "Word";

  word = "Hello word"

```

<br>

## Hoisted

Var are [hoisted]() to the top of their scope and initialized with a value of [undefined]().

```
  console.log("Say", say);

  var say = "Hello word";

```

it is interpreted as this:

```
  var say;
  console.log("Say", say);
  // say is undefined

  say = "Hello word";

```

<br>

## Problems with var

```
 var say = "hey hi";
 var times = 4;

 if (times > 3) {
  var say = "say Hello instead";
 }

 console.log(say)
 // "say Hello instead"
```

If you have used 'say' in other parts of your code, you might be surprised at the output you might get.

<br>

---

<br>

# Let

<br>

## Is a block scope

So a variable declared in a [block]() with let is only avaliable for use within that block.

```
  let greeting = "say Hi";
  let times = 4;

  if (times > 3) {
    let hello = "say Hello instead";

    console.log(hello);
    // "say Hello instead"
  }

  console.log(hello);
  // hello is not defined

```

<br>

## Mutable

A let variable can be updated but not re-declared.

```
 let greeting = "say Hi";
 greeting = "say Hello instead";

```

this will return an error:

```
  let greeting = "say Hi";

  let greeting = "say Hello instead";
  // error: Identifier 'greeting' has already been declared

```

However, if the same variable is defined in different scopes, there will be no error

```
   let greeting = "say Hi";

   if (true) {
        let greeting = "say Hello instead";

        console.log(greeting);
        // "say Hello instead"
   }

   console.log(greeting);
   // "say Hi"

```

<br>

## Hoisting of let

Just like var, let declaration are hoisted to the top. Unlike var which is initialized as undefined, the keyword is initialized. So, if you try to use a let variable declaration, you'll get a Reference Error.

<br>

---

<br>

# Const

<br>

## Const declarations are block scoped

Like let declaration, const declaration can only be accessed within the block they were declared.

<br>

## Immutable

Const cannot be updated or re-declared. So, every const declaration, therefore, must be initialized at the time of declaration.

<br>

While a const object cannot be updated, the properties of this objects can be updated. Therefore, if we declare a const object as this:

```
  const greeting = {
    message: "say Hi",
    times: 4
  }
```

while we cannot do this:

```
 const greeting = {
    words: "Hello",
    number: "five"
}

// error:  Assignment to constant variable.
```

we can do this:

```
  greeting.message = "Say hello instead"
```

<br>

## Hoisting of const

Just like let, const declarations are hoisted to the top but are not initialized.

---

<h1 align="center">Resume</h1>

- Var declarations are globally scoped of function scoped while let and const are block scoped.
- Var variables can be updated and re-declared within it's scope; Let variables can be updated but not re-declared; Const variable can neither be updated nor re-declared.
- They are all hoisted to the top of their scope. But while var variables are initialized with undefined, let and const variables are not initialized.
- While var and let can be declared without being initialized, const must be initialized during declaration.
