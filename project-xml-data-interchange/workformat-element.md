---
title: WorkFormat Element
TOCTitle: WorkFormat Element
ms:assetid: 6d1d40f3-cd02-4cd7-a28e-605b88518ee4
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968538(v=office.12)
ms:contentKeyID: 13188230
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- WorkFormat element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# WorkFormat Element




The default format for work duration values.

    <WorkFormat>
      IntegerValue
    </WorkFormat>

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
<td><p>1</p></td>
<td><p>m (minutes)</p></td>
</tr>
<tr class="even">
<td><p>2</p></td>
<td><p>h (hours, default))</p></td>
</tr>
<tr class="odd">
<td><p>3</p></td>
<td><p>d (days)</p></td>
</tr>
<tr class="even">
<td><p>4</p></td>
<td><p>w (weeks)</p></td>
</tr>
<tr class="odd">
<td><p>5</p></td>
<td><p>mo (months)</p></td>
</tr>
</tbody>
</table>

## See Also

#### Concepts

[Project Elements and XML Structure](bb968439\(v=office.12\).md)

[XML Schema for the Project Element](bb968695\(v=office.12\).md)

