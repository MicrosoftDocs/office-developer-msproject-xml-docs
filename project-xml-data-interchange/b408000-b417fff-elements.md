---
title: b408000 - b417fff Elements
TOCTitle: b408000 - b417fff Elements
ms:assetid: eb451420-0c38-4c84-8029-4a3261f24a01
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968719(v=office.12)
ms:contentKeyID: 13188409
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- b408000 - b417fff elements
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
localization_priority: Normal
---

# b408000 - b417fff Elements




A task-level enterprise custom field value.

    <b408000>
        CustomFieldValue
    </b408000>

## Attributes

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Attribute</p></th>
<th><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>DurationFormat</p></td>
<td><p>Specifies the format for a duration custom field value (days, weeks, months, and so on). For more information, see <a href="durationformat-element.md">DurationFormat Element</a>.</p></td>
</tr>
</tbody>
</table>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="task-element.md">Task</a></p></td>
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
<p>Maximum: 1 of each unique element name</p></td>
</tr>
</tbody>
</table>

## Text Value

A text value is required. This text specifies the enterprise custom field value for the task.


> [!NOTE]
> The text value must match the data type required by the custom field definition.


## Remarks

The name of the XML element that stores the enterprise custom field value corresponds to the hexadecimal representation of the custom field ID.

Table 1 lists the valid range of custom field IDs for task-level enterprise custom fields in both decimal and hexadecimal format.

Table 1. Task-level Enterprise Custom Field IDs

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Custom Field ID range (decimal)</p></th>
<th><p>Custom Field ID range (hexadecimal)</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>188776448 – 188841983</p></td>
<td><p>b408000 – b417fff</p></td>
</tr>
</tbody>
</table>

For more information, see [Custom Field Data in XML](custom-field-data-in-xml.md).

## Example

The following example shows three different representations of enterprise task custom field data.

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th><p><strong>Element</strong></p></th>
<th><p><strong>Decimal value of FieldID</strong></p></th>
<th><p><strong>Description</strong></p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>b408011</p></td>
<td><p>188776465</p></td>
<td><p>FieldName: TaskNumberTest, a number custom field with a lookup table.</p>
<p>Guid: Refers to the custom field GUID.</p>
<p>DefaultGuid: Refers to the default value in the associated lookup table of the TaskNumberTest custom field.</p>
<p>The GUID value of the b408011 element specifies the actual lookup table value.</p></td>
</tr>
<tr class="even">
<td><p>b408013</p></td>
<td><p>188776467</p></td>
<td><p>FieldName: TaskCostNL, a cost custom field that has no lookup table.</p>
<p>The value of the b408013 element is 7000. The US English installation of Project Professional shows the value as $70.00.</p></td>
</tr>
<tr class="odd">
<td><p>b408015</p></td>
<td><p>188776469</p></td>
<td><p>FieldName: TaskDurationNL, a duration custom field that has no lookup table.</p>
<p>The DurationFormat=&quot;7&quot; attribute specifies the duration format as days.</p>
<p>The value PT40H0M0S specifies 40 hours, 0 minutes, and 0 seconds. Because the work day is 8 hours, that is five days. (PT stands for Project Time, for internal use.)</p>
<p>Project Professional shows the value of the custom field as &quot;5 days.&quot;</p></td>
</tr>
</tbody>
</table>

``` xml
<Project xmlns="http://schemas.microsoft.com/project">
   . . .
   <ExtendedAttributes>
      <ExtendedAttribute>
         <FieldID>188776465</FieldID>
         <FieldName>TaskNumberTest</FieldName>
         <CFType>5</CFType>
         <Guid>DE6BF35E-9D93-40EC-A1A4-72506A9CFBDC</Guid>
         <ElemType>20</ElemType>
         <MaxMultiValues>1</MaxMultiValues>
         <UserDef>1</UserDef>
         <SecondaryPID>255885321</SecondaryPID>
         <AutoRollDown>1</AutoRollDown>
         <DefaultGuid>EBDF240A-AE0B-4224-A8B8-3FA4B7EA709F</DefaultGuid>
      </ExtendedAttribute>
      <ExtendedAttribute>
         <FieldID>188776467</FieldID>
         <FieldName>TaskCostNL</FieldName>
         <CFType>0</CFType>
         <Guid>8E00874F-EA6F-4FED-BBB7-332BCCA44B3E</Guid>
         <ElemType>20</ElemType>
         <MaxMultiValues>1</MaxMultiValues>
         <UserDef>1</UserDef>
         <SecondaryPID>255885323</SecondaryPID>
         <RollupType>3</RollupType>
         <CalculationType>1</CalculationType>
         <AutoRollDown>1</AutoRollDown>
      </ExtendedAttribute>
      <ExtendedAttribute>
         <FieldID>188776469</FieldID>
         <FieldName>TaskDurationNL</FieldName>
         <CFType>2</CFType>
         <Guid>BBC34DFF-D929-4CF3-8335-EFDA2DD38F11</Guid>
         <ElemType>20</ElemType>
         <MaxMultiValues>1</MaxMultiValues>
         <UserDef>1</UserDef>
         <SecondaryPID>255885325</SecondaryPID>
         <RollupType>3</RollupType>
         <CalculationType>1</CalculationType>
         <AutoRollDown>1</AutoRollDown>
      </ExtendedAttribute>
   </ExtendedAttributes>
   . . .
   <Tasks>
      <Task>
         . . .
         <b408011>D3561646-A7F0-4196-B211-E67E232A46EC</b408011>
         <b408013>7000</b408013>
         <b408015 DurationFormat="7">PT40H0M0S</b408015>
         . . .
      </Task>
   </Tasks>
   . . .
</Project>
```

## See Also

#### Concepts

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

[Custom Field Data in XML](custom-field-data-in-xml.md)

