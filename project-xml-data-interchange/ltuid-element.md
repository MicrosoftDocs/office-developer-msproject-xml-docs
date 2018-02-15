---
title: Ltuid Element
TOCTitle: Ltuid Element
ms:assetid: 9c171e76-bf69-48e6-836d-7eb83080e430
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968607(v=office.12)
ms:contentKeyID: 13188298
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- Ltuid element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# Ltuid Element




The globally unique identifier (GUID) of the lookup table associated with a custom field.

    <Ltuid>
      StringValue
    </Ltuid>

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

A text value of type string is required. The string must be in the form "HHHHHHHH-HHHH-HHHH-HHHH-HHHHHHHHHHHH" where "H" represents a hexadecimal digit between 0 and F.

## Example

The following example uses the Ltuid element to specify the GUID of the lookup table defined for a local custom field.

``` xml
<ExtendedAttribute>
  <FieldID>188743731</FieldID>
  <FieldName>Text1</FieldName>
  <Alias>MyLocalCustomField</Alias>
  <Ltuid>E8B19FF9-82ED-492C-A524-530640FBF913</Ltuid>
  <SecondaryPID>255869028</SecondaryPID>
  <DefaultGuid>0972C697-2DE3-46C5-8841-9CD7209989AE</DefaultGuid>
</ExtendedAttribute>
```

## See Also

#### Concepts

[ExtendedAttribute Elements and XML Structure](extendedattribute-elements-and-xml-structure.md)

[XML Schema for the ExtendedAttributes Element](xml-schema-for-the-extendedattributes-element.md)

