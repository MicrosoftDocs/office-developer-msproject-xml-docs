---
title: TimephasedData Element
TOCTitle: TimephasedData Element
ms:assetid: 41c66612-a3af-499c-b9ba-c552216d5820
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968479(v=office.12)
ms:contentKeyID: 13188171
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- TimephasedData element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# TimephasedData Element




 TimephasedData is information about a task, resource, or assignment that is distrubuted over time. Timephased data can also be associated with the baseline of a task or assignment.

    <TimephasedData>
      <UID>IntegerValue</UID>
      . . .
    </TimephasedData>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="task-element.md">Task</a>, <a href="resource-element.md">Resource</a>, <a href="assignment-element.md">Assignment</a>, <a href="baseline-element.md">Baseline</a></p></td>
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
<td><p><a href="type-element-multiple-parents.md">Type</a></p></td>
<td><p>Optional</p></td>
<td><p>One of the 76 types of timephased data.</p></td>
</tr>
<tr class="even">
<td><p><a href="uid-element.md">UID</a></p></td>
<td><p>Required</p></td>
<td><p>Unique ID for the timephased data record.</p></td>
</tr>
<tr class="odd">
<td><p><a href="start-element.md">Start</a></p></td>
<td><p>Optional</p></td>
<td><p>Start date for the timephased data record.</p></td>
</tr>
<tr class="even">
<td><p><a href="finish-element.md">Finish</a></p></td>
<td><p>Optional</p></td>
<td><p>Finish date for the timephased data record.</p></td>
</tr>
<tr class="odd">
<td><p><a href="unit-element.md">Unit</a></p></td>
<td><p>Optional</p></td>
<td><p>Time unit for the timephased data record.</p></td>
</tr>
<tr class="even">
<td><p><a href="value-element.md">Value</a></p></td>
<td><p>Optional</p></td>
<td><p>Value for each unit in the timephased data record.</p></td>
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

## Example

The following example shows that the timephased data for a task is for % complete (Type = 11), the unit of time is days (Unit = 2), and the task is 50% complete. Work on the task started at 8 a.m. on 9 November, 2007, and ended at 5 p.m. on the same day.

``` xml
<Task>
   . . .
   <TimephasedData>
      <Type>11</Type>
      <UID>2</UID>
      <Start>2007-11-09T08:00:00</Start>
      <Finish>2007-11-09T17:00:00</Finish>
      <Unit>2</Unit>
      <Value>50</Value>
   </TimephasedData>
   . . .
</Task>
```

## See Also

#### Concepts

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

[Resource Elements and XML Structure](resource-elements-and-xml-structure.md)

[XML Schema for the Resources Element](xml-schema-for-the-resources-element.md)

[Assignment Elements and XML Structure](assignment-elements-and-xml-structure.md)

[XML Schema for the Assignments Element](xml-schema-for-the-assignments-element.md)

[TimephasedDataType Elements and XML Structure](timephaseddatatype-elements-and-xml-structure.md)

[XML Schema for the TimephasedDataType Complex Type](xml-schema-for-the-timephaseddatatype-complex-type.md)

