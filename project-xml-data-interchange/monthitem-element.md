---
title: MonthItem Element
TOCTitle: MonthItem Element
ms:assetid: 7fb52838-fb36-49d2-b078-556ae4d97021
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968560(v=office.12)
ms:contentKeyID: 13188251
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- MonthItem element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
localization_priority: Normal
---

# MonthItem Element




The month item for which an exception recurrence is scheduled.

    <MonthItem>
      IntegerValue
    </MonthItem>

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

Valid values are listed in Table 1.

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
<td><p>Day</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>Weekday</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>Weekend day</p></td>
</tr>
<tr class="even">
<td><p>3</p></td>
<td><p>Sunday</p></td>
</tr>
<tr class="odd">
<td><p>4</p></td>
<td><p>Monday</p></td>
</tr>
<tr class="even">
<td><p>5</p></td>
<td><p>Tuesday</p></td>
</tr>
<tr class="odd">
<td><p>6</p></td>
<td><p>Wednesday</p></td>
</tr>
<tr class="even">
<td><p>7</p></td>
<td><p>Thursday</p></td>
</tr>
<tr class="odd">
<td><p>8</p></td>
<td><p>Friday</p></td>
</tr>
<tr class="even">
<td><p>9</p></td>
<td><p>Saturday</p></td>
</tr>
</tbody>
</table>

## Example

In the following example, the MonthItem element indicates that the calendar exception named Thanksgiving occurs on a Thursday.

``` xml
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
```

## See Also

#### Concepts

[Calendar Elements and XML Structure](calendar-elements-and-xml-structure.md)

[XML Schema for the Calendars Element](xml-schema-for-the-calendars-element.md)

