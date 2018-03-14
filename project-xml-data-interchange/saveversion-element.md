---
title: SaveVersion Element
TOCTitle: SaveVersion Element
ms:assetid: b6a5948c-cdf5-480d-8b08-d748895809e9
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968654(v=office.12)
ms:contentKeyID: 13188345
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- SaveVersion element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# SaveVersion Element




The version of Microsoft Office Project that saved the XML file.

    <SaveVersion>
      IntegerValue
    </SaveVersion>

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
<td><p>Minimum: 1</p>
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
<th><ul>
<li><p>Value</p></li>
</ul></th>
<th><ul>
<li><p>Description</p></li>
</ul></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><ul>
<li><p>12</p></li>
</ul></td>
<td><ul>
<li><p>Microsoft Office Project 2007</p></li>
</ul></td>
</tr>
</tbody>
</table>

## Remarks

The SaveVersion element is new in Project 2007. Future releases of Project will have additional values of SaveVersion.

## Example

The following example uses the SaveVersion element to indicate that Project 2007 saved the XML file.

``` xml
<Project xmlns="http://schemas.microsoft.com/project">
  …
  <SaveVersion>12</SaveVersion>
  …
</Project>
```

## See Also

#### Concepts

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

[XML Schema for the Project Element](xml-schema-for-the-project-element.md)

