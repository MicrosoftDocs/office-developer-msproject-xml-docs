---
title: MoveRemainingStartsForward Element
TOCTitle: MoveRemainingStartsForward Element
ms:assetid: 11e4beca-84b4-4594-83f0-99be5dc7a60a
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968418(v=office.12)
ms:contentKeyID: 13188111
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- MoveRemainingStartsForward element
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# MoveRemainingStartsForward Element




Indicates whether the beginning of remaining portions of tasks scheduled to have begun late should be moved up to the status date.

    <MoveRemainingStartsForward>
      BooleanValue
    </MoveRemainingStartsForward>

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

The MoveRemainingStartsForward element has a rounding error. The internal work value has eight digits; the work value loses 0.001 seconds for every minute, causing a rounding error.

## See Also

#### Concepts

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

[XML Schema for the Project Element](xml-schema-for-the-project-element.md)

