## Variables
AbleScript variables can be defined using `var` keyword:
```ablescript
var variable;
```
This will create an uninitialised variable, so it's value will be `nul`.

For assigning value to variable, you can use:
```ablescript
variable = 42;
```

Initial value of variable can be defined on declaration:
```ablescript
var variable = 42;
```

### Constants
Constants cannot be user defined, they are internally defined inside AbleScript interpreter (see `src/consts.rs`)

### Banning
AbleScript has bannable variables, what means when variable is banned, it cannot be used and it's usage resolves into runtime error.

Ban keyword was named after Rust Language Community Discord Server's owner `MelodicStream#1336` nicknamed Melo:
```ablescript
var variable = "Hello, world!";
melo variable;
variable print; owo Runtime Error
```