---
title: Unit Element
TOCTitle: Unit Element
ms:assetid: 72cd21bf-0ee5-4fb8-bc97-b4ab8f88cece
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968545(v=office.12)
ms:contentKeyID: 13188237
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- Unit element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# Unit Element




Time unit for the timephased data period.

    <Unit>
      IntegerValue
    </Unit>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="timephaseddata-element.md">TimephasedData</a></p></td>
</tr>
</tbody>
</table>

### Element Properties

The Unit element has an integer value that represents one of the following time units.

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p><strong>Value</strong></p></th>
<th><p><strong>Description</strong></p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>0</p></td>
<td><p>Minutes</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>Hours</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>Days</p></td>
</tr>
<tr class="even">
<td><p>3</p></td>
<td><p>Weeks</p></td>
</tr>
<tr class="odd">
<td><p>5</p></td>
<td><p>Months</p></td>
</tr>
<tr class="even">
<td><p>8</p></td>
<td><p>Years</p></td>
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

## See Also

#### Concepts

[TimephasedDataType Elements and XML Structure](timephaseddatatype-elements-and-xml-structure.md)

[XML Schema for the TimephasedDataType Complex Type](xml-schema-for-the-timephaseddatatype-complex-type.md)

