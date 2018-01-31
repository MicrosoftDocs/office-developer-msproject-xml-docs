---
title: AssnOwner Element
TOCTitle: AssnOwner Element
ms:assetid: 0c2e69c8-c02a-430d-8470-931b6cb07440
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968408(v=office.12)
ms:contentKeyID: 13188101
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- AssnOwner element
dev_langs:
- xml
---

# AssnOwner Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

Name of the assignment owner.

    <AssnOwner>
      StringValue
    </AssnOwner>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968611(v=office.12).md">Assignment</a>, <a href="bb968715(v=office.12).md">Resource</a></p></td>
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

A text value of type string is required.

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

[AssnOwnerGuid Element](bb968551\(v=office.12\).md)

#### Concepts

[Resource Elements and XML Structure](bb968445\(v=office.12\).md)

[XML Schema for the Resources Element](bb968511\(v=office.12\).md)

[Assignment Elements and XML Structure](bb968738\(v=office.12\).md)

[XML Schema for the Assignments Element](bb968414\(v=office.12\).md)

