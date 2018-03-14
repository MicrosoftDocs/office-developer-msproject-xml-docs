---
title: IsCostResource Element
TOCTitle: IsCostResource Element
ms:assetid: 74fc88e2-ebe0-45e9-8092-b3cfb7bc6e59
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968549(v=office.12)
ms:contentKeyID: 13188241
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- IsCostResource element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# IsCostResource Element




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
<td><p><a href="resource-element.md">Resource</a></p></td>
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

[Resource Elements and XML Structure](resource-elements-and-xml-structure.md)

[XML Schema for the Resources Element](xml-schema-for-the-resources-element.md)

