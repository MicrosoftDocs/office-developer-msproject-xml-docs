---
title: PercentWorkComplete Element
TOCTitle: PercentWorkComplete Element
ms:assetid: 9c4a9d5f-d0fd-43e9-99c0-bb13c3fd6da6
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968608(v=office.12)
ms:contentKeyID: 13188299
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- PercentWorkComplete element
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# PercentWorkComplete Element




For a Task, PercentWorkComplete is the current status of a task, expressed as the percentage of the task's work that has been completed.

For a Resource, it is the current status of all tasks assigned to a resource, expressed as the total percentage of the resource's work that has been completed.

For an Assignment, it is the current status of an assignment, expressed as the percentage of the assignment's work that has been completed.

    <PercentWorkComplete>
      IntegerValue
    </PercentWorkComplete>

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

