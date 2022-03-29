---
title: printf
linktitle: printf
description: Formats a string using the standard `fmt.Sprintf` function.
date: 2017-02-01
publishdate: 2017-02-01
lastmod: 2017-02-01
categories: [functions]
menu:
  docs:
    parent: "functions"
keywords: [strings]
signature: ["printf FORMAT INPUT"]
workson: []
hugoversion:
relatedfuncs: []
deprecated: false
---

printf performs a Concatenation function.
Comparing concatenation in PHP to concatenation in Go (Hugo):

PHP:
```
$fullname = $firstname . ' ' . $lastname
```
Go:
```
{{ $fullname := printf "%s %s" $firstname $lastname }}
```
The PHP/Go comparison, above, is taken from Regis Philbert's excellent [Hugo Translator, a cheatsheet](https://www.regisphilibert.com/blog/2017/04/hugo-cheat-sheet-go-template-translator/) .
```
{{ i18n ( printf "combined_%s" $var ) }}
```

```
{{ printf "formatted %.2f" 3.1416 }}
```

See [the go doc](https://golang.org/pkg/fmt/) for additional information.
