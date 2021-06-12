## Functios
Functios in AbleScript can be defined using `functio` keyword, identifier, parentheses (that can optionally contain arguments) and functio body.
```ablescript
functio sayhello() {
    "hello!" print;
}
```

Functio calls are statements, so they do not return any value. Luckily, all arguments are passed by reference, so you save return value by mutating them.
```ablescript
functio sum(a, b, return) {
    return = a + b;
}

var return;
sum(3, 9, return);
```