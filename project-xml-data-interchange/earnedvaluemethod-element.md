---
title: EarnedValueMethod Element
TOCTitle: EarnedValueMethod Element
ms:assetid: a151ec3f-e5f5-4141-aeaa-c595d57702e8
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968620(v=office.12)
ms:contentKeyID: 13188311
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- EarnedValueMethod element
---

# EarnedValueMethod Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

For Project, EarnedValueMethod is the default method for calculating earned value.

For Task, it indicates the type of earned value method to use in the task.

    <EarnedValueMethod>
      IntegerValue
    </EarnedValueMethod>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968701(v=office.12).md">Project</a>, <a href="bb968487(v=office.12).md">Task</a></p></td>
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

A text value of type Integer is required.

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
<td><p>Use % complete</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>Use physical % complete</p></td>
</tr>
</tbody>
</table>

## See Also

#### Concepts

[Project Elements and XML Structure](bb968439\(v=office.12\).md)

[XML Schema for the Project Element](bb968695\(v=office.12\).md)

[Task Elements and XML Structure](bb968475\(v=office.12\).md)

[XML Schema for the Tasks Element](bb968415\(v=office.12\).md)

