---
title: FieldValueGUID Element
ms.date: 03/08/2018
monikerRange: '>= project-client-2010 || project-client-odc'
---

# FieldValueGUID Element




Globally unique identifier (GUID) of an Enterprise Custom Field lookup table value.

    <FieldValueGUID>
      StringValue(255)
    </FieldValueGUID>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="enterpriseextendedattribute-element.md">EnterpriseExtendedAttribute</a></p></td>
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
<p>Maximum: 1</p></td>
</tr>
</tbody>
</table>

## Text Value

A text value of type string is required. The string must be in the form "HHHHHHHH-HHHH-HHHH-HHHH-HHHHHHHHHHHH" where "H" represents a hexadecimal digit between 0 and F.

