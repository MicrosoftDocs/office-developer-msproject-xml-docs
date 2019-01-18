---
title: CommitmentType Element
TOCTitle: CommitmentType Element
ms:assetid: e00871cd-1614-4fa8-83b2-66f2d1130428
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968709(v=office.12)
ms:contentKeyID: 13188399
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- CommitmentType element
monikerRange: '>= project-client-2007 || project-client-odc'
localization_priority: Normal
---

# CommitmentType Element




Indicates whether the task has an associated deliverable or a dependency on an associated deliverable.

    <CommitmentType>
      IntegerValue
    </CommitmentType>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="task-element.md">Task</a></p></td>
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

A text value of type integer is required.

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
<td><p>The task has no deliverable or dependency on a deliverable.</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>The task has an associated deliverable.</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>The task has a dependency on an associated deliverable.</p></td>
</tr>
</tbody>
</table>

## See Also

#### Concepts

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

