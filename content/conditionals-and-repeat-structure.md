<h1 align="center">Conditionals and repeat structure</h1>

<br>

# Conditionals

Sometimes we need choose which event is dispatch, or check if form is avaliable to submit, and others cases. JavaScript has a some conditional cases, like:

- if - else if - else
- Switch

<br>

## If - else

The most conditionals are written with if / else. Has a simple structure and also can be written in an only line. Let's see it:

```

  const nome = "João"

  if (nome === "João") {
    console.log("Meu nome é João");
  } else {
    console.log("Meu nome é Maria");
  }

```

If the name is "João", the output from console.log will be "Meu nome é João". Another thing is "Meu nome é Maria".

<br>

## Switch

Switch either is a awesome. We can choose multiple choises, like if/else.

```

  const color = "red"

  switch(color) {
    case "blue":
      return console.log("A cor é azul!")
    case "grey":
      return console.log("A cor é cinza!")
    case "red":
      return console.log("A cor é vermelho!")
  }

  // output: "A cor é vermelha"

```

If you missing put "return" or "break" on the switch, they will iterator through the other options, running each code until they find return or break.

---

<br>

## Repeat structure

Is a simple way to, for example, iterator by list, or run some code block to render a data or layout. For example, you need print each name of the party list:

```
  const partyNames = ["João","Maria","Bentina","Victor","Mônica"]
```

We will see three types of repeat structure:

<br>

### For

```
  for (const index = 0; index < partyNames.length; index++) {
    console.log("Name: ", partyNames[index])
  }
```

For has a simple structure that need three components, like index;

- First, index reference a number, 0.
- Second, index reference also a number, but it has a value the number that is less than the list length, 4.
- Third, and to finish, index reference that your value is increment 1 by 1;

<br>

So... we get the index and we use to return a value on the index position.
