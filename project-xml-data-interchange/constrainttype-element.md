---
title: ConstraintType Element
TOCTitle: ConstraintType Element
ms:assetid: d8ade667-0c92-4c1e-b0d8-76f8d2411330
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968703(v=office.12)
ms:contentKeyID: 13188393
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- ConstraintType element
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# ConstraintType Element




The constraint on the start or finish date of the task.

    <ConstraintType>
      IntegerValue
    </ConstraintType>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="task-element.md">Task</a></p></td>
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
<td><p>As soon as possible</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>As late as possible</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>Must start on</p></td>
</tr>
<tr class="even">
<td><p>3</p></td>
<td><p>Must finish on</p></td>
</tr>
<tr class="odd">
<td><p>4</p></td>
<td><p>Start no earlier than</p></td>
</tr>
<tr class="even">
<td><p>5</p></td>
<td><p>Start no later than</p></td>
</tr>
<tr class="odd">
<td><p>6</p></td>
<td><p>Finish no earlier than</p></td>
</tr>
<tr class="even">
<td><p>7</p></td>
<td><p>Finish no later than</p></td>
</tr>
</tbody>
</table>

## Remarks

Requires ConstraintDate to be set in the same task, unless ConstraintType is set to 0 or 1.

## See Also

#### Concepts

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

