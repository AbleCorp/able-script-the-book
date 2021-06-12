# Expressions vs Statements
AbleScript strictly differentiates expressions and statements. Expressions cannot cause any side effects, they have value (can be used as part of expression) and they are only mathematical and logical operations or values. 

On the other hand, statements cause side effects and they do not have any value. AbleScript's AST[^1] consists only from statements and expressions are used only as parts of statements. For example control structures, definitions and function calls are statements.

[^1]: Abstract Syntax Tree