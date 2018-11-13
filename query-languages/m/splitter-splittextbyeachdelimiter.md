---
title: "Splitter.SplitTextByEachDelimiter | Microsoft Docs"
ms.date: 4/16/2018
ms.service: powerquery

ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# Splitter.SplitTextByEachDelimiter

  
## About  
Returns a function that splits text by each delimiter in turn.  
  
## Syntax

<pre>
Splitter.SplitTextByEachDelimiter(delimiters as list, optional quoteStyle as nullable number) as function  
</pre>
  
## Arguments  
  
|Argument|Description|  
|------------|---------------|  
|Delimiters|The delimiter characters are used to identify at what points to split the string.  The delimiter character is not included in the split values.  A trailing delimiter character will yield an additional empty text value.  The split values contain all characters between the delimiters.  This function will always produce at least one value.|  
|optional quoteStyle|The quoteStyle acts as described in Lines.FromText.  By default, it is QuoteStyle.Csv.|  
  
## <a name="__toc360789916"></a>Remarks  
  
-   Splitter.SplitTextByEachDelimiter is similar to Splitter.SplitTextByDelimiter except that each delimiter is used once in order to determine the points at which to break the text.  
  