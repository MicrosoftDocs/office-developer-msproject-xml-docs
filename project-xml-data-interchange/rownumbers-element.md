---
title: RowNumbers Element
ms.date: 03/14/2018
monikerRange: '>= project-client-2010 || project-client-odc'
ms.localizationpriority: medium
---

# RowNumbers Element




An element representing the rows that make up either the source or sink of the datalink.

    <RowNumbers>
      ComplexTypeValue
    </RowNumbers>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="source-element.md">Source</a>, <a href="sink-element.md">Sink</a></p></td>
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
<td><p><a href="rownumber-element.md">RowNumbers</a></p></td>
<td><p>Required</p></td>
<td><p>The ID of the row.</p></td>
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
<td><p>Minimum: 0 for Source, 1 for Sink</p>
<p>Maximum: 100</p></td>
</tr>
</tbody>
</table>
