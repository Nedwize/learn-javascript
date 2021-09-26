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
