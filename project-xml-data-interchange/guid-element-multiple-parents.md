---
title: Guid Element (Multiple Parents)
TOCTitle: Guid Element
ms:assetid: 24a60efb-8976-4308-b601-e5a285b8a79f
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968441(v=office.12)
ms:contentKeyID: 13188134
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- Guid element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# Guid Element (Multiple Parents)




The globally unique identifier (GUID) of an outline code or enterprise custom field.

    <Guid>
        StringValue
    <Guid>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968410(v=office.12).md">OutlineCode</a>, <a href="bb968669(v=office.12).md">ExtendedAttribute</a></p></td>
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
<td><p>Minimum: 0 for local custom fields; 1 for outline codes and enterprise custom fields.</p>
<p>Maximum: 1</p></td>
</tr>
</tbody>
</table>

## Text Value

A text value of type string is required. The string must be in the form "HHHHHHHH-HHHH-HHHH-HHHH-HHHHHHHHHHHH" where H represents a hexadecimal digit between 0 and F.

## Remarks

For the ExtendedAttribute element, Guid is the custom field GUID.

For the OutlineCode element, Guid is the outline code GUID. Local outline codes and enterprise custom fields and require the Guid element; local custom fields do not.

## Example

In the following example, Text1 is a local task custom field, which does not include the Guid element. Health is an enterprise custom field, which uses the Guid element to represent the GUID of the enterprise custom field.

``` xml
<ExtendedAttributes>
  <ExtendedAttribute>
    <FieldID>188743731</FieldID>
    <FieldName>Text1</FieldName>
    <Alias>Test Task CF</Alias>
    <Ltuid>ED2E65AD-00A1-4457-97FA-A3FC708C9183</Ltuid>
    <SecondaryPID>255869028</SecondaryPID>
  </ExtendedAttribute>
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
</ExtendedAttributes>
```

## See Also

#### Concepts

[OutlineCode Elements and XML Structure](bb968596\(v=office.12\).md)

[XML Schema for the OutlineCodes Element](bb968584\(v=office.12\).md)

[ExtendedAttribute Elements and XML Structure](bb968579\(v=office.12\).md)

[XML Schema for the ExtendedAttributes Element](bb968705\(v=office.12\).md)

