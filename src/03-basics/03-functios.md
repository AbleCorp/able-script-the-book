## Functios
Functios in AbleScript are parts of program which can be called and given parameters. Unlike regular functions, they do not have a return value and their
calls are statements.

Functios are declared by keyword `functio` followed by identifier, parentheses and block.
```ablescript
functio fun() {
    "Hello, world!" print;
}

fun();
```

You can also specify parameters for functio by entering their names into parentheses. Multiple ones are spearated by commas.
```ablescript
functio greet(name1, name2) {
    "Hello, " + name1 + " and " + name2 + "!" print;
}

greet("Able", "Able")
```

```console
$ able-script --file main.able
Hello, Able and Able
```

All arguments are passed by reference, so you can manipulate with contents of the variable passed into functio.
```ablescript
functio sum(a, b, result) {
    result = a + b;
}

var x = 13;
var y = 42;
var z;
sum(x, y, z);

z == 55 print;
```
Output: `true`