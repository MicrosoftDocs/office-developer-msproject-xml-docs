---
title: ValueGUID Element
TOCTitle: ValueGUID Element
ms:assetid: 8478818f-6da6-431f-b4d0-d2113329a476
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968572(v=office.12)
ms:contentKeyID: 13188263
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- ValueGUID element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# ValueGUID Element




Globally unique identifier (GUID) of the value of an outline code or custom field for a resource or task.

    <ValueGUID>
      StringValue
    </ValueGUID>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="extendedattribute-element.md">ExtendedAttribute</a>, <a href="outlinecode-element.md">OutlineCode</a></p></td>
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

ValueGUID in a resource or task outline code value corresponds to the FieldGUID value in the outline code definition.

If a task or resource custom field rolls down to assignments, the Assignment element contains an ExtendedAttribute that has the ValueGUID.

## Example

In the following example, ValueGUID and ValueID for the outline code in the task both correspond to the *Simple 2* value in the outline code named *Task Simple OC*.

``` xml
<Project xmlns="http://schemas.microsoft.com/project">
   . . .
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
   . . .
   <ExtendedAttributes>
      <ExtendedAttribute>
         <FieldID>188744106</FieldID>
         <FieldName>Outline Code6</FieldName>
         <Alias>Task Simple OC</Alias>
         <Ltuid>26F0CA77-38CC-40C7-933D-15F839F7DB82</Ltuid>
         <SecondaryPID>255869013</SecondaryPID>
      </ExtendedAttribute>
   </ExtendedAttributes>
   . . .
   <Tasks>
      <Task>
         . . .
         <OutlineCode>
            <FieldID>188744106</FieldID>
            <ValueID>17</ValueID>
            <ValueGUID>6B0CC455-EE19-416A-8FD9-6209590B3ED7</ValueGUID>
         </OutlineCode>
         . . .
      </Task>
   </Tasks>
   . . .
</Project>
```

## See Also

#### Reference

[OutlineCode Element](outlinecode-element.md)

#### Concepts

[OutlineCode Elements and XML Structure](outlinecode-elements-and-xml-structure.md)

[XML Schema for the OutlineCodes Element](xml-schema-for-the-outlinecodes-element.md)

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

[Resource Elements and XML Structure](resource-elements-and-xml-structure.md)

[XML Schema for the Resources Element](xml-schema-for-the-resources-element.md)

