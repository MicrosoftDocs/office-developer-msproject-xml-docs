---
title: Name Element
TOCTitle: Name Element
ms:assetid: 99549287-024d-430e-8fde-53c3af351065
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968600(v=office.12)
ms:contentKeyID: 13188291
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- Name element
dev_langs:
- xml
---

# Name Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

The name of the project, calendar, calendar exception, effective work week, resource, or task.

    <Name>
      String(512): for Project, Exception, or WorkWeek; 
      String(255): for Calendar, Resource, or Task
    </Name>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968701(v=office.12).md">Project</a>, <a href="bb968481(v=office.12).md">Calendar</a>, <a href="bb968492(v=office.12).md">Exception</a>, <a href="bb968525(v=office.12).md">WorkWeek</a>, <a href="bb968715(v=office.12).md">Resource</a>, <a href="bb968487(v=office.12).md">Task</a></p></td>
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

A text value of type string is required. The text value may not exceed 512 characters for the Project , Exception, or WorkWeek elements, or 255 characters for other parent elements.

## Example

The following example uses the Name element to indicate that the calendar exception is named New Year's Day.

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

[Project Elements and XML Structure](bb968439\(v=office.12\).md)

[XML Schema for the Project Element](bb968695\(v=office.12\).md)

[Task Elements and XML Structure](bb968475\(v=office.12\).md)

[XML Schema for the Tasks Element](bb968415\(v=office.12\).md)

[Resource Elements and XML Structure](bb968445\(v=office.12\).md)

[XML Schema for the Resources Element](bb968511\(v=office.12\).md)

[Calendar Elements and XML Structure](bb968563\(v=office.12\).md)

[XML Schema for the Calendars Element](bb968557\(v=office.12\).md)

