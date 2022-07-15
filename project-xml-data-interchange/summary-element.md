---
title: Summary Element
description: Indicates whether the task is a summary task or the assignment is on a summary task.
TOCTitle: Summary Element
ms:assetid: 3a98d88c-72ab-48dd-a0a7-97928fbea13e
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968468(v=office.12)
ms:contentKeyID: 13188160
ms.date: 07/14/2022
mtps_version: v=office.12
f1_keywords:
- Summary element
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# Summary Element

Indicates whether the task is a summary task or the assignment is on a summary task.

```
<Summary>
  BooleanValue
</Summary>
```

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="assignment-element.md">Assignment</a>, <a href="task-element.md">Task</a></p></td>
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

## Text Value

A text value of type boolean is required.

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Value</p></th>
<th><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>0</p></td>
<td><p>False</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>True</p></td>
</tr>
</tbody>
</table>

## Remarks

> [!NOTE]
> You should generally assign resources to individual subtasks, not to a summary task. For more information, see [Assign a resource to a task](https://support.microsoft.com/office/add-resources-to-your-project-1a744960-d960-426a-b687-e42ba3f6c0cb) in the Project 2007 Help and How-to guide.

## See Also

[Task Elements and XML Structure](task-elements-and-xml-structure.md)
[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)
[Assignment Elements and XML Structure](assignment-elements-and-xml-structure.md)
[XML Schema for the Assignments Element](xml-schema-for-the-assignments-element.md)
