---
title: RemoveFileProperties Element
TOCTitle: RemoveFileProperties Element
ms:assetid: a205c498-80f3-4313-9377-9332324d3717
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968622(v=office.12)
ms:contentKeyID: 13188313
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- RemoveFileProperties element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# RemoveFileProperties Element




Indicates whether to remove all file properties during a save operation.

    <RemoveFileProperties>
      BooleanValue
    </RemoveFileProperties>

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
<td><p>False</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>True</p></td>
</tr>
</tbody>
</table>

## Remarks

If RemoveFileProperties is true, saving the file removes property values such as Author, Company, Manager, Subject, and Title.

## See Also

#### Concepts

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

[XML Schema for the Project Element](xml-schema-for-the-project-element.md)

