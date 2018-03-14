---
title: LevelingDelay Element
TOCTitle: LevelingDelay Element
ms:assetid: 02a5a3be-5569-4f08-97b0-c23dceb35861
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968397(v=office.12)
ms:contentKeyID: 13188090
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- LevelingDelay element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# LevelingDelay Element




For a Task, LevelingDelay is the amount of time that a task is to be delayed from its early start date as a result of resource leveling.

For an Assignment, it is the total amount of work scheduled to be performed by a resource on a task.

    <LevelingDelay>
      IntegerValue
    </LevelingDelay>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="task-element.md">Task</a>, <a href="assignment-element.md">Assignment</a></p></td>
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

## Remarks

A LevelingDelay requires the LevelingDelayFormat to be specified. For example, a leveling delay of 3 days in a task is expressed as follows:

``` xml
<Task>
    ...
    <LevelingDelay>3</LevelingDelay>
    <LevelingDelayFormat>7</LevelingDelayFormat>
    ...
</Task>
```

## See Also

#### Reference

[LevelingDelayFormat Element](levelingdelayformat-element.md)

#### Concepts

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

[Assignment Elements and XML Structure](assignment-elements-and-xml-structure.md)

[XML Schema for the Assignments Element](xml-schema-for-the-assignments-element.md)

