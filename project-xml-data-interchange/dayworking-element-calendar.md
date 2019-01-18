---
title: DayWorking Element (Calendar)
TOCTitle: DayWorking Element
ms:assetid: c049f7a9-2ef3-4e48-89fa-6d20d8b337f1
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968665(v=office.12)
ms:contentKeyID: 13188356
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- DayWorking element
monikerRange: '>= project-client-2007 || project-client-odc'
localization_priority: Normal
---

# DayWorking Element (Calendar)




Indicates whether the specified date or day type is a working day.

    <DayWorking>
      BooleanValue
    </DayWorking>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="weekday-element.md">WeekDay</a></p></td>
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
<td><p>False, non-working day.</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>True, working day.</p></td>
</tr>
</tbody>
</table>

## See Also

#### Concepts

[Calendar Elements and XML Structure](calendar-elements-and-xml-structure.md)

[XML Schema for the Calendars Element](xml-schema-for-the-calendars-element.md)

