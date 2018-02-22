---
title: BoardColumn Element
ms.date: 02/21/2018
monikerRange: 'project-client-odc'
---

# BoardColumn Element


A board status value that is a part of the BoardColumns element. This value can be selected for a task through the Board Status field.



    <BoardColumn>
      ComplexTypeValue
    </BoardColumn>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="boardcolumns-element.md">BoardColumns</a></p></td>
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
<td><p>The unique ID for the board column.</p></td>
</tr>
<tr class="even">
<td><p><a href="id-element.md">ID</a></p></td>
<td><p>Required</p></td>
<td><p>The ID for the board column.</p></td>
</tr>
<tr class="odd">
<td><p><a href="guid-element.md">GUID</a></p></td>
<td><p>Required</p></td>
<td><p>The GUID for the board column.</p></td>
</tr>
<tr class="even">
<td><p><a href="name-element.md">Name</a></p></td>
<td><p>Optional</p></td>
<td><p>The name of the board column.</p></td>
</tr>
<tr class="odd">
<td><p><a href="description-element.md">Description</a></p></td>
<td><p>Optional</p></td>
<td><p>The description of the board column.</p></td>
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

