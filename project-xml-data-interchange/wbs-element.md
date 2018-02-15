---
title: WBS Element
TOCTitle: WBS Element
ms:assetid: 82e4cde0-01e5-4a2a-93e1-aa5de8c701cb
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968566(v=office.12)
ms:contentKeyID: 13188257
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- WBS element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# WBS Element




A unique code (work breakdown structure) that represents a task's position within the hierarchical structure of the project.

    <WBS>
      StringValue
    </WBS>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968487(v=office.12).md">Task</a></p></td>
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

## Remarks

By default, the WBS code is the task's outline number (1, 2, …, n for top-level tasks; 1.1, 1.2, …, 1.n for subtasks under task 1; and so forth). To define WBS codes, click **WBS** in the **Project** menu of Microsoft Office Project. For more information, see [WBS fields](http://office.microsoft.com/en-us/project/hp010259301033.aspx).

## See Also

#### Reference

[WBSLevel Element](wbslevel-element.md)

#### Concepts

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

