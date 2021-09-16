---
title: OutlineCode Element
TOCTitle: OutlineCode Element
ms:assetid: 0dc0478b-4281-4e0e-86c0-3fdea445e6d0
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968410(v=office.12)
ms:contentKeyID: 13188103
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- OutlineCode element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# OutlineCode Element




Defines an outline code and associated value list in a project, or specifies the value of an outline code element for a resource or task.

    <OutlineCode>
      ComplexTypeValue
    </OutlineCode>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="outlinecodes-element.md">OutlineCodes</a>, <a href="resource-element.md">Resource</a>, <a href="task-element.md">Task</a></p></td>
</tr>
</tbody>
</table>

## Child Elements at the Project Level

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Element</p></th>
<th><p>Required/Optional</p></th>
<th><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="guid-element-multiple-parents.md">Guid</a></p></td>
<td><p>Required</p></td>
<td><p>New in Microsoft Office Project 2007. The globally unique identifier (GUID) of the outline code. Corresponds to the Ltuid element in associated ExtendedAttribute values.</p></td>
</tr>
<tr class="even">
<td><p><a href="fieldid-element.md">FieldID</a></p></td>
<td><p>Optional</p></td>
<td><p>Field ID number for the outline code. Field numbers correspond to Outline Code1, Outline Code2, . . . , Outline Code10, for resources and tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="fieldname-element.md">FieldName</a></p></td>
<td><p>Optional</p></td>
<td><p>Name of the custom outline code.</p></td>
</tr>
<tr class="even">
<td><p><a href="alias-element.md">Alias</a></p></td>
<td><p>Optional</p></td>
<td><p>Alias of the outline code.</p></td>
</tr>
<tr class="odd">
<td><p><a href="phoneticalias-element.md">PhoneticAlias</a></p></td>
<td><p>Optional</p></td>
<td><p>Contains phonetic pronunciation information in either Hiragana or Katakana for a custom outline code; used only in the Japanese version of Project.</p></td>
</tr>
<tr class="even">
<td><p><a href="values-element.md">Values</a></p></td>
<td><p>Optional</p></td>
<td><p>Collection of the value definitions of the outline code.</p></td>
</tr>
<tr class="odd">
<td><p><a href="enterprise-element.md">Enterprise</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the outline code is an enterprise custom field.</p></td>
</tr>
<tr class="even">
<td><p><a href="enterpriseoutlinecodealias-element.md">EnterpriseOutlineCodeAlias</a></p></td>
<td><p>Optional</p></td>
<td><p>Refers to an enterprise custom field for which the outline code is an alias.</p></td>
</tr>
<tr class="odd">
<td><p><a href="resourcesubstitutionenabled-element.md">ResourceSubstitutionEnabled</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the outline code is used with the Resource Substitution Wizard in Project. The Resource Substitution Wizard is used only with enterprise custom fields.</p></td>
</tr>
<tr class="even">
<td><p><a href="leafonly-element.md">LeafOnly</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the value specified for an outline code in a resource or task must be a leaf value.</p></td>
</tr>
<tr class="odd">
<td><p><a href="alllevelsrequired-element.md">AllLevelsRequired</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether new codes must have all levels present. Not used for enterprise custom fields.</p></td>
</tr>
<tr class="even">
<td><p><a href="onlytablevaluesallowed-element.md">OnlyTableValuesAllowed</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the outline code value must come from the associated lookup table.</p></td>
</tr>
<tr class="odd">
<td><p><a href="masks-element.md">Masks</a></p></td>
<td><p>Optional</p></td>
<td><p>Collection of code masks for the outline code value list.</p></td>
</tr>
</tbody>
</table>

## Child Elements at the Task and Resource Level

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Element</p></th>
<th><p>Required/Optional</p></th>
<th><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="fieldid-element.md">FieldID</a></p></td>
<td><p>Required</p></td>
<td><p>Field ID number for the outline code. Field numbers correspond to Outline Code1, Outline Code2, . . . , Outline Code10, for resources and tasks.</p></td>
</tr>
<tr class="even">
<td><p><a href="valueid-element.md">ValueID</a></p></td>
<td><p>Optional</p></td>
<td><p>Local ID number in the Value list associated with the outline code definition. Required for Project 2003 to read XML files saved from Project 2007.</p></td>
</tr>
<tr class="odd">
<td><p><a href="valueguid-element.md">ValueGUID</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. GUID of the value in the outline code value list. The ValueGUID matches the FieldGUID in the Value element.</p></td>
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
<p>Maximum: Unbounded</p></td>
</tr>
</tbody>
</table>

## Remarks

An outline code, with the corresponding code mask and table of values, is defined in the collection of OutlineCodes in a project. Each outline code has an associated ExtendedAttribute that specifies the outline code field type and alias.

Resources or tasks that contain outline code values include an OutlineCode element for each value. The following two pieces of data are necessary to specify the value of an OutlineCode element in a resource or task:

  - A pointer to the outline code definition that is specified by the FieldID element.

  - The outline code value, which is specified by the ValueID and the ValueGUID pointer to the Value element in the value list. The ValueGUID matches the FieldGUID in the value list. Project 2007 ignores ValueID and uses ValueGUID.

## Example

In the following example, the Guid value in the outline code definition corresponds to the Ltuid value in the associated ExtendedAttribute. The outline code alias is *Task Simple OC* for the *Outline Code6* field name. The FieldID 188744106 matches the pjCustomTaskOutlineCode6 enumeration value in the [PjCustomField Enumeration](http://msdn2.microsoft.com/en-ca/library/bb221982.aspx). You can also use the Object Browser in the Project Visual Basic editor (VBE) to find values in the PjCustomField enumeration.

The outline code mask defines one level of characters (Type = 3), of any length (Length = 0).

ValueGUID and ValueID for the outline code in the task both correspond to the *Simple 2* value in the *Task Simple OC* outline code.

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

[Ltuid Element](ltuid-element.md)

[ExtendedAttribute Element](extendedattribute-element.md)

#### Concepts

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

[XML Schema for the Project Element](xml-schema-for-the-project-element.md)

[OutlineCode Elements and XML Structure](outlinecode-elements-and-xml-structure.md)

[XML Schema for the OutlineCodes Element](xml-schema-for-the-outlinecodes-element.md)

[Resource Elements and XML Structure](resource-elements-and-xml-structure.md)

[XML Schema for the Resources Element](xml-schema-for-the-resources-element.md)

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

#### Other Resources

[PjCustomField Enumeration](http://msdn2.microsoft.com/en-ca/library/bb221982.aspx)

