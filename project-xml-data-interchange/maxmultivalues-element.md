---
title: MaxMultiValues Element
TOCTitle: MaxMultiValues Element
ms:assetid: 56c818ed-8004-43a9-9339-45364ff93fee
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968512(v=office.12)
ms:contentKeyID: 13188204
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- MaxMultiValues element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# MaxMultiValues Element




The maximum number of values you can select in a custom field picklist.

    <MaxMultiValues>
      IntegerValue
    </MaxMultiValues>

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

A text value of type integer is required.

## Example

In the following example, the MaxMultiValues element indicates that you can only select a single value for the Health enterprise custom field.

``` xml
<ExtendedAttribute>
  <FieldID>188776449</FieldID>
  <FieldName>Health</FieldName>
  <CFType>7</CFType>
  <Guid>0000E8D9-65F1-4769-9BD2-819D38036FCC</Guid>
  <ElemType>20</ElemType>
  <MaxMultiValues>1</MaxMultiValues>
  <UserDef>1</UserDef>
  <SecondaryPID>255885314</SecondaryPID>
  <DefaultGuid>000079D2-4A43-41FC-B264-98D23FADD84B</DefaultGuid>
</ExtendedAttribute>
```

## See Also

#### Concepts

[ExtendedAttribute Elements and XML Structure](extendedattribute-elements-and-xml-structure.md)

[XML Schema for the ExtendedAttributes Element](xml-schema-for-the-extendedattributes-element.md)

