# Environment variable

***

## Template home

```shell
FLINT_TEMPLATE_HOME
```

Set path for template home.

## Preset value

```
FLINT_+VARIABLE_NAME (Whitespaces replaced with underscores.)
```

You can preset value for template variable on environment variables. For example, if there is a variable named `Owner Name` and you set environment variables as following

```shell
FLINT_Owner_Name=Jason Nam
```

Now, value for `Owner Name` will be automatically collected and skipped on interactive `spark` command. If the same value presented on input file, value on file will override environment variable.
