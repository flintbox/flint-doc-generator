{% raw %}
# Predefined variable

***

Beside custom variables, several predefined variables are also available.

## File attribute

### File name

Following variables are processed into final output file name.

```
__FILE:NAME__
___FILE:NAME___
--FILE:NAME--
{{FILE:NAME}}
```

## Include file variable

You can include other files under `include/` on template files or directory names with following variables.

```
__INCLUDE:PATH TO FILE__
___INCLUDE:PATH TO FILE___
--INCLUDE:PATH TO FILE--
{{INCLUDE:PATH TO FILE}}
```

For example, read file `include/license/MIT` and replace variable with the content.

```
{{INCLUDE:license/MIT}}
```

## Date variable

Date variable has following form and processed with Swift [`DateFormatter`](https://developer.apple.com/documentation/foundation/dateformatter).

```
__DATE:LOCALE|DATE FORMAT__
___DATE:LOCALE|DATE FORMAT___
--DATE:LOCALE|DATE FORMAT--
{{DATE:LOCALE|DATE FORMAT}}
```

`LOCALE` is optional locale identifier.

`DATE FORMAT` can be one of the following values.

Type | Description
---- | -----------
`YEAR` | Date format `yyyy`
`YEAR-SHORT` | Date format `yy`
`MONTH` | Date format `MM`
`MONTH-SHORT` | Date format `M`
`DAY` | Date format `dd`
`DAY-SHORT` | Date format `d`
`SHORT` | System short date style
`MEDIUM` | System medium date style
`LONG` | System long date style
`FULL` | System full date style
Any String Value | Any date format needed

Examples,

```swift
{{DATE:YEAR}} // 2018
{{DATE:ko_KR|FULL}} // 2018년 6월 20일 수요일
--DATE:yyyy M dd-- // 2018 6 20
```
{% endraw %}
