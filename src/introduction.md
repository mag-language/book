# Introduction

Mag is a dynamic, object-oriented language with patterns, classes and multiple dispatch.

This book aims to offer a comprehensive, detailed and complete documentation of the language and its implementation, from setting up the development environment to deploying an application, regardless if it's a microcontroller, a laptop or a cloud machine.

## Multiple Dispatch

Without further ado, let's explore some language features. Using multiple dispatch, a simple Fibonacci function could look like this:

```mag
def fib(0) 0
def fib(1) 1
def fib(n Int) fib(n - 1) + fib(n - 2)
```

## Pattern Matching

Alternatively, this can also be implemented with pattern matching like this:

```mag
def fib(n Int)
  match fib
    0 => 0,
    1 => 1,
    n => fib(n - 1) + fib(n - 2),
  end
end
```