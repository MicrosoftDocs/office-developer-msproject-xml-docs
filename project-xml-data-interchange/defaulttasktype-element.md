---
title: DefaultTaskType Element
TOCTitle: DefaultTaskType Element
ms:assetid: 9a0cae2a-2c23-4351-b8a9-7b3c22a1f60c
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968603(v=office.12)
ms:contentKeyID: 13188294
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- DefaultTaskType element
monikerRange: '>= project-client-2007 || project-client-odc'
localization_priority: Normal
---

# DefaultTaskType Element




The default type of new tasks.

    <DefaultTaskType>
      IntegerValue
    </DefaultTaskType>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="project-element.md">Project</a></p></td>
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

## Text Value

A text value of type integer is required.

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Value</p></th>
<th><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>0</p></td>
<td><p>Fixed units (default); the number of resources (assignment units) remains constant, regardless of the amount of work or duration on the task</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>Fixed duration; the duration of the task remains constant, regardless of the number of resources (assignment units) assigned or the amount of work</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>Fixed work; the amount of work remains constant, regardless of any change in duration or the number of resources (assignment units) assigned to the task</p></td>
</tr>
</tbody>
</table>

## See Also

#### Concepts

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

[XML Schema for the Project Element](xml-schema-for-the-project-element.md)

