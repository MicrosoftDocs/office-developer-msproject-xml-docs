---
title: BCWS Element
TOCTitle: BCWS Element
ms:assetid: 0e9e4541-0619-4545-bc05-63826397c10f
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968411(v=office.12)
ms:contentKeyID: 13188104
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- BCWS element
monikerRange: '>= project-client-2007 || project-client-odc'
localization_priority: Normal
---

# BCWS Element




BCWS is the budgeted cost of work scheduled.

For a Task, BCWS is the cumulative timephased costs up to the status date or today's date.

For a Resource, it is the rolled-up summary of a resource's BCWS values for all assigned tasks.

For an Assignment, it is the budgeted cost of work on the assignment.

For a Baseline in a Task, BCWS is the cumulative timephased baseline costs up to the status date or today's date.

For a Baseline in a Resource, it is the budgeted cost of the work performed by the resource.

For a Baseline in an Assignment, it is the budgeted cost of work on the assignment to the current date.

    <BCWS>
      DecimalValue
    </BCWS>

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

