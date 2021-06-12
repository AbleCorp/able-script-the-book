## Data types
AbleScript's typesystem is weak and dynamic. Variables do not have explicit types and values are implicitly converted between each other.

There is implicit conversion between every value type, so you can pass everything everywhere.

| Data Type |   Example   |
|:---------:|:-----------:|
|  String   |  `"Hello"`  |
|    Int    |    `42`     |
|   Bool    |   `true`    |
|   Abool   | `sometimes` |
|    Nul    |    `nul`    |

### Abool
Aboolean is unlike boolean which is binary (true and false) ternary. It can have values `always`, `sometimes` and `never`.

Implicit conversion table:

|    Abool    |   Bool   |
|:-----------:|:--------:|
|  `always`   |  `true`  |
|   `never`   | `false`  |
| `sometimes` | randomly |