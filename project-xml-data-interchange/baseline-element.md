---
title: Baseline Element
TOCTitle: Baseline Element
ms:assetid: 985cf3e5-7378-41a9-b1d8-ebf03c1584aa
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968599(v=office.12)
ms:contentKeyID: 13188290
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- Baseline element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# Baseline Element




The collection of baseline values associated with the task, resource or assignment.

    <Baseline>
      ComplexTypeValue
    </Baseline>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968487(v=office.12).md">Task</a>, <a href="bb968715(v=office.12).md">Resource</a>, <a href="bb968611(v=office.12).md">Assignment</a></p></td>
</tr>
</tbody>
</table>

## Child Elements for a Task

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
<td><p><a href="bb968479(v=office.12).md">TimephasedData</a></p></td>
<td><p>Optional</p></td>
<td><p>The timephased data block associated with the task baseline.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968680(v=office.12).md">Number</a></p></td>
<td><p>Required</p></td>
<td><p>The unique number of the baseline data record.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968438(v=office.12).md">Interim</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the baseline is an interim baseline.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968645(v=office.12).md">Start</a></p></td>
<td><p>Optional</p></td>
<td><p>The scheduled start date of the task when the baseline was saved.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968534(v=office.12).md">Finish</a></p></td>
<td><p>Optional</p></td>
<td><p>The scheduled finish date of the task when the baseline was saved.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968640(v=office.12).md">Duration</a></p></td>
<td><p>Optional</p></td>
<td><p>The scheduled duration of the task when the baseline was saved.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968637(v=office.12).md">DurationFormat</a></p></td>
<td><p>Optional</p></td>
<td><p>The format for expressing the duration of the task baseline.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968697(v=office.12).md">EstimatedDuration</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the duration of the task is estimated.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968571(v=office.12).md">Work</a></p></td>
<td><p>Optional</p></td>
<td><p>The scheduled work for the task when the baseline was saved.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968522(v=office.12).md">Cost</a></p></td>
<td><p>Optional</p></td>
<td><p>The projected cost of the task when the baseline was saved.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968411(v=office.12).md">BCWS</a></p></td>
<td><p>Optional</p></td>
<td><p>BCWS is the budgeted cost of work scheduled. The cumulative timephased baseline costs up to the status date or today's date.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968714(v=office.12).md">BCWP</a></p></td>
<td><p>Optional</p></td>
<td><p>BCWP is the budgeted cost of work performed. The cumulative value of the task's timephased percent complete multiplied by the task's timephased baseline cost, up to the status date or today's date.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968494(v=office.12).md">FixedCost</a></p></td>
<td><p>Optional</p></td>
<td><p>New for Baseline in Project 2007. The fixed cost of the task when the baseline was saved.</p></td>
</tr>
</tbody>
</table>

## Child Elements for a Resource

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
<td><p><a href="bb968680(v=office.12).md">Number</a></p></td>
<td><p>Required</p></td>
<td><p>The unique number of the baseline data record.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968571(v=office.12).md">Work</a></p></td>
<td><p>Optional</p></td>
<td><p>The work assigned to the resource when the baseline is saved.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968522(v=office.12).md">Cost</a></p></td>
<td><p>Optional</p></td>
<td><p>The projected cost for the resource when the baseline was saved.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968411(v=office.12).md">BCWS</a></p></td>
<td><p>Optional</p></td>
<td><p>The budgeted cost of work scheduled for the resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968714(v=office.12).md">BCWP</a></p></td>
<td><p>Optional</p></td>
<td><p>The budgeted cost of the work performed by the resource on the project to-date.</p></td>
</tr>
</tbody>
</table>

## Child Elements for an Assignment

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
<td><p><a href="bb968479(v=office.12).md">TimephasedData</a></p></td>
<td><p>Optional</p></td>
<td><p>The timephased data block associated with the task baseline.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968680(v=office.12).md">Number</a></p></td>
<td><p>Required</p></td>
<td><p>The unique number of the baseline data record.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968645(v=office.12).md">Start</a></p></td>
<td><p>Optional</p></td>
<td><p>The scheduled start date of the assignment when the baseline was saved.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968534(v=office.12).md">Finish</a></p></td>
<td><p>Optional</p></td>
<td><p>The scheduled finish date of the assignment when the baseline was saved.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968571(v=office.12).md">Work</a></p></td>
<td><p>Optional</p></td>
<td><p>The total amount of work scheduled on the assignment when the baseline was saved.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968522(v=office.12).md">Cost</a></p></td>
<td><p>Optional</p></td>
<td><p>The total projected cost of the assignment when the baseline was saved.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968411(v=office.12).md">BCWS</a></p></td>
<td><p>Optional</p></td>
<td><p>The budgeted cost of work scheduled on the assignment.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968714(v=office.12).md">BCWP</a></p></td>
<td><p>Optional</p></td>
<td><p>The budgeted cost of the work performed on the assignment to date.</p></td>
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

## See Also

#### Concepts

[Task Elements and XML Structure](bb968475\(v=office.12\).md)

[XML Schema for the Tasks Element](bb968415\(v=office.12\).md)

[Resource Elements and XML Structure](bb968445\(v=office.12\).md)

[XML Schema for the Resources Element](bb968511\(v=office.12\).md)

[Assignment Elements and XML Structure](bb968738\(v=office.12\).md)

[XML Schema for the Assignments Element](bb968414\(v=office.12\).md)

