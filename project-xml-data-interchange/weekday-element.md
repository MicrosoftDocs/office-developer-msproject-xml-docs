---
title: WeekDay Element
TOCTitle: WeekDay Element
ms:assetid: 20e6a844-282c-4007-b7e6-414d2d402ac1
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968433(v=office.12)
ms:contentKeyID: 13188126
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- WeekDay element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# WeekDay Element




A weekday defines either days of the week or exception days in a calendar.

    <WeekDay>
      ComplexTypeValue
    </WeekDay>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="weekdays-element.md">WeekDays</a></p></td>
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
<td><p><a href="daytype-element.md">DayType</a></p></td>
<td><p>Required</p></td>
<td><p>Type of working day (exception, or Monday - Sunday)</p></td>
</tr>
<tr class="even">
<td><p><a href="dayworking-element-calendar.md">DayWorking</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the specified date or date type is a working day.</p></td>
</tr>
<tr class="odd">
<td><p><a href="timeperiod-element-calendar.md">TimePeriod</a></p></td>
<td><p>Optional</p></td>
<td><p>Defines a set of exception days.</p></td>
</tr>
<tr class="even">
<td><p><a href="workingtimes-element-calendar.md">WorkingTimes</a></p></td>
<td><p>Optional</p></td>
<td><p>Collection of working times that define the time worked.</p></td>
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

In the following example, Saturday (DayType = 7) and Sunday (DayType = 1) are nonworking days.

``` xml
<WeekDays>
   <WeekDay>
      <DayType>1</DayType>
      <DayWorking>0</DayWorking>
   </WeekDay>
   <WeekDay>
      <DayType>2</DayType>
      <DayWorking>1</DayWorking>
      <WorkingTimes>
         <WorkingTime>
            <FromTime>08:00:00</FromTime>
            <ToTime>12:00:00</ToTime>
         </WorkingTime>
         <WorkingTime>
            <FromTime>13:00:00</FromTime>
            <ToTime>17:00:00</ToTime>
         </WorkingTime>
      </WorkingTimes>
   </WeekDay>
   <WeekDay>
      <DayType>3</DayType>
      <DayWorking>1</DayWorking>
      <WorkingTimes>
         <WorkingTime>
            <FromTime>08:00:00</FromTime>
            <ToTime>12:00:00</ToTime>
         </WorkingTime>
         <WorkingTime>
            <FromTime>13:00:00</FromTime>
            <ToTime>17:00:00</ToTime>
         </WorkingTime>
      </WorkingTimes>
   </WeekDay>
   <WeekDay>
      <DayType>4</DayType>
      <DayWorking>1</DayWorking>
      <WorkingTimes>
         <WorkingTime>
            <FromTime>08:00:00</FromTime>
            <ToTime>12:00:00</ToTime>
         </WorkingTime>
         <WorkingTime>
            <FromTime>13:00:00</FromTime>
            <ToTime>17:00:00</ToTime>
         </WorkingTime>
      </WorkingTimes>
   </WeekDay>
   <WeekDay>
      <DayType>5</DayType>
      <DayWorking>1</DayWorking>
      <WorkingTimes>
         <WorkingTime>
            <FromTime>08:00:00</FromTime>
            <ToTime>12:00:00</ToTime>
         </WorkingTime>
         <WorkingTime>
            <FromTime>13:00:00</FromTime>
            <ToTime>17:00:00</ToTime>
         </WorkingTime>
      </WorkingTimes>
   </WeekDay>
   <WeekDay>
      <DayType>6</DayType>
      <DayWorking>1</DayWorking>
      <WorkingTimes>
         <WorkingTime>
            <FromTime>08:00:00</FromTime>
            <ToTime>12:00:00</ToTime>
         </WorkingTime>
         <WorkingTime>
            <FromTime>13:00:00</FromTime>
            <ToTime>17:00:00</ToTime>
         </WorkingTime>
      </WorkingTimes>
   </WeekDay>
   <WeekDay>
      <DayType>7</DayType>
      <DayWorking>0</DayWorking>
   </WeekDay>
</WeekDays>
```

## See Also

#### Concepts

[Calendar Elements and XML Structure](calendar-elements-and-xml-structure.md)

[XML Schema for the Calendars Element](xml-schema-for-the-calendars-element.md)

