---
title: "Lines.FromBinary | Microsoft Docs"
ms.date: 4/16/2018
ms.service: powerquery

ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# Lines.FromBinary

## Syntax

<pre>
Lines.FromBinary(**binary** as binary, optional **quoteStyle** as nullable number, optional **includeLineSeparators** as nullable logical, optional **encoding** as nullable number) as list
</pre>

## About
Converts a binary value to a list of text values split at lines breaks. If a quote style is specified, then line breaks may appear within quotes. If includeLineSeparators is true, then the line break characters are included in the text.