---
title: WorkWeeks Element
TOCTitle: WorkWeeks Element
ms:assetid: 4be76fb8-eb91-4f77-8447-4e2153e0e3d9
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968496(v=office.12)
ms:contentKeyID: 13188188
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- WorkWeeks element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# WorkWeeks Element




Contains a collection of work week defintions.

    <WorkWeeks>
    </WorkWeeks>

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

## Child Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="workweek-element.md">WorkWeek</a></p></td>
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

For an example that uses the WorkWeeks element, see [Calendar Element](calendar-element.md)


> [!WARNING]
> In the releases of Project 2007 through SP1, the WorkWeeks element name is missing when you save a project that has a non-default work week as XML. If you try to open the XML file in Project, you get the error, "An unexpected problem occurred while opening the file. The file may be damaged." The workaround is to edit the XML file and add the WorkWeeks element name, as in the following example. The XML file then opens normally. However, because the WorkWeek element contains other errors, we recommend that you do not use Project XML files to save work week data until the errors are fixed in a later service pack. For more information about editing other elements for work weeks, see the <A href="workweek-element.md">WorkWeek Element</A>.


## Example

The following example defines a non-standard work week named Test work week. The WorkWeeks opening and closing element is manually edited.

``` xml
<Calendar>
   . . .
   <WorkWeeks>
      <WorkWeek>
         <TimePeriod>
            <FromDate>2007-11-26T00:00:00</FromDate>
            <ToDate>2007-11-26T23:59:00</ToDate>
         </TimePeriod>
         <Name>Test work week</Name>
      </WorkWeek>
   </WorkWeeks>
</Calendar>
```

## See Also

#### Concepts

[Calendar Elements and XML Structure](calendar-elements-and-xml-structure.md)

[XML Schema for the Calendars Element](xml-schema-for-the-calendars-element.md)

