---
title: WorkingTimes Element (Calendar)
TOCTitle: WorkingTimes Element
ms:assetid: 09d7e8d2-2573-4fed-9cc9-235bf1e1a3a2
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968403(v=office.12)
ms:contentKeyID: 13188096
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- WorkingTimes element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# WorkingTimes Element (Calendar)




The collection of working times that defines the time for work on a working day or a calendar exception.

    <WorkingTimes>
      ComplexTypeValue
    </WorkingTimes>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="weekday-element.md">WeekDay</a></p></td>
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
<td><p><a href="workingtime-element-calendar.md">WorkingTime</a></p></td>
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

## Remarks

A WorkingTimes collection must contain at least one WorkingTime element, and can contain up to five WorkingTime elements.

## Example

The following example specifies two WorkingTime periods in a day.

``` xml
<WorkingTimes>
   <WorkingTime>
      <FromTime>09:00:00</FromTime>
      <ToTime>12:00:00</ToTime>
   </WorkingTime>
   <WorkingTime>
      <FromTime>13:00:00</FromTime>
      <ToTime>17:00:00</ToTime>
   </WorkingTime>
</WorkingTimes>
```

## See Also

#### Concepts

[Calendar Elements and XML Structure](calendar-elements-and-xml-structure.md)

[XML Schema for the Calendars Element](xml-schema-for-the-calendars-element.md)

