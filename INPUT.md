# Input

***

Generate variable input file from template.

## Command

```shell
flint input [<template-name>] [--template | -t <template-path>] [--output | -o <output-path>] [--yaml | -y] [--force | -f] [--verbose | -v]
```

or

```shell
flint i [<template-name>] [--template | -t <template-path>] [--output | -o <output-path>] [--yaml | -y] [--force | -f] [--verbose | -v]
```

## Argument

`[<template-name>]`

Template from template home to use.

## Option

`[--template | -t <template-path>]`

Path for template to use. If template name argument is presented, this value will be ignored.

`[--output | -o <output-path>]`

Path to write generated file. If not presented, current path for the process will be used.

`[--yaml | -y]`

Use YAML format. If not presented, JSON format will be used.

`[--force | -f]`

Override output path.

`[--verbose | -v]`

Output more information.
