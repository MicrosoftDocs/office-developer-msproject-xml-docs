---
title: FreeSlack Element
TOCTitle: FreeSlack Element
ms:assetid: a26cf9d8-e0e9-4c34-a476-24ea8dee4b38
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968623(v=office.12)
ms:contentKeyID: 13188314
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- FreeSlack element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# FreeSlack Element




The actual amount of time that a task can be delayed without delaying any successor tasks. If a task has zero successor tasks, free slack is the amount of time a task can be delayed without delaying the entire project.

    <FreeSlack>
      IntegerValue
    </FreeSlack>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="task-element.md">Task</a></p></td>
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

## Example

The following example shows a task can be delayed by two days, if the work day is eight hours (2 days x 8 hours/day x 60 minutes/hour x 10 tenths/minute = 9600 tenths). The actual slack time (FreeSlack) available in this case is the same as the total slack.

``` xml
<Task>
   . . .
   <FreeSlack>9600</FreeSlack>
   <TotalSlack>9600</TotalSlack>
   . . .
</Task>
```

## See Also

#### Concepts

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

