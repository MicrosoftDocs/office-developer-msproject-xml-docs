---
title: Hyperlink Element
TOCTitle: Hyperlink Element
ms:assetid: f22dbcc7-ea0e-4171-8257-3d90df08e40d
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968729(v=office.12)
ms:contentKeyID: 13188419
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- Hyperlink element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# Hyperlink Element




The title or explanatory text for a hyperlink associated with a task, resource, or assignment.

    <Hyperlink>
      String(512)Value
    </Hyperlink>

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

[HyperlinkAddress Element](bb968561\(v=office.12\).md)

[HyperlinkSubAddress Element](bb968602\(v=office.12\).md)

#### Concepts

[Task Elements and XML Structure](bb968475\(v=office.12\).md)

[XML Schema for the Tasks Element](bb968415\(v=office.12\).md)

[Resource Elements and XML Structure](bb968445\(v=office.12\).md)

[XML Schema for the Resources Element](bb968511\(v=office.12\).md)

[Assignment Elements and XML Structure](bb968738\(v=office.12\).md)

[XML Schema for the Assignments Element](bb968414\(v=office.12\).md)

