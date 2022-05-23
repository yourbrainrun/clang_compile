# clang_compile
```
clang -g -c testlib.c
libtool -static -o libmylib.a testlib.o
clang -c uselib.c
clang -o main uselib.o -L. -I. -lmylib
./main
```
