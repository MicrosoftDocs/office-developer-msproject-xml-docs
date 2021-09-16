---
title: UpdateNeeded Element
TOCTitle: UpdateNeeded Element
ms:assetid: f5141b03-2ef5-48fe-82ce-d1369021cbab
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968735(v=office.12)
ms:contentKeyID: 13188425
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- UpdateNeeded element
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# UpdateNeeded Element




Indicates whether a TeamUpdate message should be sent to the resource assigned to a task because of changes to the start date, finish date, or resource assignments.

    <UpdateNeeded>
      BooleanValue
    </UpdateNeeded>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="assignment-element.md">Assignment</a></p></td>
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

## See Also

#### Concepts

[Assignment Elements and XML Structure](assignment-elements-and-xml-structure.md)

[XML Schema for the Assignments Element](xml-schema-for-the-assignments-element.md)

