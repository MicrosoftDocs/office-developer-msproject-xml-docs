---
title: AssnOwnerGuid Element
TOCTitle: AssnOwnerGuid Element
ms:assetid: 782ab95f-9790-4d61-9227-111841305578
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968551(v=office.12)
ms:contentKeyID: 13188243
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- AssnOwnerGuid element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# AssnOwnerGuid Element




The GUID of the assignment owner.

    <AssnOwnerGuid>
      StringValue
    </AssnOwnerGuid>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="assignment-element.md">Assignment</a>, <a href="resource-element.md">Resource</a></p></td>
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

A text value of type string is required. The string must be in the form "HHHHHHHH-HHHH-HHHH-HHHH-HHHHHHHHHHHH" where "H" represents a hexadecimal digit between 0 and F.

## Example

The following example uses the AssnOwner element and the AssnOwnerGuid element to specify that the assignment owner is Ioannis Xylaras.

``` xml
<Assignment>
  …
  <AssnOwner>Ioannis Xylaras</AssnOwner>
  <AssnOwnerGuid>479C3510-B506-4CE9-BA9A-60C585111E18</AssnOwnerGuid>
  …
</Assignment>
```

## See Also

#### Reference

[AssnOwner Element](assnowner-element.md)

#### Concepts

[Resource Elements and XML Structure](resource-elements-and-xml-structure.md)

[XML Schema for the Resources Element](xml-schema-for-the-resources-element.md)

[Assignment Elements and XML Structure](assignment-elements-and-xml-structure.md)

[XML Schema for the Assignments Element](xml-schema-for-the-assignments-element.md)

