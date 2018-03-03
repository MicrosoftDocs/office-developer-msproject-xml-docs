---
title: UID Element
TOCTitle: UID Element
ms:assetid: 90074e2d-5cbf-475c-b456-5649c1b2949b
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968590(v=office.12)
ms:contentKeyID: 13188281
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- UID element
monikerRange: '>= project-client-2010 || project-client-odc'
---

# UID Element




The UID element is a unique identifier. UID specifies the data record of any of its parent elements within one project.

    <UID>
      String(16): for Project
      Integer: for all other parent elements
    </UID>

## Parent Elements

::: moniker range=">= project-client-2010"

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="project-element.md">Project</a>, <a href="calendar-element.md">Calendar</a>, <a href="resource-element.md">Resource</a>, <a href="assignment-element.md">Assignment</a>, <a href="task-element.md">Task</a>, <a href="extendedattribute-element.md">ExtendedAttribute</a>, <a href="timephaseddata-element.md">TimephasedData</a></p></td>
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
<td><p><a href="project-element.md">Project</a>, <a href="calendar-element.md">Calendar</a>, <a href="resource-element.md">Resource</a>, <a href="assignment-element.md">Assignment</a>, <a href="task-element.md">Task</a>, <a href="extendedattribute-element.md">ExtendedAttribute</a>, <a href="timephaseddata-element.md">TimephasedData</a>, <a href="boardcolumn-element.md">BoardColumn</a>, <a href="sprint-element.md">Sprint</a></p></td>
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
<td><p>Minimum: 1</p>
<p>Maximum: 1</p></td>
</tr>
</tbody>
</table>

## Remarks

The UID element is a string only for the Project element. The UID child element in Project is deprecated in Microsoft Office Project 2007.

For its other parent elements, UID is an integer. UID values are unique only within a project, not across multiple projects.

For a task, each UID is used only once within the project. If you create a task named T3 with UID = 3 and ID = 3, delete the task, and then create a new task named T3 with ID = 3, the new task UID is 4.

## See Also

#### Concepts

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

[XML Schema for the Project Element](xml-schema-for-the-project-element.md)

[Calendar Elements and XML Structure](calendar-elements-and-xml-structure.md)

[XML Schema for the Calendars Element](xml-schema-for-the-calendars-element.md)

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

[Assignment Elements and XML Structure](assignment-elements-and-xml-structure.md)

[XML Schema for the Resources Element](xml-schema-for-the-resources-element.md)

[ExtendedAttribute Elements and XML Structure](extendedattribute-elements-and-xml-structure.md)

[XML Schema for the ExtendedAttributes Element](xml-schema-for-the-extendedattributes-element.md)

[Assignment Elements and XML Structure](assignment-elements-and-xml-structure.md)

[XML Schema for the Assignments Element](xml-schema-for-the-assignments-element.md)

[TimephasedDataType Elements and XML Structure](timephaseddatatype-elements-and-xml-structure.md)

[XML Schema for the TimephasedDataType Complex Type](xml-schema-for-the-timephaseddatatype-complex-type.md)

