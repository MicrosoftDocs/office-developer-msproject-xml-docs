---
title: BaseCalendarUID Element
TOCTitle: BaseCalendarUID Element
ms:assetid: f82f2ed0-9c87-4d05-940d-7fe6ef02f09c
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968744(v=office.12)
ms:contentKeyID: 13188434
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- BaseCalendarUID element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# BaseCalendarUID Element




The unique ID for the base calendar on which this calendar depends; only used if this calendar is not a base calendar.

    <BaseCalendarUID>
      IntegerValue
    </BaseCalendarUID>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="calendar-element.md">Calendar</a></p></td>
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

For the value \<BaseCalendarUID\>-1\</BaseCalendarUID\>, the calendar is a base calendar.

## See Also

#### Concepts

[Calendar Elements and XML Structure](calendar-elements-and-xml-structure.md)

[XML Schema for the Calendars Element](xml-schema-for-the-calendars-element.md)

