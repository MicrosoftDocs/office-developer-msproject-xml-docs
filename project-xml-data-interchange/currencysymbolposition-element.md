---
title: CurrencySymbolPosition Element
TOCTitle: CurrencySymbolPosition Element
ms:assetid: a800ac60-fceb-4aec-9d82-05c683b2e424
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968631(v=office.12)
ms:contentKeyID: 13188322
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- CurrencySymbolPosition element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# CurrencySymbolPosition Element




The position of the currency symbol.

    <CurrencySymbolPosition>
      IntegerValue
    </CurrencySymbolPosition>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="project-element.md">Project</a></p></td>
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
<td><p>Minimum: 0</p>
<p>Maximum: 1</p></td>
</tr>
</tbody>
</table>

## Text Value

A text value of type Integer is required.

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Value</p></th>
<th><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>0</p></td>
<td><p>Before, no space (default), for example: $0</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>After, no space, for example: 0$</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>Before, with space, for example: $ 0</p></td>
</tr>
<tr class="even">
<td><p>3</p></td>
<td><p>After, with space, for example: 0 $</p></td>
</tr>
</tbody>
</table>

## See Also

#### Concepts

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

[XML Schema for the Project Element](xml-schema-for-the-project-element.md)

