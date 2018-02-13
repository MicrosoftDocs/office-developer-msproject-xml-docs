---
title: WorkVariance Element
TOCTitle: WorkVariance Element
ms:assetid: cd8c71ed-bf3a-4013-8e17-dd970785e79b
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968689(v=office.12)
ms:contentKeyID: 13188379
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- WorkVariance element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# WorkVariance Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

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

[Task Elements and XML Structure](bb968475\(v=office.12\).md)

[XML Schema for the Tasks Element](bb968415\(v=office.12\).md)

[Resource Elements and XML Structure](bb968445\(v=office.12\).md)

[XML Schema for the Resources Element](bb968511\(v=office.12\).md)

[Assignment Elements and XML Structure](bb968738\(v=office.12\).md)

[XML Schema for the Assignments Element](bb968414\(v=office.12\).md)

