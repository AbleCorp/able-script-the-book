## Variables
AbleScript has only mutable variables, that can be defined using `var` keyword:
```ablescript
var variable;
```
This will create an uninitialised variable = `Nul`.

For assigning value to variable, you can use:
```ablescript
variable = 42;
```

You can also specify an initial value when creating a variable:
```ablescript
var variable = 42;
```

### Constants
Constants cannot be user defined, they are internally defined inside AbleScript interpreter (see `src/consts.rs`).

### Banning
AbleScript has bannable variables. That means when variable is banned, it cannot be used and it's usage resolves into runtime error.

Ban keyword was named after Rust Language Community Discord Server's owner `MelodicStream#1336` nicknamed Melo:
```ablescript
var variable = "Hello, world!";
melo variable;
variable print; owo Runtime Error
```