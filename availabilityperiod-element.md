---
title: AvailabilityPeriod Element
TOCTitle: AvailabilityPeriod Element
ms:assetid: a4c03ace-1ef0-41a7-92df-99abc612aa73
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968625(v=office.12)
ms:contentKeyID: 13188316
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- AvailabilityPeriod element
---

# AvailabilityPeriod Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

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
<td><p><a href="bb968747(v=office.12).md">AvailabilityPeriods</a></p></td>
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
<td><p><a href="bb968686(v=office.12).md">AvailableFrom</a>, <a href="bb968648(v=office.12).md">AvailableTo</a>, <a href="bb968515(v=office.12).md">AvailableUnits</a></p></td>
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
<td><p><a href="bb968686(v=office.12).md">AvailableFrom</a></p></td>
<td><p>Optional</p></td>
<td><p>The starting date that a resource is available for work at the units specified for the current time period.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968648(v=office.12).md">AvailableTo</a></p></td>
<td><p>Optional</p></td>
<td><p>The ending date that a resource will be available for work at the units specified for the current time period.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968515(v=office.12).md">AvailableUnits</a></p></td>
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

[Resource Elements and XML Structure](bb968445\(v=office.12\).md)

[XML Schema for the Resources Element](bb968511\(v=office.12\).md)

