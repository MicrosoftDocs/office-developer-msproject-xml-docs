---
title: ActualCost Element
TOCTitle: ActualCost Element
ms:assetid: 91560464-cbfd-46e1-9927-4ecaa218e84b
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968591(v=office.12)
ms:contentKeyID: 13188282
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- ActualCost element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# ActualCost Element




For a Task, ActualCost is the costs incurred for work already performed by all resources on a task, along with any other recorded costs associated with the task.

For a Resource, it is the sum of costs incurred for the work already performed by a resource for all assigned tasks.

For an Assignment, it is the cost incurred for work already performed by a resource on a task.

    <ActualCost>
      DecimalValue
    </ActualCost>

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

