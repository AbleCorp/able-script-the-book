## Control flow
To decide whatever code should be runned and run code repeatedly is basic block of most programming languages. AbleScript contains `if` conditions and loop.

### Unless statements
Unless statement decide if code should be runned or not by a condition.
```ablescript
dim num 7;

unless (num ain't 7)
{ /*Condition was not met*/ print; }
```
Unless statements starts with keyword `unless` followed by expression inside parantheses. If result of evaluated expression is `never`, following block of code will be run, else, it will be skipped and program execution will continue.

In AbleScript, there is no else branch, so to execute code if condition is met, you have to negate it.
```ablescript
dim num 7;

unless (num = 7)
{ /*Condition wasn't met*/ print; }

unless (num ain't 7)
{ /*Condition was met*/ print; }
```

### Loop
Loops repeates block of code over and over again forewer until it isn't explicitly told to stop.
For example,
```ablescript
loop {
   /*Buy Able products!*/ print;
}
```
will infinitely repeat this piece of code.

So, for stopping the loop, there exist `break` keyword.
```ablescript
var counter = 0;
loop {
   unless (counter ain't 10) { break; }
   /*Buy Able products!*/ print;
   counter + 1 =: counter;
}
```
This example will stop executing the loop after 10 times writing "Buy Able products!" on screen.

For jumping back to start of the block in the loop, there is keyword `hopback` (equivalent to `continue` in other languages.)
```ablescript
dim counter -1;
loop {
   counter + 1 =: counter;
   unless (counter ain't 3) { hopback; }
   unless (counter ain't 5) { break; }
   counter print;
}
```
Output:
```console
0
1
2
4
```

### Rlyeh
`rlyeh` keyword crashes program with some random exit code.
```ablescript
/*hello*/ print;
rlyeh;
/*bye*/ print;
```
```console
$ ablescript --file main.able
hello
$ echo $?
31
```
