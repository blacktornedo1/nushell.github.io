---
title: from url
categories: |
  formats
version: 0.90.0
formats: |
  Parse url-encoded string as a record.
usage: |
  Parse url-encoded string as a record.
feature: extra
---
<!-- This file is automatically generated. Please edit the command in https://github.com/nushell/nushell instead. -->

# <code>{{ $frontmatter.title }}</code> for formats

<div class='command-title'>{{ $frontmatter.formats }}</div>


::: warning
 Command `from url` was not included in the official binaries by default, you have to build it with `--features=extra` flag
:::
## Signature

```> from url {flags} ```


## Input/output types:

| input  | output |
| ------ | ------ |
| string | record |

## Examples

Convert url encoded string into a record
```nu
> 'bread=baguette&cheese=comt%C3%A9&meat=ham&fat=butter' | from url
╭────────┬──────────╮
│ bread  │ baguette │
│ cheese │ comté    │
│ meat   │ ham      │
│ fat    │ butter   │
╰────────┴──────────╯
```
