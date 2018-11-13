---
title: "Sybase.Database | Microsoft Docs"
ms.date: 4/16/2018
ms.service: powerquery

ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend
manager: kfile
---
# Sybase.Database

## Syntax

<pre>
Sybase.Database(**server** as text, **database** as text, optional **options** as nullable record) as table
</pre>

## About

Returns a table of SQL tables and views available in a Sybase database on server `server` in the database instance named `database`. The port may be optionally specified with the server, separated by a colon. An optional record parameter, `options`, may be specified to control the following options: 

* `CreateNavigationProperties` : A logical (true/false) that sets whether to generate navigation properties on the returned values (default is true).
* `NavigationPropertyNameGenerator` : A function that is used for the creation of names for navigation properties.
* `Query` : A native SQL query used to retrieve data. If the query produces multiple result sets, only the first will be returned.
* `CommandTimeout` : A duration which controls how long the server-side query is allowed to run before it is canceled. The default value is ten minutes.
* `ConnectionTimeout` : A duration which controls how long to wait before abandoning an attempt to make a connection to the server. The default value is driver-dependent.
* `HierarchicalNavigation` : A logical (true/false) that sets whether to view the tables grouped by their schema names (default is false).

 The record parameter is specified as [option1 = value1, option2 = value2...] or [Query = "select ..."] for example.
  