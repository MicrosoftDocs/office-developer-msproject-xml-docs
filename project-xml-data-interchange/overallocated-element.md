---
title: OverAllocated Element
TOCTitle: OverAllocated Element
ms:assetid: 9f8faa7d-0f6a-4822-99a0-aaf381af279b
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968615(v=office.12)
ms:contentKeyID: 13188306
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- OverAllocated element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# OverAllocated Element




For a Task, Overallocated indicates whether an assigned resource on a task has been assigned to more work on the task than can be done within the normal working capacity.

For a Resource, it indicates whether the resource is assigned more work on all tasks than can be done within the normal working capacity.

For an Assignment, it indicates whether a resource is assigned to more work on a specific task than can be done within the resource's normal working capacity.

    <Overallocated>
      BooleanValue
    </Overallocated>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968487(v=office.12).md">Task</a>,<a href="bb968715(v=office.12).md">Resource</a>, <a href="bb968611(v=office.12).md">Assignment</a></p></td>
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

## See Also

#### Concepts

[Task Elements and XML Structure](bb968475\(v=office.12\).md)

[XML Schema for the Tasks Element](bb968415\(v=office.12\).md)

[Resource Elements and XML Structure](bb968445\(v=office.12\).md)

[XML Schema for the Resources Element](bb968511\(v=office.12\).md)

[Assignment Elements and XML Structure](bb968738\(v=office.12\).md)

[XML Schema for the Assignments Element](bb968414\(v=office.12\).md)
