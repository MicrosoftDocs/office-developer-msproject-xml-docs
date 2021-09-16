---
title: ID Element
TOCTitle: ID Element
ms:assetid: 23238b96-8f66-4da0-982e-2debeebf7c4f
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968437(v=office.12)
ms:contentKeyID: 13188130
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- ID element
monikerRange: '>= project-client-2010 || project-client-odc'
ms.localizationpriority: medium
---

# ID Element

For Value, it is the ID of the value within the project.

For everything else, it is the position identifier of the item within of list of items of the same kind. For example, for resources it is the position identifier within the list of resources.


    <ID>
      IntegerValue
    </ID>

## Parent Elements

::: moniker range=">= project-client-2010"

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="resource-element.md">Resource</a>, <a href="task-element.md">Task</a>, <a href="value-element.md">Value</a></p></td>
</tr>
</tbody>
</table>

::: moniker-end

::: moniker range="project-client-odc"

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="resource-element.md">Resource</a>, <a href="task-element.md">Task</a>, <a href="value-element.md">Value</a>, <a href="boardcolumn-element.md">BoardColumn</a>, <a href="sprint-element.md">Sprint</a></p></td>
</tr>
</tbody>
</table>

::: moniker-end

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

ID is not globally unique across multiple projects.

## See Also

#### Concepts

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

[Resource Elements and XML Structure](resource-elements-and-xml-structure.md)

[XML Schema for the Resources Element](xml-schema-for-the-resources-element.md)

[ExtendedAttribute Elements and XML Structure](extendedattribute-elements-and-xml-structure.md)

[XML Schema for the ExtendedAttributes Element](xml-schema-for-the-extendedattributes-element.md)

[TimephasedDataType Elements and XML Structure](timephaseddatatype-elements-and-xml-structure.md)

[XML Schema for the TimephasedDataType Complex Type](xml-schema-for-the-timephaseddatatype-complex-type.md)

