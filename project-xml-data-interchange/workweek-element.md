---
title: WorkWeek Element
TOCTitle: WorkWeek Element
ms:assetid: 608d30fc-c808-40e6-b8b4-6d7f77397d7b
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968525(v=office.12)
ms:contentKeyID: 13188217
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- WorkWeek element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# WorkWeek Element




Contains the elements that define an effective work week.

    <WorkWeek>
      ComplexTypeValue
    </WorkWeek>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968496(v=office.12).md">WorkWeeks</a></p></td>
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
<th><p>Required / Optional</p></th>
<th><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="bb968661(v=office.12).md">TimePeriod</a></p></td>
<td><p>Optional</p></td>
<td><p>Defines a contiguous set of days in a work week.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968600(v=office.12).md">Name</a></p></td>
<td><p>Optional</p></td>
<td><p>Name of the effective week</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968433(v=office.12).md">WeekDay</a></p></td>
<td><p>Optional</p></td>
<td><p>Defines days in the work week.</p></td>
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

## Remarks


> [!WARNING]
> In the releases of Project 2007 through SP1, the WorkWeek element is not closed when you save a project that has a work week with modified working times as XML. In addition, the modified WorkingTimes elements are not saved. If you try to open the XML file in Project, you get the error, "An unexpected problem occurred while opening the file. The file may be damaged." You can edit the XML file so that it is valid and opens normally. However, because Project 2007 does not correctly read the modified working times from the XML file, we recommend that you do not use Project XML files to save work week data until the errors are fixed in a later service pack.


To be able to open the XML file, you can edit the file and do the following:

  - Add the WorkWeeks name in the empty opening and closing elements for the WorkWeeks section.

  - Close all of the WeekDay elements by adding \</WeekDay\>.

  - Add the missing WorkingTimes sections with the FromTime and ToTime child elements.

## Example

The following example shows the manually edited sections in bold font and with comments. The XML file opens in Project, so you can use other data, but the working times still show the default times.

``` xml
<Calendar>
   <Calendars>
      . . .
      <WorkWeeks>       <!-- Add element name-->
         <WorkWeek>
            <TimePeriod>
               <FromDate>2007-11-26T00:00:00</FromDate>
               <ToDate>2007-11-26T23:59:00</ToDate>
            </TimePeriod>
            <Name>Training day</Name>
            <WeekDay>
               <DayType>2</DayType>
               <DayWorking>1</DayWorking>
               <WorkingTimes>   <!-- Add modified working times-->
                  <WorkingTime><FromTime>14:00:00</FromTime><ToTime>17:00:00</ToTime></WorkingTime></WorkingTimes></WeekDay>    <!-- Add closing element -->
         </WorkWeek>
      </WorkWeeks>   <!-- Add element name-->
   </Calendar>
</Calendars>
```

## See Also

#### Concepts

[Calendar Elements and XML Structure](bb968563\(v=office.12\).md)

[XML Schema for the Calendars Element](bb968557\(v=office.12\).md)

