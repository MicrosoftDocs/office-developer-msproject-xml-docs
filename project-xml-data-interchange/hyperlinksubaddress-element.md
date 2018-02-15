---
title: HyperlinkSubAddress Element
TOCTitle: HyperlinkSubAddress Element
ms:assetid: 99c068ea-a59e-4572-b8e7-5701736b9056
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968602(v=office.12)
ms:contentKeyID: 13188293
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- HyperlinkSubAddress element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# HyperlinkSubAddress Element




For a hyperlink associated with a task, resource, or assignment, the HyperlinkSubAddress refers to a specific location within a document.

    <HyperlinkSubAddress>
      String(512)Value
    </HyperlinkSubAddress>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="task-element.md">Task</a>, <a href="resource-element.md">Resource</a>, <a href="assignment-element.md">Assignment</a></p></td>
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

## Example

The following example shows a hyperlink for a task named T2, where the complete URL is [http://msdn2.microsoft.com/en-us/library/bb456485.aspx\#officepj2007platform\_\_documentation](http://msdn2.microsoft.com/en-us/library/bb456485.aspx).

``` xml
<Task>
    <UID>2</UID>
    <ID>2</ID>
    <Name>T2</Name>
    . . .
    <Hyperlink>Links for Project documentation</Hyperlink>
    <HyperlinkAddress>http://msdn2.microsoft.com/en-us/library/bb456485.aspx</HyperlinkAddress>
    <HyperlinkSubAddress>officepj2007platform__documentation</HyperlinkSubAddress>
. . .
</Task>
```

## See Also

#### Reference

[Hyperlink Element](hyperlink-element.md)

[HyperlinkAddress Element](hyperlinkaddress-element.md)

#### Concepts

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

[Resource Elements and XML Structure](resource-elements-and-xml-structure.md)

[XML Schema for the Resources Element](xml-schema-for-the-resources-element.md)

[Assignment Elements and XML Structure](assignment-elements-and-xml-structure.md)

[XML Schema for the Assignments Element](xml-schema-for-the-assignments-element.md)

