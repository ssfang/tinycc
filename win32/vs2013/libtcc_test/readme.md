
## use tcc as a "backend" for a code generator .

The libtcc library enables you to use TCC as a backend for dynamic code generation.

Read the `libtcc.h' to have an overview of the API. Read `libtcc_test.c' to have a very simple example.

The idea consists in giving a C string containing the program you want to compile directly to libtcc. Then you can access to any global symbol (function or variable) defined.

In the example, it includes a "Simple libc header" `tcclib.h` and links `libtcc1.a` for TCC.


If no envirenment set, you would need to do the following.
```
D:\ProgramFiles\Microsoft Visual Studio 12.0>F:\repo\tcc\tinycc\win32\vs2013\Debug\libtcc_test.exe -
IF:\repo\tcc\tinycc;F:\repo\tcc\tinycc\include -LF:\repo\tcc\tinycc\win32
Hello World!
fib(32) = 2178309
add(32, 64) = 96
```