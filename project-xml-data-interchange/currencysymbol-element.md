---
title: CurrencySymbol Element
TOCTitle: CurrencySymbol Element
ms:assetid: 52326940-06b2-401e-998c-71ca77c944a3
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968502(v=office.12)
ms:contentKeyID: 13188194
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- CurrencySymbol element
monikerRange: '>= project-client-2007 || project-client-odc'
localization_priority: Normal
---

# CurrencySymbol Element




The currency symbol used to represent the type of currency used in the project.

    <CurrencySymbol>
      String(20)Value
    </CurrencySymbol>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="project-element.md">Project</a></p></td>
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

## Remarks

The default CurrencySymbol value for new projects is determined by the enterprise global template. If there is no enterprise global template value, the default value is the same as the default in Microsoft Office Project.

## See Also

#### Concepts

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

[XML Schema for the Project Element](xml-schema-for-the-project-element.md)

