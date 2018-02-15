---
title: ResourceSubstitutionEnabled Element
TOCTitle: ResourceSubstitutionEnabled Element
ms:assetid: 268bba0c-25fe-4d1b-b68f-87388ad411fa
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968443(v=office.12)
ms:contentKeyID: 13188136
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- ResourceSubstitutionEnabled element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# ResourceSubstitutionEnabled Element




Indicates whether the custom outline code is used with the Resource Substitution Wizard. only used for outline codes added as enterprise text custom fields.

    <ResourceSubstitutionEnabled>
      BooleanValue
    </ResourceSubstitutionEnabled>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="outlinecode-element.md">OutlineCode</a></p></td>
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

ResourceSubstitutionEnabled can be true only for resource outline codes added to Microsoft Office Project Server 2007 as enterprise resource text custom fields.

## See Also

#### Concepts

[OutlineCode Elements and XML Structure](outlinecode-elements-and-xml-structure.md)

[XML Schema for the OutlineCodes Element](xml-schema-for-the-outlinecodes-element.md)

