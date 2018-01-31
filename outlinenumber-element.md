---
title: OutlineNumber Element
TOCTitle: OutlineNumber Element
ms:assetid: b3a0a187-116d-4dec-898e-2cc3381525a5
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968651(v=office.12)
ms:contentKeyID: 13188342
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- OutlineNumber element
---

# OutlineNumber Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

Indicates the exact position of a task in the outline. For example, "7.2" indicates that a task is the second subtask under the seventh top-level summary task.

    <OutlineNumber>
      String(512)Value
    </OutlineNumber>

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

## Remarks

The OutlineNumber is a string indicating the task's position in the outline hierarchy; "5.2.6" is an example. The OutlineLevel is a simple number, such as 2.

## See Also

#### Concepts

[Task Elements and XML Structure](bb968475\(v=office.12\).md)

[XML Schema for the Tasks Element](bb968415\(v=office.12\).md)

