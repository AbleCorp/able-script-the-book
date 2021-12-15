# Carts
Carts are the only collections in AbleScript which stores key - value mappings. They are defined by typing comma-separated `value <= key` associations into square brackets.

```ablescript
var cart = [
    "Buy Able products" <= "What to do?",
    6 * 9 <= "answ" + "er",
    "able" <= true
];
```

To access or change values, put square square brackets behind the cart with the key.

```ablescript
cart[true] = "Able";
cart["What to do" + "?"] print;
```