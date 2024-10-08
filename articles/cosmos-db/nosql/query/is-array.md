---
title: IS_ARRAY
titleSuffix: Azure Cosmos DB for NoSQL
description: An Azure Cosmos DB for NoSQL system function that returns a boolean indicating whether an expression is an array.
author: seesharprun
ms.author: sidandrews
ms.service: azure-cosmos-db
ms.subservice: nosql
ms.topic: reference
ms.devlang: nosql
ms.date: 08/22/2024
ms.custom: query-reference
---

# IS_ARRAY (NoSQL query)

[!INCLUDE[NoSQL](../../includes/appliesto-nosql.md)]

Returns a boolean value indicating if the type of the specified expression is an array.  
  
## Syntax
  
```nosql
IS_ARRAY(<expr>)  
```  
  
## Arguments

| | Description |
| --- | --- |
| **`expr`** | Any expression. |
  
## Return types
  
Returns a boolean expression.  
  
## Examples
  
The following example checks objects of various types using the function.  
  
:::code language="nosql" source="~/cosmos-db-nosql-query-samples/scripts/is-array/query.sql" highlight="2-10":::

:::code language="json" source="~/cosmos-db-nosql-query-samples/scripts/is-array/result.json":::

## Remarks

- This function benefits from a [range index](../../index-policy.md#includeexclude-strategy).

## Related content

- [System functions](system-functions.yml)
- [`IS_OBJECT`](is-object.md)
