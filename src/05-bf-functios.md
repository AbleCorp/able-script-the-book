# BF functios
One of AbleScript's core functions is running BF code. Simple BF functio can be declarated using `bff` keyword:
```ablescript
bff helloworld
{
   ++++++++++[>+++++++>++++++++++>+++>+<<<<
   -]>++.>+.+++++++..+++.>++.<<++++++++++++
   +++.>.+++.------.--------.>+.>.
}
```

Default tape size limit is 30 000 bytes, but that can be overriden using tape size parameter on declaration
```ablescript
bff helloworld (1200) { ... }
```

BF functios are called in same way as Able functios:
```ablescript
helloworld();
```
You can specify input data as parametre.
