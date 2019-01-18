---
title: DaysOfWeek Element
TOCTitle: DaysOfWeek Element
ms:assetid: 83ab0be5-93bb-41c0-bf4c-4a4fce3d2cf5
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968569(v=office.12)
ms:contentKeyID: 13188260
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- DaysOfWeek element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
localization_priority: Normal
---

# DaysOfWeek Element




Specifies the day or days of the week that an exception is valid.

    <DaysOfWeek>
      IntegerValue
    </DaysOfWeek>

## Parent Elements

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

## Text Value

A text value of type integer is required.

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
<td><p>1</p></td>
<td><p>Sunday</p></td>
</tr>
<tr class="even">
<td><p>2</p></td>
<td><p>Monday</p></td>
</tr>
<tr class="odd">
<td><p>4</p></td>
<td><p>Tuesday</p></td>
</tr>
<tr class="even">
<td><p>8</p></td>
<td><p>Wednesday</p></td>
</tr>
<tr class="odd">
<td><p>16</p></td>
<td><p>Thursday</p></td>
</tr>
<tr class="even">
<td><p>32</p></td>
<td><p>Friday</p></td>
</tr>
<tr class="odd">
<td><p>64</p></td>
<td><p>Saturday</p></td>
</tr>
</tbody>
</table>

## Remarks

To represent multiple days, add the values. For example, a value of 62 indicates that the exception occurs every weekday (2 + 4 + 8 + 16 + 32 = 62).

## Example

In the following example, the DaysOfWeek element indicates that the calendar exception occurs on Tuesdays and Thursdays (4 + 16 = 20).

``` xml
<Exception>
  <EnteredByOccurrences>0</EnteredByOccurrences>
  <TimePeriod>
    <FromDate>2007-01-01T00:00:00</FromDate>
    <ToDate>2007-12-28T23:59:00</ToDate>
  </TimePeriod>
  <Occurrences>104</Occurrences>
  <Name>Team Meeting </Name>
  <Type>6</Type>
  <Period>1</Period>
  <DaysOfWeek>20</DaysOfWeek>
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

