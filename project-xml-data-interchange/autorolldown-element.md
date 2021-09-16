---
title: AutoRollDown Element
TOCTitle: AutoRollDown Element
ms:assetid: 1c644e22-6e35-4a74-a845-e7665a45da1b
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968428(v=office.12)
ms:contentKeyID: 13188121
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- AutoRollDown element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# AutoRollDown Element




Indicates whether automatic rolldown of custom field values to the assignment level is enabled.

    <AutoRollDown>
      BooleanValue
    </AutoRollDown>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="extendedattribute-element.md">ExtendedAttribute</a></p></td>
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

The following example uses the AutoRollDown element to specify that configured values for the Team Name custom field should roll down to the assignment level.

``` xml
<ExtendedAttribute>
  <FieldID>205553664</FieldID>
  <FieldName>Team Name</FieldName>
  <CFType>7</CFType>
  <Guid>0000740F-CF67-4B93-A405-F0C12C5BC942</Guid>
  <ElemType>21</ElemType>
  <MaxMultiValues>1</MaxMultiValues>
  <UserDef>1</UserDef>
  <SecondaryPID>255885312</SecondaryPID>
  <AutoRollDown>1</AutoRollDown>
</ExtendedAttribute>
```

## See Also

#### Concepts

[ExtendedAttribute Elements and XML Structure](extendedattribute-elements-and-xml-structure.md)

[XML Schema for the ExtendedAttributes Element](xml-schema-for-the-extendedattributes-element.md)

