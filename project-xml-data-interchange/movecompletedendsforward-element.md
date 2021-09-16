---
title: MoveCompletedEndsForward Element
TOCTitle: MoveCompletedEndsForward Element
ms:assetid: 370fee53-9488-4907-8d5c-d355fd85b8d3
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968463(v=office.12)
ms:contentKeyID: 13188155
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- MoveCompletedEndsForward element
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# MoveCompletedEndsForward Element




Indicates whether the end of completed portions of tasks scheduled to have been completed before the status date, but begun late, should be moved up to the status date.

    <MoveCompletedEndsForward>
      BooleanValue
    </MoveCompletedEndsForward>

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

The MoveCompletedEndsForward element has a rounding error. The internal work value has eight digits; the work value loses 0.001 seconds for every minute, causing a rounding error.

## See Also

#### Concepts

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

[XML Schema for the Project Element](xml-schema-for-the-project-element.md)

