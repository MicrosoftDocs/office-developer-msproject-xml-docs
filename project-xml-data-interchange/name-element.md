---
title: Name Element
ms.date: 03/14/2018
monikerRange: '>= project-client-2010 || project-client-odc'
ms.localizationpriority: medium
---

# Name Element

::: moniker range=">= project-client-2010"


The name of the project, calendar, calendar exception, effective work week, resource, task, view, filter, group, map, table, drawing, report, or VBA project. The field is not loadable for views, filters, groups, maps, tables, drawings, reports or VBA projects.

    <Name>
      String(512): for Project, Exception, or WorkWeek; 
      String(255): for Calendar, Resource, Task, View, Filter, Group, Map, Table, Drawing, Report, or VBA project
    </Name>
    
::: moniker-end

::: moniker range="project-client-odc"


The name of the project, calendar, calendar exception, effective work week, resource, task, view, filter, group, map, table, drawing, report, VBA project, board column, or sprint. The field is not loadable for views, filters, groups, maps, tables, drawings, reports or VBA projects.

    <Name>
      String(512): for Project, Exception, or WorkWeek; 
      String(255): for Calendar, Resource, Task, View, Filter, Group, Map, Table, Drawing, Report, VBA project, Board Column, or Sprint
    </Name>
    
::: moniker-end

## Parent Elements


::: moniker range=">= project-client-2010"

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="project-element.md">Project</a>, <a href="calendar-element.md">Calendar</a>, <a href="exception-element.md">Exception</a>, <a href="workweek-element.md">WorkWeek</a>, <a href="resource-element.md">Resource</a>, <a href="task-element.md">Task</a>, <a href="view-element.md">View</a>, <a href="filter-element.md">Filter</a>, <a href="group-element.md">Group</a>,  <a href="map-element.md">Map</a>, <a href="table-element.md">Table</a>, <a href="drawing-element.md">Drawing</a>, <a href="report-element.md">Report</a>, <a href="vbaproject-element.md">VBA Project</a></p></td>
</tr>
</tbody>
</table>

::: moniker-end

::: moniker range="project-client-odc"

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="project-element.md">Project</a>, <a href="calendar-element.md">Calendar</a>, <a href="exception-element.md">Exception</a>, <a href="workweek-element.md">WorkWeek</a>, <a href="resource-element.md">Resource</a>, <a href="task-element.md">Task</a>, <a href="view-element.md">View</a>, <a href="filter-element.md">Filter</a>, <a href="group-element.md">Group</a>,  <a href="map-element.md">Map</a>, <a href="table-element.md">Table</a>, <a href="drawing-element.md">Drawing</a>, <a href="report-element.md">Report</a>, <a href="vbaproject-element.md">VBA Project</a>, <a href="boardcolumn-element.md">Board Column</a>, <a href="sprint-element.md">Sprint</a></p></td>
</tr>
</tbody>
</table>

::: moniker-end



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

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

[XML Schema for the Project Element](xml-schema-for-the-project-element.md)

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

[Resource Elements and XML Structure](resource-elements-and-xml-structure.md)

[XML Schema for the Resources Element](xml-schema-for-the-resources-element.md)

[Calendar Elements and XML Structure](calendar-elements-and-xml-structure.md)

[XML Schema for the Calendars Element](xml-schema-for-the-calendars-element.md)

