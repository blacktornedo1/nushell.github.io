---
title: date now
categories: |
  date
version: 0.90.0
date: |
  Get the current date.
usage: |
  Get the current date.
feature: default
---
<!-- This file is automatically generated. Please edit the command in https://github.com/nushell/nushell instead. -->

# <code>{{ $frontmatter.title }}</code> for date

<div class='command-title'>{{ $frontmatter.date }}</div>

## Signature

```> date now {flags} ```


## Input/output types:

| input   | output   |
| ------- | -------- |
| nothing | datetime |

## Examples

Get the current date and display it in a given format string.
```nu
> date now | format date "%Y-%m-%d %H:%M:%S"

```

Get the time duration from 2019-04-30 to now
```nu
> (date now) - 2019-05-01

```

Get the time duration since a more accurate time
```nu
> (date now) - 2019-05-01T04:12:05.20+08:00

```

Get current time in full RFC3339 format with timezone
```nu
> date now | debug

```
