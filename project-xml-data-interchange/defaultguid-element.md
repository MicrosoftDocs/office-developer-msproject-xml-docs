---
title: DefaultGuid Element
TOCTitle: DefaultGuid Element
ms:assetid: 22c2fd78-5409-4ce5-9e81-c62bd6403757
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968436(v=office.12)
ms:contentKeyID: 13188129
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- DefaultGuid element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# DefaultGuid Element




Specifies the GUID of the default lookup table entry.

    <DefaultGuid>
      StringValue
    </DefaultGuid>

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

A text value of type string is required. The string must be in the form "HHHHHHHH-HHHH-HHHH-HHHH-HHHHHHHHHHHH" where H represents a hexadecimal digit between 0 and F.

## Example

The following example uses the DefaultGuid element to specify the GUID of the default lookup table value for the Health enterprise custom field.

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

[ExtendedAttribute Elements and XML Structure](bb968579\(v=office.12\).md)

[XML Schema for the ExtendedAttributes Element](bb968705\(v=office.12\).md)

