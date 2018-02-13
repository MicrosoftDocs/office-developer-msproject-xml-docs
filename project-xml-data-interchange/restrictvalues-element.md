---
title: RestrictValues Element
TOCTitle: RestrictValues Element
ms:assetid: a6aca4dd-c947-496f-bcce-a4742f73bab3
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968626(v=office.12)
ms:contentKeyID: 13188317
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- RestrictValues element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# RestrictValues Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

Indicates whether the custom field values are restricted to values in the list.

    <RestrictValues>
      BooleanValue
    </RestrictValues>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968669(v=office.12).md">ExtendedAttribute</a></p></td>
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

\<RestrictValues\>0\</RestrictValues\> means that users can type additional values for the custom field.

## See Also

#### Concepts

[ExtendedAttribute Elements and XML Structure](bb968579\(v=office.12\).md)

[XML Schema for the ExtendedAttributes Element](bb968705\(v=office.12\).md)

