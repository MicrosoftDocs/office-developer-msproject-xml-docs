---
title: WeekDays Element
TOCTitle: WeekDays Element
ms:assetid: 136be91a-672e-42d7-a8f5-77f0861dbcb9
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968420(v=office.12)
ms:contentKeyID: 13188113
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- WeekDays element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# WeekDays Element




Contains the collection of WeekDay elements that define a calendar.

    <WeekDays>
      ComplexTypeValue
    </WeekDays>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="calendar-element.md">Calendar</a></p></td>
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
<td><p><a href="weekday-element.md">WeekDay</a></p></td>
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

