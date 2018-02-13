---
title: ScheduleFromStart Element
TOCTitle: ScheduleFromStart Element
ms:assetid: f786738d-d6f6-46b1-a18b-94548a226150
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968741(v=office.12)
ms:contentKeyID: 13188431
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- ScheduleFromStart element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# ScheduleFromStart Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

Indicates whether the project is scheduled from the start date.

    <ScheduleFromStart>
      BooleanValue
    </ScheduleFromStart>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968701(v=office.12).md">Project</a></p></td>
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
<td><p>False; the project is scheduled from the finish date.</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>True; the project is scheduled from the start date.</p></td>
</tr>
</tbody>
</table>

## See Also

#### Concepts

[Project Elements and XML Structure](bb968439\(v=office.12\).md)

[XML Schema for the Project Element](bb968695\(v=office.12\).md)

