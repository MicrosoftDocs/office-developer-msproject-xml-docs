---
title: Duration Element
ms.date: 03/14/2018
monikerRange: '>= project-client-2010 || project-client-odc'
ms.localizationpriority: medium
---

# Duration Element


For a Task , Duration is the total span of active working time.

For a task's Baseline , it is the scheduled duration of the task when the baseline was saved.

::: moniker range="project-client-odc"

For Sprints, the duration value of the sprint.

::: moniker-end

    <Duration>
      TimeSpanValue
    </Duration>

## Parent Elements

::: moniker range=">= project-client-2010"

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="baseline-element.md">Baseline</a>, <a href="task-element.md">Task</a></p></td>
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
<td><p><a href="baseline-element.md">Baseline</a>, <a href="task-element.md">Task</a>, <a href="sprint-element.md">Sprint</a></p></td>
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

