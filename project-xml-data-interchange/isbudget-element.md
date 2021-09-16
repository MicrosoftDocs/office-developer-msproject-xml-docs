---
title: IsBudget Element
TOCTitle: IsBudget Element
ms:assetid: 9e3cbbb0-2df5-4c26-aa62-335daf8a238d
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968612(v=office.12)
ms:contentKeyID: 13188303
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- IsBudget element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# IsBudget Element




Indicates whether the resource is a budget resource.

    <IsBudget>
      BooleanValue
    </IsBudget>

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

A string value of type boolean is required.

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

The following example uses the IsBudget element to indicate that the resource is not a budget resource.

``` xml
<Resource>
  …
  <IsBudget>0</IsBudget>
  …
</Resource>
```

## See Also

#### Concepts

[Resource Elements and XML Structure](resource-elements-and-xml-structure.md)

[XML Schema for the Resources Element](xml-schema-for-the-resources-element.md)

