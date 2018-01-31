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
---

# Alias Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

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
<td><p><a href="bb968669(v=office.12).md">ExtendedAttribute</a>, <a href="bb968410(v=office.12).md">OutlineCode</a></p></td>
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

[OutlineCode Elements and XML Structure](bb968596\(v=office.12\).md)

[XML Schema for the OutlineCodes Element](bb968584\(v=office.12\).md)

[ExtendedAttribute Elements and XML Structure](bb968579\(v=office.12\).md)

[XML Schema for the ExtendedAttributes Element](bb968705\(v=office.12\).md)

