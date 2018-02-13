---
title: Summary Element
TOCTitle: Summary Element
ms:assetid: 3a98d88c-72ab-48dd-a0a7-97928fbea13e
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968468(v=office.12)
ms:contentKeyID: 13188160
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- Summary element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# Summary Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

Indicates whether the task is a summary task or the assignment is on a summary task.

    <Summary>
      BooleanValue
    </Summary>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968611(v=office.12).md">Assignment</a>, <a href="bb968487(v=office.12).md">Task</a></p></td>
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
> You should generally assign resources to individual subtasks, not to a summary task. For more information, see <A href="http://office.microsoft.com/en-us/project/ha101935931033.aspx">Assign a resource to a task</A> in the Project 2007 Help and How-to guide.


## See Also

#### Concepts

[Task Elements and XML Structure](bb968475\(v=office.12\).md)

[XML Schema for the Tasks Element](bb968415\(v=office.12\).md)

[Assignment Elements and XML Structure](bb968738\(v=office.12\).md)

[XML Schema for the Assignments Element](bb968414\(v=office.12\).md)

