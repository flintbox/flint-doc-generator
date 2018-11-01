# Add

***

Copy template to template home path.

## Command

```shell
flint template add <path-to-template> [<template-name>] [--force | -f] [--verbose | -v]
```

or

```shell
flint t a <path-to-template> [<template-name>] [--force | -f] [--verbose | -v]
```

## Argument

`<path-to-template>`

Path to template.

`[<template-name>]`

Template name. This is sub path relative to template home. If not present, the value will be the last path component of path to template.

## Option

`[--force | -f]`

Override existing template under template home.

`[--verbose | -v]`

Output more information.
