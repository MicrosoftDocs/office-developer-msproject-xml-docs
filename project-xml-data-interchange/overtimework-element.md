---
title: OvertimeWork Element
TOCTitle: OvertimeWork Element
ms:assetid: 9d534b47-3d09-4ef7-90ee-416c3418d97d
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968609(v=office.12)
ms:contentKeyID: 13188300
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- OvertimeWork element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# OvertimeWork Element




For a Task, OvertimeWork is the amount of overtime scheduled to be performed by all resources assigned to a task and charged at overtime rates.

For a Resource, it is the amount of overtime to be performed for all tasks assigned to a resource and charged at the resource's overtime rate.

For an Assignment, it is the amount of overtime to be performed by a resource on a task; charged at the resource's overtime rate.

    <OvertimeWork>
      DurationValue
    </OvertimeWork>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968487(v=office.12).md">Task</a>, <a href="bb968715(v=office.12).md">Resource</a>, <a href="bb968611(v=office.12).md">Assignment</a></p></td>
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

