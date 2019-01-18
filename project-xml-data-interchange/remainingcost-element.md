---
title: RemainingCost Element
TOCTitle: RemainingCost Element
ms:assetid: f14789f4-9450-40a8-b43d-b66f314518bd
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968728(v=office.12)
ms:contentKeyID: 13188418
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- RemainingCost element
monikerRange: '>= project-client-2007 || project-client-odc'
localization_priority: Normal
---

# RemainingCost Element




For a Task, RemainingCost is the remaining scheduled expense of a task that will be incurred in completing the remaining scheduled work by all resources assigned to a task.

For a Resource, it is the remaining scheduled expense that will be incurred in completing the remaining work assigned to a resource.

For an Assignment, it is the costs associated with completing all remaining scheduled work by any resources on a specific task.

    <RemainingCost>
      DecimalValue
    </RemainingCost>

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

