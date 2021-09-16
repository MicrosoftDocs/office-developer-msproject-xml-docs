---
title: Cost Element
TOCTitle: Cost Element
ms:assetid: 5e1959e5-0af9-4ea1-bbe7-33c7d277cfbd
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968522(v=office.12)
ms:contentKeyID: 13188214
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- Cost element
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# Cost Element




For a Task, Cost is the total scheduled (or projected) cost for a task, based on costs already incurred for work performed by all resources assigned to the task, in addition to the costs planned for the remaining work for the assignment.

For a Resource, it is the total scheduled cost for a resource for all assigned tasks, based on costs already incurred for work performed by the resource on all assigned tasks in addition to the costs planned for all remaining work.

For an Assignment, it is the total projected cost of the assignment when the baseline was saved.

For a Baseline, it is the total scheduled (or projected) cost for an assignment based on costs already incurred for work performed by the resource on a task, in addition to the costs planned for the remaining work for the assignment.

    <Cost>
      DecimalValue
    </Cost>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="task-element.md">Task</a>, <a href="resource-element.md">Resource</a>, <a href="assignment-element.md">Assignment</a>, <a href="baseline-element.md">Baseline</a></p></td>
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

