---
title: b608000 - b617fff Elements
TOCTitle: b608000 - b617fff Elements
ms:assetid: 6c774043-2a50-47f8-97a0-815ade5bf2ad
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968536(v=office.12)
ms:contentKeyID: 13188228
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- b608000 - b617fff elements
dev_langs:
- xml
---

# b608000 - b617fff Elements

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

A project-level enterprise custom field value.

    <b608000>
        CustomFieldValue
    </b608000>

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
<td><p>Specifies the format for a duration custom field value (days, weeks, months, and so on). For more information, see <a href="bb968637(v=office.12).md">DurationFormat Element</a>.</p></td>
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
<td><p><a href="bb968487(v=office.12).md">Task</a></p></td>
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

A text value is required. This text specifies the enterprise custom field value for the project.


> [!NOTE]
> The text value must match the data type required by the custom field definition.


## Remarks

The name of the XML element that stores the enterprise custom field value corresponds to the hexadecimal representation of the custom field ID.

Table 1 lists the valid range of custom field IDs for project-level enterprise custom fields in both decimal and hexadecimal format.

Table 1. Project-level Enterprise Custom Field IDs

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
<td><p>190873600 – 190939135</p></td>
<td><p>b608000 – b617fff</p></td>
</tr>
</tbody>
</table>

For more information, see [Custom Field Data in XML](bb968687\(v=office.12\).md).

## Example

The following example shows two different representations of enterprise project custom field data.

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
<td><p>b608007</p></td>
<td><p>190873607</p></td>
<td><p>FieldName: ProjectNumberTest, a number custom field with a lookup table.</p>
<p>Guid: Refers to the custom field GUID.</p>
<p>DefaultGuid: Refers to the default value in the associated lookup table of the ProjectNumberTest custom field.</p>
<p>The GUID value of the b608007 element specifies the actual lookup table value.</p></td>
</tr>
<tr class="even">
<td><p>b60800a</p></td>
<td><p>205553676</p></td>
<td><p>FieldName: ProjectDurationNL, a duration custom field that has no lookup table.</p>
<p>The DurationFormat=&quot;9&quot; attribute specifies the duration format as weeks.</p>
<p>The value PT280H0M0S specifies 280 hours, 0 minutes, and 0 seconds. Because the work week is 40 hours, that is seven weeks. (PT stands for Project Time, for internal use.)</p>
<p>Project Professional shows the value of the custom field as &quot;7 wks.&quot;</p></td>
</tr>
</tbody>
</table>

``` xml
<Project xmlns="http://schemas.microsoft.com/project">
   . . .
   <ExtendedAttributes>
      <ExtendedAttribute>
         <FieldID>190873607</FieldID>
         <FieldName>ProjectNumberTest</FieldName>
         <CFType>5</CFType>
         <Guid>7AA9C196-A0BB-4FA0-BBDD-E16B6C36901A</Guid>
         <ElemType>20</ElemType>
         <MaxMultiValues>1</MaxMultiValues>
         <UserDef>1</UserDef>
         <DefaultGuid>EBDF240A-AE0B-4224-A8B8-3FA4B7EA709F</DefaultGuid>
      </ExtendedAttribute>
      <ExtendedAttribute>
         <FieldID>190873610</FieldID>
         <FieldName>ProjectDurationNL</FieldName>
         <CFType>2</CFType>
         <Guid>0FA0F636-98A0-4841-8129-08B84560E977</Guid>
         <ElemType>20</ElemType>
         <MaxMultiValues>1</MaxMultiValues>
         <UserDef>1</UserDef>
      </ExtendedAttribute>
   </ExtendedAttributes>
   . . .
   <Tasks>
      <Task>
         . . .
         <b608007>59B6725E-92B7-4242-9CCB-00AFA1B0A9C1</b608007>
         <b60800a DurationFormat="9">PT280H0M0S</b60800a>
         . . .
      </Task>
   </Tasks>
   . . .
</Project>
```

## See Also

#### Concepts

[Task Elements and XML Structure](bb968475\(v=office.12\).md)

[XML Schema for the Tasks Element](bb968415\(v=office.12\).md)

[Custom Field Data in XML](bb968687\(v=office.12\).md)

