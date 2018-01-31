---
title: c408000 - c417fff Elements
TOCTitle: c408000 - c417fff Elements
ms:assetid: 603a3b7d-fa41-44eb-8aef-7cc99c54439c
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968524(v=office.12)
ms:contentKeyID: 13188216
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- c408000 - c417fff elements
dev_langs:
- xml
---

# c408000 - c417fff Elements

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

A resource-level enterprise custom field value.

    <c408000>
        CustomFieldValue
    </c408000>

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
<td><p><a href="bb968715(v=office.12).md">Resource Element</a></p></td>
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

A text value is required. The text specifies the enterprise custom field value for the resource.


> [!NOTE]
> The text value must match the data type required by the custom field definition.


## Remarks

The name of the XML element that stores the enterprise custom field value corresponds to the hexadecimal representation of the FieldID element.

Table 1 lists the valid range of custom field IDs for resource-level enterprise custom fields in both decimal and hexadecimal format.

Table 1. Resource-level enterprise custom field IDs

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Custom field ID range (decimal)</p></th>
<th><p>Custom field ID range (hexadecimal)</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>205553664 – 205619199</p></td>
<td><p>c408000 – c417fff</p></td>
</tr>
</tbody>
</table>

For more information, see [Custom Field Data in XML](bb968687\(v=office.12\).md).

## Example

The following example shows three different representations of enterprise resource custom field data.

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
<td><p>c408008</p></td>
<td><p>205553672</p></td>
<td><p>FieldName: ResourceNumberTest, a number custom field with a lookup table.</p>
<p>Guid: Refers to the custom field GUID.</p>
<p>DefaultGuid: Refers to the default value in the associated lookup table of the ResourceNumberTest custom field.</p>
<p>The GUID value of the c408008 element specifies the actual lookup table value.</p></td>
</tr>
<tr class="even">
<td><p>c40800b</p></td>
<td><p>205553675</p></td>
<td><p>FieldName: ResourceDateNL, a date custom field that has no lookup table.</p>
<p>The value of the custom field in the US English installation of Project Professional is &quot;Thu 11/8/07&quot; (Thursday, 8 November 2007).</p></td>
</tr>
<tr class="odd">
<td><p>c40800c</p></td>
<td><p>205553676</p></td>
<td><p>FieldName: ResourceDurationNL, a duration custom field that has no lookup table.</p>
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
         <FieldID>205553672</FieldID>
         <FieldName>ResourceNumberTest</FieldName>
         <CFType>5</CFType>
         <Guid>F570EA97-EE3E-4D5D-8444-B9DCDA75ADD0</Guid>
         <ElemType>21</ElemType>
         <MaxMultiValues>1</MaxMultiValues>
         <UserDef>1</UserDef>
         <SecondaryPID>255885332</SecondaryPID>
         <AutoRollDown>1</AutoRollDown>
         <DefaultGuid>EBDF240A-AE0B-4224-A8B8-3FA4B7EA709F</DefaultGuid>
      </ExtendedAttribute>
      <ExtendedAttribute>
         <FieldID>205553675</FieldID>
         <FieldName>ResourceDateNL</FieldName>
         <CFType>1</CFType>
         <Guid>303073AE-54FC-429B-9105-E9407E2BE7F2</Guid>
         <ElemType>21</ElemType>
         <MaxMultiValues>1</MaxMultiValues>
         <UserDef>1</UserDef>
         <SecondaryPID>255885335</SecondaryPID>
         <RollupType>0</RollupType>
         <CalculationType>1</CalculationType>
         <AutoRollDown>1</AutoRollDown>
      </ExtendedAttribute>
      <ExtendedAttribute>
         <FieldID>205553676</FieldID>
         <FieldName>ResourceDurationNL</FieldName>
         <CFType>2</CFType>
         <Guid>C7FFB2E7-9BA1-4A0D-97A8-8EFB8F0BD286</Guid>
         <ElemType>21</ElemType>
         <MaxMultiValues>1</MaxMultiValues>
         <UserDef>1</UserDef>
         <SecondaryPID>255885336</SecondaryPID>
         <RollupType>3</RollupType>
         <CalculationType>1</CalculationType>
         <AutoRollDown>1</AutoRollDown>
      </ExtendedAttribute>
   </ExtendedAttributes>
   . . .
   <Resources>
      <Resource>
         . . .
         <c408008>C0141D97-54F0-4CBD-97A6-48611227CD81</c408008>
         <c40800b>2007-11-08T08:00:00</c40800b>
         <c40800c DurationFormat="9">PT280H0M0S</c40800c>
         . . .
      </Resource>
   </Resources>
   . . .
</Project>
```

## See Also

#### Concepts

[Resource Elements and XML Structure](bb968445\(v=office.12\).md)

[XML Schema for the Resources Element](bb968511\(v=office.12\).md)

[Custom Field Data in XML](bb968687\(v=office.12\).md)

