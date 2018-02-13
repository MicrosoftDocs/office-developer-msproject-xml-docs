---
title: TimePeriod Element (Calendar)
TOCTitle: TimePeriod Element
ms:assetid: bded10b6-c40c-4d6e-83c2-0ec82dd3eac8
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968661(v=office.12)
ms:contentKeyID: 13188352
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- TimePeriod element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# TimePeriod Element (Calendar)




Defines a set of exception days or a work week.

    <TimePeriod>
      ComplexTypeValue
    </TimePeriod>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968433(v=office.12).md">WeekDay</a>, <a href="bb968525(v=office.12).md">WorkWeek</a></p></td>
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
<td><p><a href="bb968583(v=office.12).md">FromDate</a></p></td>
<td><p>Optional</p></td>
<td><p>Start date of the calendar exception or work week.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968399(v=office.12).md">ToDate</a></p></td>
<td><p>Optional</p></td>
<td><p>End date of the calendar exception or work week.</p></td>
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

For an example that includes a calendar exception and a work week, see [Calendar Element](bb968481\(v=office.12\).md).

## See Also

#### Concepts

[Calendar Elements and XML Structure](bb968563\(v=office.12\).md)

[XML Schema for the Calendars Element](bb968557\(v=office.12\).md)

