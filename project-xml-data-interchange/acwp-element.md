---
title: ACWP Element
TOCTitle: ACWP Element
ms:assetid: e9fd44ae-e18b-4fe7-ad7a-6b5fb1ef9456
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968717(v=office.12)
ms:contentKeyID: 13188407
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- ACWP element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# ACWP Element




ACWP is the actual cost of work performed up to the project status date or the current date.

For a Task, ACWP is the costs incurred for work already done on a task.

For a Resource, it is the sum of ACWP values for all of a resource's assignments.

For an Assignment, it is the costs incurred for work already performed by a resource on a task.

    <ACWP>
      FloatValue
    </ACWP>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="task-element.md">Task</a>, <a href="resource-element.md">Resource</a>, <a href="assignment-element.md">Assignment</a></p></td>
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

## See Also

#### Concepts

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

[Resource Elements and XML Structure](resource-elements-and-xml-structure.md)

[XML Schema for the Resources Element](xml-schema-for-the-resources-element.md)

[Assignment Elements and XML Structure](assignment-elements-and-xml-structure.md)

[XML Schema for the Assignments Element](xml-schema-for-the-assignments-element.md)

