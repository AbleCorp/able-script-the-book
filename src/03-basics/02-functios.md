## Functios
Functios in AbleScript can be defined using `functio` keyword, identifier, parentheses (that can optionally contain arguments) and functio body.
```ablescript
functio sayhello() {
    "hello!" print;
}
```

Functio calls are statements, so they do not return any value. Luckily, all arguments are passed by reference, so you save return value by mutating them.
```ablescript
functio sum(aa, bb, return) {
    return = aa + bb;
}

var return;
sum(3, 9, return);
```

### Eval
If you want to evaluate a value of code, simply call it:
```ablescript
var num = 4 + 2;
num + "print"();
```

### Functio chains
Using `+` and `*` operators, functions in AbleScript can be "chained"

#### Chain kinds
- `+`: Equal - all arguments for chain are equally devided between left and right hand-side functions
- `*`: By arity - all arguments are distributed for every functio in chain by its arity


```ablescript
functio printsum(num1, num2) {
    num1 + num2 print;
}

functio hello(name) {
    "Hello, " + name + "!"print;
}

var sumhello = printsum * hello;
sumhello(3, 4, "Able");
```

Output:
```
7
Hello, Able!
```
