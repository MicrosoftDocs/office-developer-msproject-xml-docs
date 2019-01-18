---
title: Finish Element
ms.date: 03/14/2018
monikerRange: '>= project-client-2010 || project-client-odc'
localization_priority: Normal
---

# Finish Element




For a Task, Resource, or Assignment element, Finish is the date and time that a task is scheduled to be completed.

For a Baseline element, it is the scheduled finish date of the task, resource, or assignment when the baseline was saved.

For a TimephasedData element, it is the finish date of the timephased data period in the task, resource, assignment, or baseline.

::: moniker range="project-client-odc"

For Sprints, the finish date of the sprint.

::: moniker-end

    <Finish>
      DateTimeValue
    </Finish>

## Parent Elements

::: moniker range=">= project-client-2010"

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="task-element.md">Task</a>, <a href="resource-element.md">Resource</a>, <a href="assignment-element.md">Assignment</a>, <a href="baseline-element.md">Baseline</a>, <a href="timephaseddata-element.md">TimephasedData</a></p></td>
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
<td><p><a href="task-element.md">Task</a>, <a href="resource-element.md">Resource</a>, <a href="assignment-element.md">Assignment</a>, <a href="baseline-element.md">Baseline</a>, <a href="timephaseddata-element.md">TimephasedData</a>, <a href="sprint-element.md">Sprint</a></p></td>
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

## See Also

#### Concepts

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

[Assignment Elements and XML Structure](assignment-elements-and-xml-structure.md)

[XML Schema for the Resources Element](xml-schema-for-the-resources-element.md)

[Assignment Elements and XML Structure](assignment-elements-and-xml-structure.md)

[XML Schema for the Assignments Element](xml-schema-for-the-assignments-element.md)

[TimephasedDataType Elements and XML Structure](timephaseddatatype-elements-and-xml-structure.md)

[XML Schema for the TimephasedDataType Complex Type](xml-schema-for-the-timephaseddatatype-complex-type.md)

