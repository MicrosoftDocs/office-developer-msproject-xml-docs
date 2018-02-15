---
title: Mask Element
TOCTitle: Mask Element
ms:assetid: bd78e7ac-a2b7-40a6-8e8a-2947ae8c01c3
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968659(v=office.12)
ms:contentKeyID: 13188350
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- Mask element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# Mask Element




Indicates whether the custom outline code must be used with all related resources and tasks.

    <Mask>
      ComplexTypeValue
    </Mask>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968478(v=office.12).md">Masks</a></p></td>
</tr>
</tbody>
</table>

## Child Elements

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Element</p></th>
<th><p>Required / Optional</p></th>
<th><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="bb968635(v=office.12).md">Level</a></p></td>
<td><p>Optional</p></td>
<td><p>Level that is assigned to each outline code value, beginning with 1.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968434(v=office.12).md">Type</a></p></td>
<td><p>Optional</p></td>
<td><p>Type of code string for first-level tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968526(v=office.12).md">Length</a></p></td>
<td><p>Optional</p></td>
<td><p>Maximum length in characters of the outline code values, from 1 – 255. If length is any, the value is zero.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968421(v=office.12).md">Separator</a></p></td>
<td><p>Optional</p></td>
<td><p>Character used to separate outline code levels.</p></td>
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
<p>Maximum: Unbounded</p></td>
</tr>
</tbody>
</table>

## Remarks

The four elements of the mask constitute the format in which the outline code must appear.

## See Also

#### Concepts

[OutlineCode Elements and XML Structure](outlinecode-elements-and-xml-structure.md)

[XML Schema for the OutlineCodes Element](xml-schema-for-the-outlinecodes-element.md)

