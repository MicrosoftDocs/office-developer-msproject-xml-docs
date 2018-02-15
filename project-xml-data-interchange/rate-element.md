---
title: Rate Element
TOCTitle: Rate Element
ms:assetid: e9de4a2a-10e0-47f3-81e7-9f98ceafbb4a
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968716(v=office.12)
ms:contentKeyID: 13188406
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- Rate element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# Rate Element




The definition of a time period, and the rates applicable for the resource during that period.

    <Rate>
      ComplexTypeValue
    </Rate>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="rates-element.md">Rates</a></p></td>
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
<th><p>Required/Optional</p></th>
<th><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="ratesfrom-element.md">RatesFrom</a></p></td>
<td><p>Required</p></td>
<td><p>The date the rate becomes available.</p></td>
</tr>
<tr class="even">
<td><p><a href="ratesto-element.md">RatesTo</a></p></td>
<td><p>Required</p></td>
<td><p>The last date the rate is available.</p></td>
</tr>
<tr class="odd">
<td><p><a href="ratetable-element.md">RateTable</a></p></td>
<td><p>Optional</p></td>
<td><p>The unique identifier of the cost rate table (A through E) for the resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="standardrate-element.md">StandardRate</a></p></td>
<td><p>Optional</p></td>
<td><p>The standard pay rate for the resource for the defined period.</p></td>
</tr>
<tr class="odd">
<td><p><a href="standardrateformat-element.md">StandardRateFormat</a></p></td>
<td><p>Optional</p></td>
<td><p>The units used to display the standard rate.</p></td>
</tr>
<tr class="even">
<td><p><a href="overtimerate-element.md">OvertimeRate</a></p></td>
<td><p>Optional</p></td>
<td><p>The overtime rate for the resource for the defined period.</p></td>
</tr>
<tr class="odd">
<td><p><a href="overtimerateformat-element.md">OvertimeRateFormat</a></p></td>
<td><p>Optional</p></td>
<td><p>The units used to display the overtime rate.</p></td>
</tr>
<tr class="even">
<td><p><a href="costperuse-element.md">CostPerUse</a></p></td>
<td><p>Optional</p></td>
<td><p>The cost per use of the resource.</p></td>
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
<p>Maximum: 25</p></td>
</tr>
</tbody>
</table>

## See Also

#### Concepts

[Resource Elements and XML Structure](resource-elements-and-xml-structure.md)

[XML Schema for the Resources Element](xml-schema-for-the-resources-element.md)

