---
title: ExternalTask Element
TOCTitle: ExternalTask Element
ms:assetid: 96f30b4f-3b97-45d0-964a-eb28a4042af1
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968595(v=office.12)
ms:contentKeyID: 13188286
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- ExternalTask element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# ExternalTask Element




Indicates whether a task in an external project links to the task.

    <ExternalTask>
      BooleanValue
    </ExternalTask>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968487(v=office.12).md">Task</a></p></td>
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
<td><p>False, the task originates in the current project and has no external links</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>True, the task links to a task in an external project.</p></td>
</tr>
</tbody>
</table>

## See Also

#### Concepts

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

