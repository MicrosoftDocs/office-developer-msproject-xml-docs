---
title: CurrencyDigits Element
TOCTitle: CurrencyDigits Element
ms:assetid: adb6f90f-bbe0-4843-994b-390255360400
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968638(v=office.12)
ms:contentKeyID: 13188329
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- CurrencyDigits element
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# CurrencyDigits Element




The number of digits that appear after the decimal when Microsoft Office Project shows currency values.

    <CurrencyDigits>
      IntegerValue
    </CurrencyDigits>

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
<td><p>No digits after the decimal, for example: $0</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>One digit after the decimal, for example: $0.0</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>Two digits after the decimal, for example: $0.00</p></td>
</tr>
</tbody>
</table>

## See Also

#### Concepts

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

[XML Schema for the Project Element](xml-schema-for-the-project-element.md)

