---
title: "Guid.From | Microsoft Docs"
ms.date: 4/16/2018
ms.service: powerquery

ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# Guid.From
## Syntax

<pre>
Guid.From(<b>value</b> as nullable text) as nullable text
</pre>

## About
Returns a `Guid.Type` value from the given `value`. If the given `value` is `null`, `Guid.From` returns `null`. A check will be performed to see if the given `value` is in an acceptable format. Acceptable formats provided in the examples.

## Example 1
The Guid can be provided as 32 contiguous hexadecimal digits.

```powerquery-m
Guid.From("05FE1DADC8C24F3BA4C2D194116B4967")
```

`"05fe1dad-c8c2-4f3b-a4c2-d194116b4967"`

## Example 2
The Guid can be provided as 32 hexadecimal digits separated by hyphens into blocks of 8-4-4-4-12.

```powerquery-m
Guid.From("05FE1DAD-C8C2-4F3B-A4C2-D194116B4967")
```

`"05fe1dad-c8c2-4f3b-a4c2-d194116b4967"`

## Example 3
The Guid can be provided as 32 hexadecimal digits separated by hyphens and enclosed in braces.

```powerquery-m
Guid.From("{05FE1DAD-C8C2-4F3B-A4C2-D194116B4967}")
```

`"05fe1dad-c8c2-4f3b-a4c2-d194116b4967"`

## Example 4
The Guid can be provided as 32 hexadecimal digits separated by hyphens and enclosed by parentheses.

```powerquery-m
Guid.From("(05FE1DAD-C8C2-4F3B-A4C2-D194116B4967)")
```

`"05fe1dad-c8c2-4f3b-a4c2-d194116b4967"`
