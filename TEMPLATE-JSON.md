# template.json

***

Template manifest file. YAML is also supported.

```json
{
  "description": "Template description",
  "variables": [
    {
      "name": "Author"
    },
    {
      "name": "Module Name",
      "defaultValue": "CLI"
    }
  ],
  "prehooks": [
    "script1.sh",
    "script2.sh",
    "script3.sh"
  ],
  "posthooks": [
    "script4.sh",
    "script5.sh"
  ]
}
```

`description`

Template description. This field is optional.

`variables`

Variable used in template. Each item has `name` and optional `defaultValue`. This field is optional.

`prehooks`

Prehook scripts. These scripts will be executed in sequence before the variables are processed. Scripts can use `FLINT_OUTPUT_PATH` and `FLINT_+EACH_VARIABLE_NAME (Whitespaces replaced with underscores.)` environment variable. This field is optional.

`posthooks`

Posthook scripts. These scripts will be executed in sequence after the variables are processed. Scripts can use `FLINT_OUTPUT_PATH` and `FLINT_+EACH_VARIABLE_NAME (Whitespaces replaced with underscores.)` environment variable. This field is optional.
