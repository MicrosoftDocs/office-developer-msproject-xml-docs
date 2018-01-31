---
title: MoveRemainingStartsBack Element
TOCTitle: MoveRemainingStartsBack Element
ms:assetid: b2fa4c92-1740-4532-bd40-03e32ed8a8c3
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968650(v=office.12)
ms:contentKeyID: 13188341
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- MoveRemainingStartsBack element
---

# MoveRemainingStartsBack Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

Indicates whether the beginning of remaining portions of tasks scheduled to begin after the status date, but begun early, should be moved back to the status date.

    <MoveRemainingStartsBack>
      BooleanValue
    </MoveRemainingStartsBack>

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
<td><p>Minimum: 0</p>
<p>Maximum: 1</p></td>
</tr>
</tbody>
</table>

## Text Value

A text value of type boolean is required.

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
<td><p>False</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>True</p></td>
</tr>
</tbody>
</table>

## Remarks

The MoveRemainingStartsBack element has a rounding error. The internal work value has eight digits; the work value loses 0.001 seconds for every minute, causing a rounding error.

## See Also

#### Concepts

[Project Elements and XML Structure](bb968439\(v=office.12\).md)

[XML Schema for the Project Element](bb968695\(v=office.12\).md)

