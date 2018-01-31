---
title: RollupType Element
TOCTitle: RollupType Element
ms:assetid: 422ed965-01fe-45ec-8b7e-0a606b174c66
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968480(v=office.12)
ms:contentKeyID: 13188172
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- RollupType element
---

# RollupType Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

Indicates the method used to calculate custom field rollup values for summary tasks.

    <RollupType>
      IntegerValue
    </RollupType>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968669(v=office.12).md">ExtendedAttribute</a></p></td>
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

Required Integer

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
<td><p>Maximum (OR for flag fields)</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>Minimum (AND for flag fields)</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>Count all</p></td>
</tr>
<tr class="even">
<td><p>3</p></td>
<td><p>Sum</p></td>
</tr>
<tr class="odd">
<td><p>4</p></td>
<td><p>Average</p></td>
</tr>
<tr class="even">
<td><p>5</p></td>
<td><p>Average, first sub-level</p></td>
</tr>
<tr class="odd">
<td><p>6</p></td>
<td><p>Count, first sub-level</p></td>
</tr>
<tr class="even">
<td><p>7</p></td>
<td><p>Count, non-summaries</p></td>
</tr>
</tbody>
</table>

## See Also

#### Concepts

[ExtendedAttribute Elements and XML Structure](bb968579\(v=office.12\).md)

[XML Schema for the ExtendedAttributes Element](bb968705\(v=office.12\).md)

