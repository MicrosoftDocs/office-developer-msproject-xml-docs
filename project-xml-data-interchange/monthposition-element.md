---
title: MonthPosition Element
TOCTitle: MonthPosition Element
ms:assetid: a48960a9-a435-423e-9a15-1f01ed366621
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968624(v=office.12)
ms:contentKeyID: 13188315
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- MonthPosition element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# MonthPosition Element




The position of a month item within a month.

    <MonthPosition>
      IntegerValue
    </MonthPosition>

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
<td><p>0</p></td>
<td><p>First position</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>Second position</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>Third position</p></td>
</tr>
<tr class="even">
<td><p>3</p></td>
<td><p>Fourth position</p></td>
</tr>
<tr class="odd">
<td><p>4</p></td>
<td><p>Last position</p></td>
</tr>
</tbody>
</table>

## Example

In the following example, the MonthPosition element specifies that the exception named Thanksgiving occurs on the fourth Thursday of the month of November.

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

