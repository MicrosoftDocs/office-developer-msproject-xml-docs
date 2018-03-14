---
title: Work Element
TOCTitle: Work Element
ms:assetid: 84494840-6469-4cbd-ae35-8246d88dfe97
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968571(v=office.12)
ms:contentKeyID: 13188262
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- Work element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# Work Element




For a Task, Work is the total amount of work scheduled to be performed on a task by all assigned resources.

For a Resource, it is the total amount of work scheduled to be performed by a resource on all assigned tasks.

For an Assignment, it is the total amount of work scheduled to be performed by a resource on a task.

For a Baseline, it is the scheduled work for the task, resource or assignment when the baseline was saved.

    <Work>
      DurationValue
    </Work>

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

## Example

The following example shows there are 16 hours of work scheduled for all resources on task T3. Because the scheduled duration is also 16 hours, work on the task hasn't started. The Work value PT16H0M0S specifies 16 hours, 0 minutes, 0 seconds. The PT stands for Project Time and is for internal use.

``` xml
<Task>
   <UID>3</UID>
   <ID>3</ID>
   <Name>T3</Name>
   <Type>1</Type>
   <IsNull>0</IsNull>
   <CreateDate>2007-11-09T15:30:00</CreateDate>
   <WBS>3</WBS>
   <OutlineNumber>3</OutlineNumber>
   <OutlineLevel>1</OutlineLevel>
   <Priority>500</Priority>
   <Start>2007-11-15T08:00:00</Start>
   <Finish>2007-11-16T17:00:00</Finish>
   <Duration>PT16H0M0S</Duration>
   <DurationFormat>53</DurationFormat>
   <Work>PT16H0M0S</Work>
   . . .
</Task>
```

## See Also

#### Concepts

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

[Resource Elements and XML Structure](resource-elements-and-xml-structure.md)

[XML Schema for the Resources Element](xml-schema-for-the-resources-element.md)

[Assignment Elements and XML Structure](assignment-elements-and-xml-structure.md)

[XML Schema for the Assignments Element](xml-schema-for-the-assignments-element.md)

