---
title: WorkVariance Element
TOCTitle: WorkVariance Element
ms:assetid: cd8c71ed-bf3a-4013-8e17-dd970785e79b
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968689(v=office.12)
ms:contentKeyID: 13188379
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- WorkVariance element
monikerRange: '>= project-client-2007 || project-client-odc'
localization_priority: Normal
---

# WorkVariance Element




For a Task, WorkVariance is the difference between a task's baseline work and the currently scheduled work.

For a Resource, it is the difference between a resource's total baseline work and the currently scheduled work.

For an Assignment, it is the variance of assignment work from the baseline work, expressed as minutes x 1000.

    <WorkVariance>
      FloatValue
    </WorkVariance>

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

