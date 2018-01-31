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
---

# TimephasedData Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

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
<td><p><a href="bb968487(v=office.12).md">Task</a>, <a href="bb968715(v=office.12).md">Resource</a>, <a href="bb968611(v=office.12).md">Assignment</a>, <a href="bb968599(v=office.12).md">Baseline</a></p></td>
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
<td><p><a href="bb968434(v=office.12).md">Type</a></p></td>
<td><p>Optional</p></td>
<td><p>One of the 76 types of timephased data.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968590(v=office.12).md">UID</a></p></td>
<td><p>Required</p></td>
<td><p>Unique ID for the timephased data record.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968645(v=office.12).md">Start</a></p></td>
<td><p>Optional</p></td>
<td><p>Start date for the timephased data record.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968534(v=office.12).md">Finish</a></p></td>
<td><p>Optional</p></td>
<td><p>Finish date for the timephased data record.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968545(v=office.12).md">Unit</a></p></td>
<td><p>Optional</p></td>
<td><p>Time unit for the timephased data record.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968696(v=office.12).md">Value</a></p></td>
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

[Task Elements and XML Structure](bb968475\(v=office.12\).md)

[XML Schema for the Tasks Element](bb968415\(v=office.12\).md)

[Resource Elements and XML Structure](bb968445\(v=office.12\).md)

[XML Schema for the Resources Element](bb968511\(v=office.12\).md)

[Assignment Elements and XML Structure](bb968738\(v=office.12\).md)

[XML Schema for the Assignments Element](bb968414\(v=office.12\).md)

[TimephasedDataType Elements and XML Structure](bb968722\(v=office.12\).md)

[XML Schema for the TimephasedDataType Complex Type](bb968734\(v=office.12\).md)

