---
title: EarnedValueMethod Element
TOCTitle: EarnedValueMethod Element
ms:assetid: a151ec3f-e5f5-4141-aeaa-c595d57702e8
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968620(v=office.12)
ms:contentKeyID: 13188311
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- EarnedValueMethod element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# EarnedValueMethod Element




For Project, EarnedValueMethod is the default method for calculating earned value.

For Task, it indicates the type of earned value method to use in the task.

    <EarnedValueMethod>
      IntegerValue
    </EarnedValueMethod>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="project-element.md">Project</a>, <a href="task-element.md">Task</a></p></td>
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
<td><p>Use % complete</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>Use physical % complete</p></td>
</tr>
</tbody>
</table>

## See Also

#### Concepts

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

[XML Schema for the Project Element](xml-schema-for-the-project-element.md)

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

