## Hello world

First of all, you need to create a new AbleScript project.

On Unix systems, you have to do:
```console
$ mkdir hello_world
$ cd hello_world
$ touch main.able
```
and then open `main.able` with your editor of choice.

Hello World program in AbleScript looks like this:
```ablescript
"Hello, world!" print;
```

Then, execute your program with AbleScript
```console
$ able-script --file main.able
```