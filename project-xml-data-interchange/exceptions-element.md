---
title: Exceptions Element
TOCTitle: Exceptions Element
ms:assetid: a0b410df-e930-4b2c-89a2-823e2359f800
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968618(v=office.12)
ms:contentKeyID: 13188309
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- Exceptions element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# Exceptions Element




The collection of exceptions associated with a calendar.

    <Exceptions>
      <Exception>…</Exception>
    </Exceptions>

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

## Child Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="exception-element.md">Exception</a></p></td>
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

The following example contains definitions for two calendar exceptions in the Exceptions element. New Year's Day is defined yearly by the day of the month (Type = 2). Thanksgiving is defined yearly by position (Type = 3), where the holiday is on the fourth (MonthPosition = 3) Thursday (MonthItem = 7) in November (Month = 10).

``` xml
<Exceptions>
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
  <Exception>
    <EnteredByOccurrences>0</EnteredByOccurrences>
    <TimePeriod>
      <FromDate>2007-11-22T00:00:00</FromDate>
      <ToDate>2026-11-30T23:59:00</ToDate>
    </TimePeriod>
    <Occurrences>20</Occurrences>
    <Name>Thanksgiving</Name>
    <Type>3</Type>
    <Month>10</Month>
    <MonthItem>7</MonthItem>
    <MonthPosition>3</MonthPosition>
    <DayWorking>0</DayWorking>
  </Exception>
</Exceptions>
```

## See Also

#### Concepts

[Calendar Elements and XML Structure](calendar-elements-and-xml-structure.md)

[XML Schema for the Calendars Element](xml-schema-for-the-calendars-element.md)

