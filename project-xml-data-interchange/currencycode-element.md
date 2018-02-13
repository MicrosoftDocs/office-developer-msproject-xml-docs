---
title: CurrencyCode Element
TOCTitle: CurrencyCode Element
ms:assetid: 8535d7d5-1414-4222-baaf-f16f8bc8131c
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968575(v=office.12)
ms:contentKeyID: 13188266
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- CurrencyCode element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# CurrencyCode Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

A three letter currency character code.

    <CurrencyCode>
        StringValue
    </CurrencyCode>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968701(v=office.12).md">Project</a></p></td>
</tr>
</tbody>
</table>

## Occurrences

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Minimum: 1</p>
<p>Maximum: 1</p></td>
</tr>
</tbody>
</table>

## Text Value

A text value of type string is required. The string can have no more than three characters.

## Remarks

The currency character codes are defined in ISO 4217; for example, the United States Dollar is USD, the Japanese Yen is JPY, and the European Euro is EUR.

The default value for new projects is determined by the enterprise global template. If there is no enterprise global template value, the default value is taken from the Windows operating system where Project Server is running.

## Example

The following example uses the CurrencyCode element to specify that the currency for the project is United States dollars.

``` xml
<Project xmlns="http://schemas.microsoft.com/project">
  …
  <CurrencyCode>USD</CurrencyCode>
  …
</Project>
```

## See Also

#### Concepts

[Project Elements and XML Structure](bb968439\(v=office.12\).md)

[XML Schema for the Project Element](bb968695\(v=office.12\).md)

