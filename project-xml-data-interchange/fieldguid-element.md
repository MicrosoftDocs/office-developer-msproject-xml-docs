---
title: FieldGUID Element
TOCTitle: FieldGUID Element
ms:assetid: aa629c7c-8921-42c6-9f82-000baf39c3fa
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968634(v=office.12)
ms:contentKeyID: 13188325
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- FieldGUID element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# FieldGUID Element




Globally unique identifier (GUID) of an outline code value.

    <FieldGUID>
      StringValue
    </FieldGUID>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968696(v=office.12).md">Value</a></p></td>
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

## Remarks

FieldGUID corresponds to the [ValueGUID](valueguid-element.md) element in the outline code value for a task or resource.

## Example

In the following example, the outline code has two values. Each value satisfies the code mask for any number of characters (the mask Type = 3 and the mask Length = 0).

The ValueID is unique only within the project and the FieldGUID is unique across all projects. ValueID is required for Microsoft Office Project 2003 to read XML files saved from Project 2007. Project 2007 ignores ValueID and uses FieldGUID.

``` xml
<OutlineCodes>
   <OutlineCode>
      <Guid>26F0CA77-38CC-40C7-933D-15F839F7DB82</Guid>
      <Enterprise>0</Enterprise>
      <ResourceSubstitutionEnabled>0</ResourceSubstitutionEnabled>
      <LeafOnly>0</LeafOnly>
      <AllLevelsRequired>0</AllLevelsRequired>
      <OnlyTableValuesAllowed>0</OnlyTableValuesAllowed>
      <Masks>
         <Mask>
            <Level>1</Level>
            <Type>3</Type>
            <Length>0</Length>
            <Separator>.</Separator>
         </Mask>
      </Masks>
      <Values>
         <Value>
            <ValueID>16</ValueID>
            <FieldGUID>985194AB-77BA-4545-BCE8-99761B5538D9</FieldGUID>
            <ParentValueID>0</ParentValueID>
            <Type>21</Type>
            <Value>Simple 1</Value>
         </Value>
         <Value>
            <ValueID>17</ValueID>
            <FieldGUID>6B0CC455-EE19-416A-8FD9-6209590B3ED7</FieldGUID>
            <ParentValueID>0</ParentValueID>
            <Type>21</Type>
            <Value>Simple 2</Value>
         </Value>
      </Values>
   </OutlineCode>
</OutlineCodes>
```

## See Also

#### Reference

[ValueID Element](valueid-element.md)

#### Concepts

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

[XML Schema for the Project Element](xml-schema-for-the-project-element.md)

[OutlineCode Elements and XML Structure](outlinecode-elements-and-xml-structure.md)

[XML Schema for the OutlineCodes Element](xml-schema-for-the-outlinecodes-element.md)

