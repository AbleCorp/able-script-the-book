## Functios
Functios in AbleScript can be defined using `functio` keyword, identifier, parentheses (that can optionally contain arguments) and functio body.
```ablescript
functio sayhello ()
{
   /*hello!*/ print;
}
```

Functio calls are statements, so they do not return any value. Luckily, all arguments are passed by reference, so you save return value by mutating them.
```ablescript
functio sum (aa, bb, return)
{
   aa + bb =: return;
}

return dim;
sum (3, 9);
```

See, how you do not have to pass the variable as an argument if variable already exists in the scope.

### Eval
If you want to evaluate a value of code, simply call it:
```ablescript
num dim 4 + 2;
num + /*print*/ ();
```

### Functio chains
Using `+` and `*` operators, functions in AbleScript can be "chained"

#### Chain kinds
- `+`: Equal - all arguments for chain are equally devided between left and right hand-side functions
- `*`: By arity - all arguments are distributed for every functio in chain by its arity


```ablescript
functio PrintA (arg)
{ /*A: */ + arg print; }

functio PrintB (arg)
{ /*B: */ + arg print; }

PrintA * PrintB (4, 2);
```

Output:
```
A: 4
B: 2
```
