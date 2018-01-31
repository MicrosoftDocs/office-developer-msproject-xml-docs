---
title: WeekDays Element
TOCTitle: WeekDays Element
ms:assetid: 136be91a-672e-42d7-a8f5-77f0861dbcb9
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968420(v=office.12)
ms:contentKeyID: 13188113
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- WeekDays element
dev_langs:
- xml
---

# WeekDays Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

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
<td><p><a href="bb968481(v=office.12).md">Calendar</a></p></td>
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
<td><p><a href="bb968433(v=office.12).md">WeekDay</a></p></td>
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

[Calendar Elements and XML Structure](bb968563\(v=office.12\).md)

[XML Schema for the Calendars Element](bb968557\(v=office.12\).md)

