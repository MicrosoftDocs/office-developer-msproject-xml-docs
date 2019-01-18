---
title: WorkGroup Element
TOCTitle: WorkGroup Element
ms:assetid: ed14d8e2-f8d6-4565-92db-6b1a7c91558d
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968721(v=office.12)
ms:contentKeyID: 13188411
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- WorkGroup element
monikerRange: '>= project-client-2007 || project-client-odc'
localization_priority: Normal
---

# WorkGroup Element




The type of workgroup to which the resource belongs. WorkGroup also specifies the type of messaging method used to communicate with the project team.

    <WorkGroup>
      IntegerValue
    </WorkGroup>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="resource-element.md">Resource</a></p></td>
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

Required Integer value.

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
<td><p>Default</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>None; workgroup messaging is not used on this project</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>E-mail only</p></td>
</tr>
<tr class="even">
<td><p>3</p></td>
<td><p>Web (Project Web Access)</p></td>
</tr>
</tbody>
</table>

## See Also

#### Concepts

[Resource Elements and XML Structure](resource-elements-and-xml-structure.md)

[XML Schema for the Resources Element](xml-schema-for-the-resources-element.md)

