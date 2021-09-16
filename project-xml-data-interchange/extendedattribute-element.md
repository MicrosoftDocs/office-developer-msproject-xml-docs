---
title: ExtendedAttribute Element
TOCTitle: ExtendedAttribute Element
ms:assetid: c16eb20b-416e-4659-9d5a-2c006a45a1fb
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968669(v=office.12)
ms:contentKeyID: 13188359
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- ExtendedAttribute element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# ExtendedAttribute Element




An extended attribute represents a custom field or outline code in Microsoft Office Project. The extended attribute can be a local custom field or outline code, or it can be an enterprise custom field. The definition depends on whether an extended attribute is defined within an ExtendedAttributes collection, or in a Task, Resource, or Assignment. In general, there can be an unlimited number of extended attributes, subject to the limitations described in the Remarks section.

    <ExtendedAttribute>
      ComplexTypeValue
    </ExtendedAttribute>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="extendedattributes-element.md">ExtendedAttributes</a>, <a href="task-element.md">Task</a>, <a href="resource-element.md">Resource</a>, <a href="assignment-element.md">Assignment</a></p></td>
</tr>
</tbody>
</table>

## Child Elements for the ExtendedAttributes Collection

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Element</p></th>
<th><p>Required / Optional</p></th>
<th><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="fieldid-element.md">FieldID</a></p></td>
<td><p>Optional</p></td>
<td><p>Corresponds to the enumeration value of the local custom field (Text1, Text2, and so forth). FieldID is not unique across multiple projects.</p></td>
</tr>
<tr class="even">
<td><p><a href="fieldname-element.md">FieldName</a></p></td>
<td><p>Optional</p></td>
<td><p>Name of the custom field.</p></td>
</tr>
<tr class="odd">
<td><p><a href="cftype-element.md">CFType</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Type of custom field (cost, date, duration, finish, flag, number, start, or text).</p></td>
</tr>
<tr class="even">
<td><p><a href="guid-element-multiple-parents.md">Guid</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. GUID of the custom field.</p></td>
</tr>
<tr class="odd">
<td><p><a href="elemtype-element.md">ElemType</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Type of entity (task, resource, or assignment) with which the custom field is associated.</p></td>
</tr>
<tr class="even">
<td><p><a href="maxmultivalues-element.md">MaxMultiValues</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Maximum number of values you can select in a custom field value list</p></td>
</tr>
<tr class="odd">
<td><p><a href="userdef-element.md">UserDef</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Indicates whether the custom field is user defined.</p></td>
</tr>
<tr class="even">
<td><p><a href="alias-element.md">Alias</a></p></td>
<td><p>Optional</p></td>
<td><p>Alias of the custom field.</p></td>
</tr>
<tr class="odd">
<td><p><a href="secondarypid-element.md">SecondaryPID</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Secondary project identifier (PID) of the custom field for assignment roll down.</p></td>
</tr>
<tr class="even">
<td><p><a href="autorolldown-element.md">AutoRollDown</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Indicates whether automatic roll down of custom field values to the assignment level is enabled.</p></td>
</tr>
<tr class="odd">
<td><p><a href="defaultguid-element.md">DefaultGuid</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Specifies the GUID of the default lookup table entry.</p></td>
</tr>
<tr class="even">
<td><p><a href="ltuid-element.md">Ltuid</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. GUID of the lookup table associated with the custom field.</p></td>
</tr>
<tr class="odd">
<td><p><a href="phoneticalias-element.md">PhoneticAlias</a></p></td>
<td><p>Optional</p></td>
<td><p>Contains phonetic information in either Hiragana or Katakana for an extended attribute; used only in the Japanese version of Project.</p></td>
</tr>
<tr class="even">
<td><p><a href="rolluptype-element.md">RollupType</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates the method used to calculate roll-ups to summary tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="calculationtype-element.md">CalculationType</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether roll-ups are calculated for task and group summary rows.</p></td>
</tr>
<tr class="even">
<td><p><a href="formula-element.md">Formula</a></p></td>
<td><p>Optional</p></td>
<td><p>Formula that Project uses to populate the custom field.</p></td>
</tr>
<tr class="odd">
<td><p><a href="restrictvalues-element.md">RestrictValues</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether only values in the list are allowed in the file.</p></td>
</tr>
<tr class="even">
<td><p><a href="valuelistsortorder-element.md">ValuelistSortOrder</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Indicates how value lists are sorted (descending or ascending).</p></td>
</tr>
<tr class="odd">
<td><p><a href="appendnewvalues-element.md">AppendNewValues</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether new values added to the project are automatically added to the list.</p></td>
</tr>
<tr class="even">
<td><p><a href="default-element-extendedattribute.md">Default</a></p></td>
<td><p>Optional</p></td>
<td><p>Refers to the ID of the default value in the list; not used if there is no default set.</p></td>
</tr>
<tr class="odd">
<td><p><a href="valuelist-element.md">ValueList</a></p></td>
<td><p>Optional</p></td>
<td><p>The collection of extended attribute values.</p></td>
</tr>
</tbody>
</table>

## Child Elements for a Task, Resource, or Assignment

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Element</p></th>
<th><p>Required / Optional</p></th>
<th><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="fieldid-element.md">FieldID Element</a></p></td>
<td><p>Optional</p></td>
<td><p>Field ID for the extended attribute.</p></td>
</tr>
<tr class="even">
<td><p><a href="value-element.md">Value Element</a></p></td>
<td><p>Optional</p></td>
<td><p>Actual value of the extended attribute.</p></td>
</tr>
<tr class="odd">
<td><p><a href="durationformat-element.md">DurationFormat Element</a></p></td>
<td><p>Optional</p></td>
<td><p>An enumeration of the duration format for the extended attribute (day, week, month, and so forth).</p></td>
</tr>
<tr class="even">
<td><p><a href="valueguid-element.md">ValueGUID</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. GUID of the value in the custom field value list. The ValueGUID matches the FieldGUID in the Value element, for multi-value custom fields.</p></td>
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

The following two pieces of data are necessary to specify the value of an ExtendedAttribute in a task, resource, or assignment:

  - A pointer to the extended attribute definition that is specified by the FieldID element.

  - The custom field value, which is specified by the Value element or by the ValueGUID pointer to the Value element in the value list. The ValueGUID matches the FieldGUID in the value list.

If the custom field is of type Duration, the value requires the DurationFormat element. If the custom field is calculated by a formula, ValueGUID shows the following: \<ValueGUID\>00000000-0000-0000-0000-000000000000\</ValueGUID\>


> [!NOTE]
> When loading a project stored as XML data, Microsoft Office Project recognizes a maximum of 5000 ValueList elements. All others are ignored.


## Example

The FieldName value corresponds to PjCustomField enumeration value in the FieldID element. For example, the FieldID 188743731 for the Information local custom field matches the pjCustomTaskText1 value in [PjCustomField Enumeration](http://msdn2.microsoft.com/en-ca/library/bb221982.aspx).


> [!NOTE]
> The FieldID 205521019 is currently missing in the PjCustomField documentation. However, you can find in the Object Browser in the Project Visual Basic editor (VBE), the value is for pjCustomResourceCost1.


``` xml
<ExtendedAttributes>
   <ExtendedAttribute>
      <FieldID>188743731</FieldID>
      <FieldName>Text1</FieldName>
      <Alias>Information</Alias>
      <Ltuid>6F76DA0E-4294-467A-9A66-5E2909578CE8</Ltuid>
      <SecondaryPID>255869028</SecondaryPID>
      <DefaultGuid>D2C35FC6-639A-4F88-A1FF-987F432F3A9D</DefaultGuid>
   </ExtendedAttribute>
   <ExtendedAttribute>
      <FieldID>205521019</FieldID>
      <FieldName>Cost1</FieldName>
      <Alias>Extra Cost</Alias>
      <Ltuid>06AC981F-E8E6-4F20-A26F-8A408A36660B</Ltuid>
      <SecondaryPID>255852663</SecondaryPID>
      <AutoRollDown>1</AutoRollDown>
   </ExtendedAttribute>
</ExtendedAttributes>
. . .
<Tasks>
   <Task>
      <UID>1</UID>
      <ID>1</ID>
      <Name>T1</Name>
      . . .
      <ExtendedAttribute>
         <FieldID>188743731</FieldID>
         <Value>Info 1</Value>
         <ValueGUID>D2C35FC6-639A-4F88-A1FF-987F432F3A9D</ValueGUID>
      </ExtendedAttribute>
   </Task>
   </Task>
</Tasks>
. . .
<Resources>
   <Resource>
      <UID>1</UID>
      <ID>1</ID>
      <Name>R1</Name>
      . . .
      <ExtendedAttribute>
         <FieldID>205521019</FieldID>
         <Value>3000</Value>
         <ValueGUID>1EBF58AF-8EF0-400C-8E36-78628FF0E21C</ValueGUID>
      </ExtendedAttribute>
   </Resource>
</Resources>
```

## See Also

#### Reference

[OutlineCode Element](outlinecode-element.md)

#### Concepts

[ExtendedAttribute Elements and XML Structure](extendedattribute-elements-and-xml-structure.md)

[XML Schema for the ExtendedAttributes Element](xml-schema-for-the-extendedattributes-element.md)

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

[Resource Elements and XML Structure](resource-elements-and-xml-structure.md)

[XML Schema for the Resources Element](xml-schema-for-the-resources-element.md)

[Assignment Elements and XML Structure](assignment-elements-and-xml-structure.md)

[XML Schema for the Assignments Element](xml-schema-for-the-assignments-element.md)

#### Other Resources

[PjCustomField Enumeration](http://msdn2.microsoft.com/en-ca/library/bb221982.aspx)

