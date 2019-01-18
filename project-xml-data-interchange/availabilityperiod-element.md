---
title: AvailabilityPeriod Element
TOCTitle: AvailabilityPeriod Element
ms:assetid: a4c03ace-1ef0-41a7-92df-99abc612aa73
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968625(v=office.12)
ms:contentKeyID: 13188316
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- AvailabilityPeriod element
monikerRange: '>= project-client-2007 || project-client-odc'
localization_priority: Normal
---

# AvailabilityPeriod Element




Defines a period when a resource is available.

    <AvailabilityPeriod>
      ComplexTypeValue
    </AvailabilityPeriod>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="availabilityperiods-element.md">AvailabilityPeriods</a></p></td>
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
<td><p><a href="availablefrom-element.md">AvailableFrom</a>, <a href="availableto-element.md">AvailableTo</a>, <a href="availableunits-element.md">AvailableUnits</a></p></td>
</tr>
</tbody>
</table>

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
<td><p><a href="availablefrom-element.md">AvailableFrom</a></p></td>
<td><p>Optional</p></td>
<td><p>The starting date that a resource is available for work at the units specified for the current time period.</p></td>
</tr>
<tr class="even">
<td><p><a href="availableto-element.md">AvailableTo</a></p></td>
<td><p>Optional</p></td>
<td><p>The ending date that a resource will be available for work at the units specified for the current time period.</p></td>
</tr>
<tr class="odd">
<td><p><a href="availableunits-element.md">AvailableUnits</a></p></td>
<td><p>Optional</p></td>
<td><p>The percentage that the resource is available during the specified period.</p></td>
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

## See Also

#### Concepts

[Resource Elements and XML Structure](resource-elements-and-xml-structure.md)

[XML Schema for the Resources Element](xml-schema-for-the-resources-element.md)

