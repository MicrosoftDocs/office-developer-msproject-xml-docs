---
title: Value Element
TOCTitle: Value Element
ms:assetid: d367ebe0-7f26-4e01-8c3b-b248996da52d
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968696(v=office.12)
ms:contentKeyID: 13188386
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- Value element
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
description: Learn about the Value Element in Microsoft Office Project's XML Data Interchange. Understand its role in OutlineCode, ExtendedAttribute, and TimephasedData elements.
---

# Value Element




In an OutlineCode element, Value is the actual value of the custom outline code.

In an ExtendedAttribute element, Value is the actual value of an extended attribute (custom field).

In a TimephasedData element, Value is the value for each unit in the timephased data record.

    <Value>
      StringValue
    </Value>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="valuelist-element.md">ValueList</a>, <a href="values-element.md">Values</a>, <a href="extendedattribute-element.md">ExtendedAttribute</a>, <a href="https://msdn.microsoft.com/en-us/library/office%7cps12con%7c%7e%5chtml%5cpjxml_elemtimephaseddata_hv01056849.xml.htm(v=office.12)">TimephasedData</a>, <a href="enterpriseextendedattribute-element.md">EnterpriseExtendedAttribute</a></p></td>
</tr>
</tbody>
</table>

## Child Elements within OutlineCode

Values is the parent of a Value element within an OutlineCode element.

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th><p><strong>Element</strong></p></th>
<th><p><strong>Required/Optional</strong></p></th>
<th><p><strong>Description</strong></p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="valueid-element.md">ValueID</a></p></td>
<td><p>Optional</p></td>
<td><p>Unique ID for the custom outline code.</p></td>
</tr>
<tr class="even">
<td><p><a href="fieldguid-element.md">FieldGUID</a></p></td>
<td><p>Required</p></td>
<td><p>New in Project 2007. GUID of the outline code value.</p></td>
</tr>
<tr class="odd">
<td><p><a href="type-element-multiple-parents.md">Type</a></p></td>
<td><p>Required</p></td>
<td><p>New in Project 2007. Type of the outline code (text, date, duration, flag, cost, number)</p></td>
</tr>
<tr class="even">
<td><p><a href="parentvalueid-element.md">ParentValueID</a> </p></td>
<td><p>Optional</p></td>
<td><p>Unique ID for the parent node of the custom outline code.</p></td>
</tr>
<tr class="odd">
<td><p>Value</p></td>
<td><p>Optional</p></td>
<td><p>Actual value of the custom outline code.</p></td>
</tr>
<tr class="even">
<td><p><a href="description-element.md">Description</a></p></td>
<td><p>Optional</p></td>
<td><p>Description of the custom outline code.</p></td>
</tr>
</tbody>
</table>

## Child Elements within ExtendedAttribute

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th><p><strong>Element</strong></p></th>
<th><p><strong>Required/Optional</strong></p></th>
<th><p><strong>Description</strong></p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="id-element.md">ID</a> </p></td>
<td><p>Required</p></td>
<td><p>Unique ID for the outline code or custom field.</p></td>
</tr>
<tr class="even">
<td><p>Value</p></td>
<td><p>Optional</p></td>
<td><p>Actual value of the outline code or custom field.</p></td>
</tr>
<tr class="odd">
<td><p><a href="description-element.md">Description</a></p></td>
<td><p>Optional</p></td>
<td><p>Description of the outline code or custom field.</p></td>
</tr>
<tr class="even">
<td><p><a href="phonetic-element.md">Phonetic</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Phonetic information for custom field or outline code names.</p></td>
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

Value is recursive in an OutlineCode as part of the Values Element, and in ExtendedAttribute as part of a ValueList.

TimephasedData elements occur in Assignment , Baseline , Resource , and Task elements.

Child elements of Value can appear in any order.

## See Also

#### Reference

[OutlineCode Element](outlinecode-element.md)

[Assignment Element](assignment-element.md)

[Baseline Element](baseline-element.md)

[Resource Element](resource-element.md)

[Task Element](task-element.md)

#### Concepts

[OutlineCode Elements and XML Structure](outlinecode-elements-and-xml-structure.md)

[XML Schema for the OutlineCodes Element](xml-schema-for-the-outlinecodes-element.md)

[ExtendedAttribute Elements and XML Structure](extendedattribute-elements-and-xml-structure.md)

[XML Schema for the ExtendedAttributes Element](xml-schema-for-the-extendedattributes-element.md)

[TimephasedDataType Elements and XML Structure](timephaseddatatype-elements-and-xml-structure.md)

[XML Schema for the TimephasedDataType Complex Type](xml-schema-for-the-timephaseddatatype-complex-type.md)

