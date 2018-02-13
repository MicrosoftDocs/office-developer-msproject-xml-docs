---
title: Value Element
TOCTitle: Value Element
ms:assetid: d367ebe0-7f26-4e01-8c3b-b248996da52d
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968696(v=office.12)
ms:contentKeyID: 13188386
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- Value element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# Value Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

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
<td><p><a href="bb968702(v=office.12).md">ValueList</a>, <a href="bb968604(v=office.12).md">Values</a>, <a href="bb968669(v=office.12).md">ExtendedAttribute</a>, <a href="https://msdn.microsoft.com/en-us/library/office%7cps12con%7c%7e%5chtml%5cpjxml_elemtimephaseddata_hv01056849.xml.htm(v=office.12)">TimephasedData</a></p></td>
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
<td><p><a href="bb968406(v=office.12).md">ValueID</a></p></td>
<td><p>Optional</p></td>
<td><p>Unique ID for the custom outline code.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968634(v=office.12).md">FieldGUID</a></p></td>
<td><p>Required</p></td>
<td><p>New in Project 2007. GUID of the outline code value.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968434(v=office.12).md">Type</a></p></td>
<td><p>Required</p></td>
<td><p>New in Project 2007. Type of the outline code (text, date, duration, flag, cost, number)</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968739(v=office.12).md">ParentValueID</a> </p></td>
<td><p>Optional</p></td>
<td><p>Unique ID for the parent node of the custom outline code.</p></td>
</tr>
<tr class="odd">
<td><p>Value</p></td>
<td><p>Optional</p></td>
<td><p>Actual value of the custom outline code.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968567(v=office.12).md">Description</a></p></td>
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
<td><p><a href="bb968437(v=office.12).md">ID</a> </p></td>
<td><p>Required</p></td>
<td><p>Unique ID for the outline code or custom field.</p></td>
</tr>
<tr class="even">
<td><p>Value</p></td>
<td><p>Optional</p></td>
<td><p>Actual value of the outline code or custom field.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968567(v=office.12).md">Description</a></p></td>
<td><p>Optional</p></td>
<td><p>Description of the outline code or custom field.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968486(v=office.12).md">Phonetic</a></p></td>
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

[OutlineCode Element](bb968410\(v=office.12\).md)

[Assignment Element](bb968611\(v=office.12\).md)

[Baseline Element](bb968599\(v=office.12\).md)

[Resource Element](bb968715\(v=office.12\).md)

[Task Element](bb968487\(v=office.12\).md)

#### Concepts

[OutlineCode Elements and XML Structure](bb968596\(v=office.12\).md)

[XML Schema for the OutlineCodes Element](bb968584\(v=office.12\).md)

[ExtendedAttribute Elements and XML Structure](bb968579\(v=office.12\).md)

[XML Schema for the ExtendedAttributes Element](bb968705\(v=office.12\).md)

[TimephasedDataType Elements and XML Structure](bb968722\(v=office.12\).md)

[XML Schema for the TimephasedDataType Complex Type](bb968734\(v=office.12\).md)

