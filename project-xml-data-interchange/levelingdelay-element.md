---
title: LevelingDelay Element
TOCTitle: LevelingDelay Element
ms:assetid: 02a5a3be-5569-4f08-97b0-c23dceb35861
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968397(v=office.12)
ms:contentKeyID: 13188090
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- LevelingDelay element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# LevelingDelay Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

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
<td><p><a href="bb968487(v=office.12).md">Task</a>, <a href="bb968611(v=office.12).md">Assignment</a></p></td>
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

[LevelingDelayFormat Element](bb968448\(v=office.12\).md)

#### Concepts

[Task Elements and XML Structure](bb968475\(v=office.12\).md)

[XML Schema for the Tasks Element](bb968415\(v=office.12\).md)

[Assignment Elements and XML Structure](bb968738\(v=office.12\).md)

[XML Schema for the Assignments Element](bb968414\(v=office.12\).md)

