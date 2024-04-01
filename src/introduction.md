# Introduction

Mag is a dynamic, object-oriented language with patterns, classes and multiple dispatch.

Here is a simple example of a Fibonacci function implemented using multiple dispatch in Mag:

```mag
def fib(0) 0
def fib(1) 1
def fib(n Int) fib(n - 1) + fib(n - 2)
```