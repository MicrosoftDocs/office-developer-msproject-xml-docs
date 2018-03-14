---
title: EnteredByOccurrences Element
TOCTitle: EnteredByOccurrences Element
ms:assetid: 81819336-f180-44ea-a4a4-c6140398d105
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968564(v=office.12)
ms:contentKeyID: 13188255
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- EnteredByOccurrences element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# EnteredByOccurrences Element




Indicates whether the range of recurrence for the calendar exception is defined by a number of occurrences, or by a finish date.

    <EnteredByOccurrences>
      BooleanValue
    </EnteredByOccurrences>

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

A text value of type boolean is required.

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
<td><p>False. The range of recurrence for the exception is defined by a finish date.</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>True. The range of recurrence for the exception is defined by a number of occurrences.</p></td>
</tr>
</tbody>
</table>

## Example

The following example uses the EnteredByOccurrences element to indicate that this calendar exception was entered with a range of recurrence defined by a finish date.

``` xml
<Exception>
  <EnteredByOccurrences>0</EnteredByOccurrences>
  <TimePeriod>
    <FromDate>2007-01-01T00:00:00</FromDate>
    <ToDate>2007-01-01T23:59:00</ToDate>
  </TimePeriod>
  <Occurrences>1</Occurrences>
  <Name>New Year's Day</Name>
  <Type>1</Type>
  <DayWorking>0</DayWorking>
</Exception>
```

## See Also

#### Concepts

[Calendar Elements and XML Structure](calendar-elements-and-xml-structure.md)

[XML Schema for the Calendars Element](xml-schema-for-the-calendars-element.md)

