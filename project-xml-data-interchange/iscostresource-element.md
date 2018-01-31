---
title: IsCostResource Element
TOCTitle: IsCostResource Element
ms:assetid: 74fc88e2-ebe0-45e9-8092-b3cfb7bc6e59
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968549(v=office.12)
ms:contentKeyID: 13188241
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- IsCostResource element
dev_langs:
- xml
---

# IsCostResource Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

Indicates whether the resource is a cost resource.

    <IsCostResource>
      BooleanValue
    </IsCostResource>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968715(v=office.12).md">Resource</a></p></td>
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

Valid values are listed in Table 1.

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

The following example uses the IsCostResource element to indicate that the resource is a cost resource.

``` xml
<Resource>
  …
  <IsCostResource>1</IsCostResource>
  …
</Resource>
```

## See Also

#### Concepts

[Resource Elements and XML Structure](bb968445\(v=office.12\).md)

[XML Schema for the Resources Element](bb968511\(v=office.12\).md)

