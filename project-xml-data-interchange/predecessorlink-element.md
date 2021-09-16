---
title: PredecessorLink Element
TOCTitle: PredecessorLink Element
ms:assetid: e372749d-6fbd-47a8-b73b-a037b24fcb05
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968712(v=office.12)
ms:contentKeyID: 13188402
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- PredecessorLink element
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# PredecessorLink Element




Defines the predecessor task on which this task depends for its start or finish date.

    <PredecessorLink>
      ComplexTypeValue
    </PredecessorLink>

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

## Child Elements

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Element</p></th>
<th><p>Required/Optional</p></th>
<th><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="predecessoruid-element.md">PredecessorUID</a></p></td>
<td><p>Optional</p></td>
<td><p>Unique ID number for the predecessor task.</p></td>
</tr>
<tr class="even">
<td><p><a href="type-element-multiple-parents.md">Type</a></p></td>
<td><p>Optional</p></td>
<td><p>Type of predecessor task link (FF, FS, SF, SS).</p></td>
</tr>
<tr class="odd">
<td><p><a href="crossproject-element.md">CrossProject</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the task predecessor is part of another project.</p></td>
</tr>
<tr class="even">
<td><p><a href="crossprojectname-element.md">CrossProjectName</a></p></td>
<td><p>Optional</p></td>
<td><p>External predecessor project.</p></td>
</tr>
<tr class="odd">
<td><p><a href="linklag-element.md">LinkLag</a></p></td>
<td><p>Optional</p></td>
<td><p>Amount of lag time (in tenths of a minute) from the predecessor task.</p></td>
</tr>
<tr class="even">
<td><p><a href="lagformat-element.md">LagFormat</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates the time format (hours, days, and so on) for the amount of lag specified in LinkLag.</p></td>
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
<p>Maximum: Unbounded</p></td>
</tr>
</tbody>
</table>

## See Also

#### Concepts

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

