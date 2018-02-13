---
title: ValueList Element
TOCTitle: ValueList Element
ms:assetid: d797b79a-8f07-4309-851c-fcf8ffce49d2
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968702(v=office.12)
ms:contentKeyID: 13188392
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- ValueList element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# ValueList Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

When values of extended attributes are specified as properties of elements in the schema, they can either be specified by values or by references to values contained in the list. Applications can assume a value list is ordered in the manner specified by the ValueListSortOrder (ascending or descending).

    <ValueList>
      ComplexTypeValue
    </ValueList>

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

## Child Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968696(v=office.12).md">Value</a></p></td>
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

## Remarks

The ValueList element contains a collection of Value elements for an ExtendedAttribute. Value elements for an OutlineCode element are contained in a Values collection.

## See Also

#### Concepts

[ExtendedAttribute Elements and XML Structure](bb968579\(v=office.12\).md)

[XML Schema for the ExtendedAttributes Element](bb968705\(v=office.12\).md)

