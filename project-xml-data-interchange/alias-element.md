---
title: Alias Element
TOCTitle: Alias Element
ms:assetid: 01c1a8dd-39cc-490d-84de-d75c4ba95fd1
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968395(v=office.12)
ms:contentKeyID: 13188088
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- Alias element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# Alias Element




The alias of the custom field or outline code.

    <Alias>
      String(50): for OutlineCode or ExtendedAttribute
    </Alias>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="extendedattribute-element.md">ExtendedAttribute</a>, <a href="outlinecode-element.md">OutlineCode</a></p></td>
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

## Example

In the following example, the alias of the task local custom field named Duration6 is Test Duration. Microsoft Office Project would show the custom field in a list as **Test Duration (Duration6)**.

``` xml
<ExtendedAttributes>
   <ExtendedAttribute>
      <FieldID>188743957</FieldID>
      <FieldName>Duration6</FieldName>
      <Alias>Test Duration</Alias>
      <SecondaryPID>255868973</SecondaryPID>
      <RollupType>3</RollupType>
      <CalculationType>1</CalculationType>
      <Formula>[Duration]*3</Formula>
   </ExtendedAttribute>
</ExtendedAttributes>
```

## See Also

#### Concepts

[OutlineCode Elements and XML Structure](outlinecode-elements-and-xml-structure.md)

[XML Schema for the OutlineCodes Element](xml-schema-for-the-outlinecodes-element.md)

[ExtendedAttribute Elements and XML Structure](extendedattribute-elements-and-xml-structure.md)

[XML Schema for the ExtendedAttributes Element](xml-schema-for-the-extendedattributes-element.md)

