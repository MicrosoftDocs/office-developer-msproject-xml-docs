---
title: Occurrences Element
TOCTitle: Occurrences Element
ms:assetid: e04aaef6-8207-47a9-8711-a66e628ad2ae
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968710(v=office.12)
ms:contentKeyID: 13188400
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- Occurrences element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
localization_priority: Normal
---

# Occurrences Element




The number of occurrences for which the calendar exception is valid.

    <Occurrences>
      IntegerValue
    </Occurrences>

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

## Example

In the following example, the Occurrences element indicates that the calendar exception occurs only once.

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

