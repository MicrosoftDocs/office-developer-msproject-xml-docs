---
title: CFType Element
TOCTitle: CFType Element
ms:assetid: c4a58f3b-68ef-419f-9d73-1a50b5bc019e
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968675(v=office.12)
ms:contentKeyID: 13188365
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- CFType element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# CFType Element




The custom field type.

    <CFType>
      IntegerValue
    </CFType>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968669(v=office.12).md">ExtendedAttribute</a></p></td>
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
<td><p>Cost</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>Date</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>Duration</p></td>
</tr>
<tr class="even">
<td><p>3</p></td>
<td><p>Finish</p></td>
</tr>
<tr class="odd">
<td><p>4</p></td>
<td><p>Flag</p></td>
</tr>
<tr class="even">
<td><p>5</p></td>
<td><p>Number</p></td>
</tr>
<tr class="odd">
<td><p>6</p></td>
<td><p>Start</p></td>
</tr>
<tr class="even">
<td><p>7</p></td>
<td><p>Text</p></td>
</tr>
</tbody>
</table>

## Example

The following example uses the CFType element to indicate that the enterprise Health custom field is a text field.

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

