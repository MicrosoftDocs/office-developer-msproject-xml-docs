---
title: StatusManager Element
TOCTitle: StatusManager Element
ms:assetid: a87e6390-ab36-4041-baa1-939bc6b448f7
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968633(v=office.12)
ms:contentKeyID: 13188324
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- StatusManager element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# StatusManager Element




The name of the task status manager.

    <StatusManager>
      StringValue
    </StatusManager>

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

A text value of type string is required.

## Remarks

The status manager for a task can be a different person than the project manager. The status manager takes ownership of task assignments, and receives all status updates for those assignments.

## Example

The following example uses the StatusManager element to indicate that Ioannis Xylaras is the status manager for the task.

``` xml
<Task>
  . . .
  <StatusManager>Ioannis Xylaras</StatusManager>
  . . .
</Task>
```

## See Also

#### Concepts

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

