# Spark

***

Generate project from template.

## Command

```shell
flint spark [<template-name>] [--template | -t <template-path>] [--output | -o <output-path>] [--input | -i <input-file-path>] [--force | -f] [--verbose | -v]
```

or

```shell
flint s [<template-name>] [--template | -t <template-path>] [--output | -o <output-path>] [--input | -i <input-file-path>] [--force | -f] [--verbose | -v]
```

## Argument

`[<template-name>]`

Template from template home to use.

## Option

`[--template | -t <template-path>]`

Path for template to use. If template name argument is presented, this value will be ignored.

`[--output | -o <output-path>]`

Path to write generated project. If not presented, current path for the process will be used.

`[--input | -i <input-file-path>]`

Variable input file path.

`[--force | -f]`

Override output path.

`[--verbose | -v]`

Output more information.
