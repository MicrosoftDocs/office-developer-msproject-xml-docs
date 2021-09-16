---
title: DefaultFixedCostAccrual Element
TOCTitle: DefaultFixedCostAccrual Element
ms:assetid: f7bd8c0b-b3f8-4e8e-b7fb-59980002ecf3
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968743(v=office.12)
ms:contentKeyID: 13188433
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- DefaultFixedCostAccrual element
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# DefaultFixedCostAccrual Element




The default part of the project where fixed costs are accrued.

    <DefaultFixedCostAccrual>
      IntegerValue
    </DefaultFixedCostAccrual>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="project-element.md">Project</a></p></td>
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

A text value of type integer is required.

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
<td><p>Start</p></td>
</tr>
<tr class="even">
<td><p>2</p></td>
<td><p>Prorated (default)</p></td>
</tr>
<tr class="odd">
<td><p>3</p></td>
<td><p>End</p></td>
</tr>
</tbody>
</table>

## See Also

#### Concepts

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

[XML Schema for the Project Element](xml-schema-for-the-project-element.md)

