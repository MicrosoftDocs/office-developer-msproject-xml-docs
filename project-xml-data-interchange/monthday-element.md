---
title: MonthDay Element
TOCTitle: MonthDay Element
ms:assetid: d6aadb78-4d79-4a08-81e6-c9a907ed1f28
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968700(v=office.12)
ms:contentKeyID: 13188390
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- MonthDay element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# MonthDay Element




The day of the month on which an exception recurrence is scheduled.

    <MonthDay>
      IntegerValue
    <MonthDay>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968492(v=office.12).md">Exception</a></p></td>
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

## Example

In the following example, the MonthDay element specifies that the exception named New Year's Day occurs on the first day of the month.

``` xml
<Exception>
  <EnteredByOccurrences>0</EnteredByOccurrences>
  <TimePeriod>
    <FromDate>2007-01-01T00:00:00</FromDate>
    <ToDate>2026-01-01T23:59:00</ToDate>
  </TimePeriod>
  <Occurrences>20</Occurrences>
  <Name>New Year's Day</Name>
  <Type>2</Type>
  <Month>0</Month>
  <MonthDay>1</MonthDay>
  <DayWorking>0</DayWorking>
</Exception>
```

## See Also

#### Concepts

[Calendar Elements and XML Structure](bb968563\(v=office.12\).md)

[XML Schema for the Calendars Element](bb968557\(v=office.12\).md)

