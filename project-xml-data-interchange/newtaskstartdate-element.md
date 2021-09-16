---
title: NewTaskStartDate Element
TOCTitle: NewTaskStartDate Element
ms:assetid: d621417d-eb69-4fdb-abf7-cebd523eaad0
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968699(v=office.12)
ms:contentKeyID: 13188389
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- NewTaskStartDate element
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# NewTaskStartDate Element




Specifies whether the default start date for a new task is the project start date or the current date.

    <NewTaskStartDate>
      IntegerValue
    </NewTaskStartDate>

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

Required Integer

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
<td><p>Project start date</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>Current date</p></td>
</tr>
</tbody>
</table>

## See Also

#### Concepts

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

[XML Schema for the Project Element](xml-schema-for-the-project-element.md)

