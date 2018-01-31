---
title: Month Element
TOCTitle: Month Element
ms:assetid: 2d77e623-efaa-4695-a08f-1b64e8525292
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968450(v=office.12)
ms:contentKeyID: 13188142
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- Month element
dev_langs:
- xml
---

# Month Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

The month for which an exception recurrence is scheduled.

    <Month>
      IntegerValue
    </Month>

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
<td><p>0</p></td>
<td><p>January</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>February</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>March</p></td>
</tr>
<tr class="even">
<td><p>3</p></td>
<td><p>April</p></td>
</tr>
<tr class="odd">
<td><p>4</p></td>
<td><p>May</p></td>
</tr>
<tr class="even">
<td><p>5</p></td>
<td><p>June</p></td>
</tr>
<tr class="odd">
<td><p>6</p></td>
<td><p>July</p></td>
</tr>
<tr class="even">
<td><p>7</p></td>
<td><p>August</p></td>
</tr>
<tr class="odd">
<td><p>8</p></td>
<td><p>September</p></td>
</tr>
<tr class="even">
<td><p>9</p></td>
<td><p>October</p></td>
</tr>
<tr class="odd">
<td><p>10</p></td>
<td><p>November</p></td>
</tr>
<tr class="even">
<td><p>11</p></td>
<td><p>December</p></td>
</tr>
</tbody>
</table>

## Example

The following example uses the Month element to indicate that the calendar exception named New Year's Day occurs in January.

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

