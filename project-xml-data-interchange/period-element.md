---
title: Period Element
TOCTitle: Period Element
ms:assetid: 7a3c8c71-6993-4b8b-8b50-9743ea95e732
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968554(v=office.12)
ms:contentKeyID: 13188246
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- Period element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# Period Element




The period of recurrence for the calendar exception.

    <Period>
      IntegerValue
    </Period>

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

In the following example, the Period element indicates that the calendar exception named Team Meeting occurs once every two weeks.

``` xml
<Exception>
  <EnteredByOccurrences>1</EnteredByOccurrences>
  <TimePeriod>
    <FromDate>2007-01-01T00:00:00</FromDate>
    <ToDate>2007-12-26T23:59:00</ToDate>
  </TimePeriod>
  <Occurrences>52</Occurrences>
  <Name>Team Meeting</Name>
  <Type>6</Type>
  <Period>2</Period>
  <DaysOfWeek>8</DaysOfWeek>
  <DayWorking>1</DayWorking>
  <WorkingTimes>
    <WorkingTime>
      <FromTime>08:00:00</FromTime>
      <ToTime>12:00:00</ToTime>
    </WorkingTime>
    <WorkingTime>
      <FromTime>13:00:00</FromTime>
      <ToTime>14:00:00</ToTime>
    </WorkingTime>
    <WorkingTime>
      <FromTime>15:00:00</FromTime>
      <ToTime>16:00:00</ToTime>
    </WorkingTime>
  </WorkingTimes>
</Exception>
```

## See Also

#### Concepts

[Calendar Elements and XML Structure](calendar-elements-and-xml-structure.md)

[XML Schema for the Calendars Element](xml-schema-for-the-calendars-element.md)

