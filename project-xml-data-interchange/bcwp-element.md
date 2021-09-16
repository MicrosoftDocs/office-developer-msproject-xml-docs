---
title: BCWP Element
TOCTitle: BCWP Element
ms:assetid: e4f0b550-4c8a-4d66-8041-6bed732a03a6
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968714(v=office.12)
ms:contentKeyID: 13188404
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- BCWP element
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# BCWP Element




BCWP is the budgeted cost of work performed.

For a Task, BCWP is the cumulative value of the task's timephased percent complete multiplied by the task's timephased baseline cost, up to the status date or today's date.

For a Resource, it is the rolled-up summary of a resource's BCWP values for all assigned tasks, calculated up to the status date or today's date.

For an Assignment, it is the budgeted cost of the work performed on the assignment to date.

For a Baseline in a Task, BCWP is the cumulative value of the task's timephased percent complete multiplied by the task's timephased baseline cost, up to the status date or today's date.

For a Baseline in a Resource, it is the budgeted cost of the work performed by the resource on the project to-date.

For a Baseline in an Assignment, it is the budgeted cost of the work performed on the assignment to-date.

    <BCWP>
      DecimalValue
    </BCWP>

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

