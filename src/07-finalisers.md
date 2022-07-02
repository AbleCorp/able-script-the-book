# Finalisers
If you need to run some code at the end of the program, you can use the `finally` block:
```ablescript
finally {
    /*Goodbye!*/ print;
}

/*Hello!*/ print;
```

Output:
```
Hello!
Goodbye!
```

This is similar to `defer` from other languages, but rather than executing at the end of the function, it executes at the end of the whole program.

Finally blocks are executed in the order they were defined.