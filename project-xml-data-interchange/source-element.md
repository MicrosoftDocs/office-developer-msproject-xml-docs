---
title: Source Element
ms.date: 03/14/2018
monikerRange: '>= project-client-2010 || project-client-odc'
localization_priority: Normal
---

# Source Element


The source of the datalink. This can either be a location in the project or an external source like a reference to a cell range in Excel. 



    <Source>
      ComplexTypeValue
    </Source>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="datalink-element.md">DataLink</a></p></td>
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
<td><p><a href="columnnames-element.md">ColumnNames</a></p></td>
<td><p>Optional</p></td>
<td><p>The column names of the source.</p></td>
</tr>
<tr class="even">
<td><p><a href="rownumbers-element.md">RowNumbers</a></p></td>
<td><p>Optional</p></td>
<td><p>The row numbers of the source.</p></td>
</tr>
<tr class="odd">
<td><p><a href="externalsource-element.md">ExternalSource</a></p></td>
<td><p>Optional</p></td>
<td><p>A boolean noting if the source is external to the project.</p></td>
</tr>
<tr class="even">
<td><p><a href="externalfilename-element.md">ExternalFileName</a></p></td>
<td><p>Optional</p></td>
<td><p>The file name plus path of the file that is the source of the link.</p></td>
</tr>
<tr class="odd">
<td><p><a href="externalfilereference-element.md">ExternalFileReference</a></p></td>
<td><p>Optional</p></td>
<td><p>A string indicatang exactly what is being linked to.</p></td>
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
<td><p>Minimum: 1</p>
<p>Maximum: 1000</p></td>
</tr>
</tbody>
</table>

## Notes

Either the column name and row number will be specified as the source or the external fields.

## See Also

#### Concepts

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

[XML Schema for the Project Element](xml-schema-for-the-project-element.md)
