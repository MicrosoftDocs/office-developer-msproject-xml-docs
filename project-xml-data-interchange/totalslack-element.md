---
title: TotalSlack Element
TOCTitle: TotalSlack Element
ms:assetid: a87b9c2d-ea76-4cb7-9848-40295c72fd01
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968632(v=office.12)
ms:contentKeyID: 13188323
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- TotalSlack element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# TotalSlack Element




The amount of time a task can be delayed without delaying a project's finish date. Time is in tenths of a minute.

    <TotalSlack>
      IntegerValue
    </TotalSlack>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968487(v=office.12).md">Task</a></p></td>
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

The following example shows a task can be delayed by two days, if the work day is eight hours (2 days x 8 hours/day x 60 minutes/hour x 10 tenths/minute = 9600 tenths). The actual slack time available in this case is the same as the total slack.

``` xml
<Task>
   . . .
   <FreeSlack>9600</FreeSlack>
   <TotalSlack>9600</TotalSlack>
   . . .
</Task>
```

## See Also

#### Reference

[FreeSlack Element](bb968623\(v=office.12\).md)

#### Concepts

[Task Elements and XML Structure](bb968475\(v=office.12\).md)

[XML Schema for the Tasks Element](bb968415\(v=office.12\).md)

