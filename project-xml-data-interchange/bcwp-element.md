---
title: BCWP Element
TOCTitle: BCWP Element
ms:assetid: e4f0b550-4c8a-4d66-8041-6bed732a03a6
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968714(v=office.12)
ms:contentKeyID: 13188404
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- BCWP element
monikerRange: '>= project-client-2007 || project-client-odc'
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
<td><p><a href="bb968487(v=office.12).md">Task</a>, <a href="bb968715(v=office.12).md">Resource</a>, <a href="bb968611(v=office.12).md">Assignment</a>, <a href="bb968599(v=office.12).md">Baseline</a></p></td>
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

[Task Elements and XML Structure](bb968475\(v=office.12\).md)

[XML Schema for the Tasks Element](bb968415\(v=office.12\).md)

[Resource Elements and XML Structure](bb968445\(v=office.12\).md)

[XML Schema for the Resources Element](bb968511\(v=office.12\).md)

[Assignment Elements and XML Structure](bb968738\(v=office.12\).md)

[XML Schema for the Assignments Element](bb968414\(v=office.12\).md)

