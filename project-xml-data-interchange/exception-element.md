---
title: Exception Element
TOCTitle: Exception Element
ms:assetid: 4918cdc1-9871-4124-8dba-6df6a7f49512
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968492(v=office.12)
ms:contentKeyID: 13188184
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- Exception element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# Exception Element




The Exception element defines a single calendar exception.

    <Exception>
            ComplexTypeValue
    </Exception>

## ent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="exceptions-element.md">Exceptions</a></p></td>
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
<td><p><a href="enteredbyoccurrences-element.md">EnteredByOccurrences</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the range of recurrence for the calendar exception is defined by a number of occurrences, or by a finish date.</p></td>
</tr>
<tr class="even">
<td><p><a href="timeperiod-element-calendar.md">TimePeriod</a></p></td>
<td><p>Optional</p></td>
<td><p>Defines a set of exception days.</p></td>
</tr>
<tr class="odd">
<td><p><a href="occurrences-element.md">Occurrences</a></p></td>
<td><p>Optional</p></td>
<td><p>Number of occurrences for which the calendar exception is valid.</p></td>
</tr>
<tr class="even">
<td><p><a href="name-element.md">Name</a></p></td>
<td><p>Optional</p></td>
<td><p>Name of the calendar exception.</p></td>
</tr>
<tr class="odd">
<td><p><a href="https://msdn.microsoft.com/en-us/library/office%7cps12con%7c%7e%5chtml%5cdc9db984-4269-46c4-a911-cba802cb3d0a.htm(v=office.12)">Type</a></p></td>
<td><p>Optional</p></td>
<td><p>Type of calendar exception (daily, yearly by day of the month, monthly by position, weekly, by day count, and so on).</p></td>
</tr>
<tr class="even">
<td><p><a href="period-element.md">Period</a></p></td>
<td><p>Optional</p></td>
<td><p>The period of recurrence for the exception.</p></td>
</tr>
<tr class="odd">
<td><p><a href="daysofweek-element.md">DaysOfWeek</a></p></td>
<td><p>Optional</p></td>
<td><p>Specifies the day or days of the week the exception is valid.</p></td>
</tr>
<tr class="even">
<td><p><a href="monthitem-element.md">MonthItem</a></p></td>
<td><p>Optional</p></td>
<td><p>The month item for which an exception recurrence is scheduled (day, weekday, Sunday, Monday, and so on).</p></td>
</tr>
<tr class="odd">
<td><p><a href="monthposition-element.md">MonthPosition</a></p></td>
<td><p>Optional</p></td>
<td><p>The position of a month item within a month (first, second, third, fourth, or last).</p></td>
</tr>
<tr class="even">
<td><p><a href="month-element.md">Month</a></p></td>
<td><p>Optional</p></td>
<td><p>The month for which an exception recurrence is scheduled ( 0 = January, …, 11 = December).</p></td>
</tr>
<tr class="odd">
<td><p><a href="monthday-element.md">MonthDay</a></p></td>
<td><p>Optional</p></td>
<td><p>The day of the month on which an exception recurrence is scheduled.</p></td>
</tr>
<tr class="even">
<td><p><a href="dayworking-element-calendar.md">DayWorking</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the specified exception day type is a working day.</p></td>
</tr>
<tr class="odd">
<td><p><a href="workingtimes-element-calendar.md">WorkingTimes</a></p></td>
<td><p>Optional</p></td>
<td><p>The collection of working times that define the time worked on the working day. There must be at least one WorkingTime and a maximum of five specified.</p></td>
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

## Example

In the following example, the Exception element defines a calendar exception for the 20 occurrences of New Year's Day from January 1, 1997 to January 1, 2026.

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

[Calendar Elements and XML Structure](calendar-elements-and-xml-structure.md)

[XML Schema for the Calendars Element](xml-schema-for-the-calendars-element.md)

