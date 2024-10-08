---
title: StringToNull
titleSuffix: Azure Cosmos DB for NoSQL
description: An Azure Cosmos DB for NoSQL system function that returns a string expression converted to null.
author: seesharprun
ms.author: sidandrews
ms.service: azure-cosmos-db
ms.subservice: nosql
ms.topic: reference
ms.devlang: nosql
ms.date: 08/22/2024
ms.custom: query-reference
---

# StringToNull (NoSQL query)

[!INCLUDE[NoSQL](../../includes/appliesto-nosql.md)]

Converts a string expression to `null`.
  
## Syntax

```nosql
StringToNull(<string_expr>)  
```

## Arguments

| | Description |
| --- | --- |
| **`string_expr`** | A string expression. |

## Return types

Returns a `null`.

## Examples
  
The following example illustrates how this function works with various data types.

:::code language="nosql" source="~/cosmos-db-nosql-query-samples/scripts/stringtonull/query.sql" highlight="2-9":::

:::code language="json" source="~/cosmos-db-nosql-query-samples/scripts/stringtonull/result.json":::

## Remarks

- This function doesn't use the index.
- If the expression can't be converted, the function returns `undefined`.

> [!NOTE]
> For more information on the JSON format, see [https://json.org](https://json.org/).

## Related content

- [System functions](system-functions.yml)
- [`StringToBoolean`](stringtoboolean.md)
