# Advanced JavaScript

- [Roadmap](https://coggle.it/diagram/XE3ZoVj-rtA5hcxj/t/advanced-javascript)

## The V8 Engine

- JavaScript Code runs in the browser with the help of an engine.
- Brendan Eich created the first JS engine (SpiderMonkey) while working at NetScape (Marc Andressen's Company). Previously browsers could only read HTML and CSS.
- There are many such engines like V8 and SpiderMonkey, the most famous of them being the V8 engine by Google.
- In 2008, Google was working on Google Maps. They wanted the browser to be faster, before 2008 JS used be slow, Google devs changed the entire scenario by building V8 which gave immense capabilities to the web which you see these days.
- V8 is written in C++

### How does the JS Engine work?

- Lexical Analysis / Tokenisation
- AST (Abstract Syntax Trees) (astexplorer.net)
- Interpreter
- Optimised Code

### But what is ECMASCRIPT?

- ECMASCRIPT is the standard version of JS that engines must adhere to for interoperability of web pages across different browsers.

### Interpreter vs Compiler

A compiler will compile down the source code to Machine Code and use that piece of binary whenever the code needs to run. A compiler is essentially a piece of code which takes one language and converts it into another.

An interpreter on the other hand will take every line one by one and convert it into machine code.

Compilation is generally faster because repeated portions of code can be directly run from the machine code, where in an interpreted language the code within the loop will have to be converted each time to machine code.

A compiler can also be slower as it has to compile down to machine code first.

Using the best of both worlds, an interpreter's ability to run code line by line and compiler's ability to optimise, we built the JIT (Just In Time Compiler)

- V8 takes in source code and spits out BYTECODE, this is known as ignition.
- A profiler looks out for optimisations and iterations.
- If the profiler finds some pieces of code which are repeated, they are passed down to the compiler. They constantly make updates to optimise the code.
- The compiler for V8 is called TurboFan

### Call Stack and Memory Heap

#### Memory Heap

- Memory heap stores the data of our app. The variables, objects all these are stored in the Memory Heap. This is where the memory allocation happens.

#### Call Stack

- Call stack actually keeps a track of what is happening line by line in a program. This is where the engine keeps track of where the code is in it's execution.

- The main function of our file is called the Global Execution Context.
