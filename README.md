## Haha Language
This is my take on making my own basic esoteric interpreted shell programming language, named `Haha` for fun. This is just a very basic interpreter, coded only in a few days (with a lot of other days looking at tutorials and designing prototypes) as a beginner in C++, so it goes without saying: use it on your own risk. <sub>It might even explode.</sub>




---

### Running
The dependencies that the interpreter use are all present in the modern C++ standard library: `regex`, `vector`, `fstream`, etc. So it shouldn't be too hard to compile it with MinGW if you're on Windows. There's a statically-linked build in the release tab if you want.

After you opened the program, it will then ask you to input the name of your `.haha` file. Simply write the full name of it there and press enter.




---


### Contents
- [Printing "Hello World!"](#pri)
- [Variables](#var)
- [Arithmetic](#art)
- [Increment and Decrement](#inc)
- [Newlines](#new)
- [System Commands](#sys)
- [Conditions](#con)
- [Control Flow](#cont)
- [Warning](#war)



---

### <a id="pri">Printing "Hello World!"</a>
What's an introduction to a programming language without starting at the famous `Hello World!`? To print a `Hello World!` program, make a new file named `helloworld.haha`, and use the `haha` keyword to print text to the console:

```
haha Hello World!
```
Output: `Hello World!`

We don't use double quotes because `haha` always expect string literals as its subsequent argument. In order to print variables, we use `hahaha`.

```
hahaha x
```
This prints a variable named `x`.

`Note: Keywords MUST always be placed at the start of a line. Otherwise, it will be considered a comment.`

```
This is a comment!
  haha This also now a comment!
```

---

### <a id="var">Variables</a>
`Haha` has only two data types: a signed integer (`ha`) and a string (`ah`).

Here's an example of a variable declaration:
```
ha x 10
ah text What da dog doin
```

To take an input and store it to a variable, you can use `hhaa`.

```
ha x 0
hhaa x
hahaha x
```

This declares a signed integer variable `x` initialized as 0 at its definition. It then proceeds to request an input from the user to store in the `x` variable— then prints it out to the console.

---


### <a id="art">Arithmetic</a>
`Haha` only supports the four basic math operations `+`,`-`,`*`,`/`.

To calculate, you can use the `aha` keyword. 
```
ha x 3
ha y 2
ha z 0
aha x + y z
hahaha z
```
Output: `5`


It takes four arguments: `variable`, `operator`,`variable`,`variable`. Where the first two variables are used to get the numbers to calculate and the third one to store it (which in this case is variable `z`).


---

### <a id="inc">Increment and Decrement</a>
To increment/decrement an `ha` variable, you can use `a`.

```
a ++ x
a -- x
```

---

### <a id="new">Newlines</new>

`Haha` doesn't read a newline symbol (`\n`). So in order to create one, you use `h`. It takes an integer as its subsequent argument to print how many newlines you want.

This prints out 1 newline:
```
h 1
```

This prints out 1000 newline (yeh):
```
h 1000
```
---

### <a id="sys">System commands</sys>
To execute commands on the system console, you can use `aah`.


For clearing the screen.
```
aah clear
```

For viewing the current date.
```
aah date
aah time
```

---

### <a id="con">Conditions</a>
To start a condition, you can use the `haa` keyword, ending with `he` to break the condition.

```
ha x 10
ha y 5
haa x < y
haha x
he
```
Nothing will be printed to the console with this program (because 10 isn't greater than 5).

`haa` only takes an integer variable as its argument.

`Note: Nested haa is not supported. Trying to nest haa statements will result in unexpected things occurring. I warned you.`

---

### <a id="cont">Control Flow</a>
In order to iterate through a series of keywords, you can use `haahaa`, followed by an `ah` variable argument, and ending with `hehe` to break the iteration.

```
ha x 5
haahaa x
hahaha x
a ++ x
hehe
```
Output: `56789`

`Note: If you didn't add an argument to haahaa, it will automatically evaluate to 1. Nested iterations here are also a no-no.`



---

### <a id="war">Warning</a>
This is my very first time creating my own programming language, so expect that there would be a LOT of edge cases (also zero error handling).  I'm simply relatively inexperienced in the end, so constructive criticisms are always welcomed!

#### License
[MIT](https://github.com/vonnogadas/haha-language/blob/main/LICENSE)
