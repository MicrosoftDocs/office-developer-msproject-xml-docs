---
title: ValueID Element
TOCTitle: ValueID Element
ms:assetid: 0b4257c5-1238-4f8d-81fa-6fe80bb5af3e
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968406(v=office.12)
ms:contentKeyID: 13188099
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- ValueID element
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# ValueID Element




In OutlineCode, ValueID is the local ID of an outline code value.

In ExtendedAttribute, it is the ID of the value of an extended attribute (a custom field). ValueID is unique only within the project.

    <ValueID>
      IntegerValue
    </ValueID>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="value-element.md">Value</a></p></td>
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

 ValueID is a child of the Value element in an OutlineCode. The Values element contains a collection of Value elements. ValueID is required for Microsoft Office Project 2003 to read XML files saved from Project 2007. Project 2007 ignores ValueID and uses FieldGUID.

## Remarks

An ExtendedAttribute also contains a Value element, but there the value is part of a ValueList collection; an ExtendedAttribute value has an ID, not a ValueID.

## See Also

#### Reference

[FieldGUID Element](fieldguid-element.md)

#### Concepts

[OutlineCode Elements and XML Structure](outlinecode-elements-and-xml-structure.md)

[XML Schema for the OutlineCodes Element](xml-schema-for-the-outlinecodes-element.md)

[ExtendedAttribute Elements and XML Structure](extendedattribute-elements-and-xml-structure.md)

[XML Schema for the ExtendedAttributes Element](xml-schema-for-the-extendedattributes-element.md)

