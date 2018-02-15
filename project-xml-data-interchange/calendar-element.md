---
title: Calendar Element
TOCTitle: Calendar Element
ms:assetid: 4232bf41-6652-4763-a885-ba0c1c520152
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968481(v=office.12)
ms:contentKeyID: 13188173
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- Calendar element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# Calendar Element




A calendar is used to define standard working and nonworking times in Microsoft Office Project. A project must have one base calendar. Tasks and resources may have their own calendars, which are based on a base calendar.

    <Calendar>
      ComplexTypeValue
    </Calendar>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="calendars-element.md">Calendars</a></p></td>
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
<td><p><a href="uid-element.md">UID</a></p></td>
<td><p>Required</p></td>
<td><p>The unique ID for the calendar.</p></td>
</tr>
<tr class="even">
<td><p><a href="name-element.md">Name</a></p></td>
<td><p>Optional</p></td>
<td><p>The name of the calendar.</p></td>
</tr>
<tr class="odd">
<td><p><a href="isbasecalendar-element.md">IsBaseCalendar</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the calendar is a base calendar.</p></td>
</tr>
<tr class="even">
<td><p><a href="basecalendaruid-element.md">BaseCalendarUID</a></p></td>
<td><p>Optional</p></td>
<td><p>The unique ID for the base calendar on which this calendar depends; only used if this calendar is not a base calendar.</p></td>
</tr>
<tr class="odd">
<td><p><a href="weekdays-element.md">WeekDays</a></p></td>
<td><p>Optional</p></td>
<td><p>The type of working day (a day of the week, or exception).</p></td>
</tr>
<tr class="even">
<td><p><a href="exceptions-element.md">Exceptions</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Collection of exceptions associated with the calendar.</p></td>
</tr>
<tr class="odd">
<td><p><a href="workweeks-element.md">WorkWeeks</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Collection of work week definitions.</p></td>
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
<p>Maximum: Unbounded</p></td>
</tr>
</tbody>
</table>

## Example

The following example shows a local calendar named Team Base Calendar. The calendar is created as a new base calendar, not as a copy of another calendar.


> [!WARNING]
> In the releases of Project 2007 through SP1, the WorkWeeks element name is missing when you save a project that has a non-default work week as XML. If you try to open the XML file in Project, you get an error, "An unexpected problem occurred while opening the file. The file may be damaged." The workaround is to edit the XML file and add the WorkWeeks element name, as in the following example. The XML file then opens normally. However, because the WorkWeek element contains other errors, we recommend that you do not use Project XML files to save work week data until the errors are fixed in a later service pack. For more information about editing other elements for work weeks, see the <A href="workweek-element.md">WorkWeek Element</A>.


``` xml
<Calendar>
   <UID>5</UID>
   <Name>Team Base Calendar</Name>
   <IsBaseCalendar>1</IsBaseCalendar>
   <BaseCalendarUID>-1</BaseCalendarUID>
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
      . . .
   </WeekDays>
   <Exceptions>
      <Exception>
         <EnteredByOccurrences>0</EnteredByOccurrences>
         <TimePeriod>
            <FromDate>2007-11-22T00:00:00</FromDate>
            <ToDate>2007-11-23T23:59:00</ToDate>
         </TimePeriod>
         <Occurrences>2</Occurrences>
         <Name>Thanksgiving holidays</Name>
         <Type>1</Type>
         <DayWorking>0</DayWorking>
      </Exception>
   </Exceptions>
   <WorkWeeks>
      <WorkWeek>
         <TimePeriod>
            <FromDate>2007-11-26T00:00:00</FromDate>
            <ToDate>2007-11-26T23:59:00</ToDate>
         </TimePeriod>
         <Name>Post-holiday working days</Name>
      </WorkWeek>
   </WorkWeeks>
</Calendar>
```

## See Also

#### Concepts

[Calendar Elements and XML Structure](calendar-elements-and-xml-structure.md)

[XML Schema for the Calendars Element](xml-schema-for-the-calendars-element.md)

