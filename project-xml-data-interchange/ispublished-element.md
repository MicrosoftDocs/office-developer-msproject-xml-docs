---
title: IsPublished Element
TOCTitle: IsPublished Element
ms:assetid: 54c16411-8ce2-4eda-aa3c-7558a525f690
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968507(v=office.12)
ms:contentKeyID: 13188199
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- IsPublished element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# IsPublished Element




Indicates whether the task is published.

    <IsPublished>
      BooleanValue
    </IsPublished>

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

A text value of type boolean is required.

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
<td><p>False</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>True</p></td>
</tr>
</tbody>
</table>

## Example

The following example uses the IsPublished element to indicate that the task has been published.

``` xml
<Task>
  …
  <IsPublished>1</IsPublished>
  …
</Task>
```

## See Also

#### Concepts

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

