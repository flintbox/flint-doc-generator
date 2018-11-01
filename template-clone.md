# Clone

***

Clone template repository to template home path.

## Command

```shell
flint template clone <repository-url> [<template-name>] [--branch | -b <branch>] [--force | -f] [--verbose | -v]
```

or

```shell
flint t c <repository-url> [<template-name>] [--branch | -b <branch>] [--force | -f] [--verbose | -v]
```

## Argument

`<repository-url>`

Repository URL to clone.

`[<template-name>]`

Template name. This is sub path relative to template home. If not present, the value will be the name from repository URL.

## Option

`[--branch | -b <branch>]`

Branch to clone.

`[--force | -f]`

Override existing template under template home.

`[--verbose | -v]`

Output more information.
