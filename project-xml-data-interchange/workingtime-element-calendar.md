---
title: WorkingTime Element (Calendar)
TOCTitle: WorkingTime Element
ms:assetid: 8df6f9e2-701d-4ea4-87a9-8b3e6debd4b7
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968585(v=office.12)
ms:contentKeyID: 13188276
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- WorkingTime element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# WorkingTime Element (Calendar)




Defines up to five time periods for work on a working day or for a calendar exception.

    <WorkingTime>
      ComplexTypeValue
    </WorkingTime>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="workingtimes-element-calendar.md">WorkingTimes</a></p></td>
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
<th><p>Required/Optional</p></th>
<th><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="fromtime-element-calendar.md">FromTime</a></p></td>
<td><p>Optional</p></td>
<td><p>Start of the working time.</p></td>
</tr>
<tr class="even">
<td><p><a href="totime-element-calendar.md">ToTime</a></p></td>
<td><p>Optional</p></td>
<td><p>End of the working time.</p></td>
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
<td><p>Minimum: 1</p>
<p>Maximum: 5</p></td>
</tr>
</tbody>
</table>

## Remarks

There must be at least one WorkingTime specified in a WorkingTimes collection, and there may be no more than five WorkingTime elements.

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

