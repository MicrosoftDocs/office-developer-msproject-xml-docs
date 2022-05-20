---
title: Custom Field Data in XML
TOCTitle: Custom Field Data in XML
ms:assetid: cb642a89-7686-441f-a9da-b3925a8612ea
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968687(v=office.12)
ms:contentKeyID: 13188377
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- XML and Project
- XML schema [Project 2007]
- Custom field XML data
- Custom field data
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# Custom Field Data in XML




The Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd) changes the way that some custom field information is represented in XML. This article describes how Office Project 2007 represents custom field definitions and custom field values in XML format.

## Custom Field Data

Project stores information about custom fields as one of two types:

  - **Custom field definition**  A custom field definition consists of data required to define a local or enterprise custom field. Project for the web local custom fields are presented as enterprise custom fields. This data includes information such as the custom field name, custom field ID, and custom field type.
    
    The XML elements that are used to store custom field definitions are defined in the [XML Schema for the ExtendedAttributes Element](xml-schema-for-the-extendedattributes-element.md) section of the Project XML Data Interchange Schema.

  - **Custom field value**  A custom field value is data required to define a particular value for a custom field and associate it with a project, task, resource, or assignment. For example, you can configure the Health enterprise custom field to the value Late for a particular task.

This article includes the following sections:

  - Custom Field Definitions in XML

  - Custom Field Values in XML

## Custom Field Definitions in XML

Project 2007 represents all enterprise and local custom field definitions in the extended attribute collection, which is contained within the ExtendedAttributes element in the XML output file. Each custom field definition is represented by a single ExtendedAttribute element and its children.

The following example shows the XML representation of an extended attribute collection that defines two custom fields. Text1 is a local custom field, while Health is an enterprise custom field that is preconfigured in Project 2007.

``` xml
<ExtendedAttributes>
    <ExtendedAttribute>
        <FieldID>188743731</FieldID>
        <FieldName>Text1</FieldName>
        <Alias>MyLocalCustomField</Alias>
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

When you save a project as XML, all local custom field definitions are written to the extended attributes collection. However, you can choose to include only the currently loaded enterprise custom fields in the XML output. Electing to save only the currently loaded enterprise global items can result in a smaller, more manageable XML file.

For more information about saving projects as XML, see [Saving and Opening Projects in XML Format](saving-and-opening-projects-in-xml-format.md).

## Custom Field Values in XML

When you configure a specific value for a custom field at the project, task, resource, or assignment level, Project 2007 writes information about that value to the summary task, task, resource, or assignment section of the XML output, respectively.

To represent a custom field value in XML, you must satisfy the following three requirements:

  - Associate the custom field value with the Project entity (project, task, resource, or assignment) that it is configured for.

  - Associate the custom field value with the custom field definition that it belongs to.

  - Specify the custom field value.

The following sections describe how Project 2007 represents custom field values in XML:

  - Enterprise Custom Field Values

  - Local Custom Field Values

### Enterprise Custom Field Values

In Project 2007 you can configure an unlimited number of enterprise custom fields. This enhancement changes the way that Project 2007 stores enterprise custom field values in XML.

The following example shows the relevant XML output for a task that has the Health enterprise custom field configured to the lookup table value On Schedule.

``` xml
    <Task>
        ...
        <b408001>0000BB21-B2AE-410A-88B6-82C108903823</b408001>
        ...
    </Task>
```

This XML satisfies the three requirements for storing a custom field value in XML as follows:

  - The custom field value is written to the summary task, task, resource, or assignment section of the XML output that the value is configured for. This associates the custom field value with the correct Project entity, in this case a particular task.

  - The custom field ID is used to link the custom field value to the custom field definition. The custom field ID is stored in the FieldID element in the custom field definition. For the Health enterprise custom field, the custom field ID is 188776449.
    
    The name of the XML element that stores the custom field value, in this case the b408001 element, corresponds to the hexadecimal representation of the custom field ID. For the Health enterprise custom field, the hexadecimal value 0xb408001 is equal to the binary value 188776449.

  - The custom field value is stored inside the b408001 element. Because the Health enterprise custom field is a lookup table, the custom field value for On Schedule is the GUID of that lookup table value, 0000BB21-B2AE-410A-88B6-82C108903823.

Table 1 shows the valid ranges of custom field IDs for each type of enterprise custom field.

Table 1. Enterprise custom field IDs

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Enterprise Custom Field Value Configuration</p></th>
<th><p>Custom Field ID Range (Decimal)</p></th>
<th><p>Custom Field ID Range (Hexadecimal)</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>Project level</p></td>
<td><p>190873600 – 190939135</p></td>
<td><p>b608000 – b617fff</p></td>
</tr>
<tr class="even">
<td><p>Task level</p></td>
<td><p>188776448 – 188841983</p></td>
<td><p>b408000 – b417fff</p></td>
</tr>
<tr class="odd">
<td><p>Resource level</p></td>
<td><p>205553664 – 205619199</p></td>
<td><p>c408000 – c417fff</p></td>
</tr>
<tr class="even">
<td><p>Assignment level</p></td>
<td><p>255885312 – 255950847</p></td>
<td><p>f408000 – f417fff</p></td>
</tr>
</tbody>
</table>

Because there are 262,140 possible enterprise custom field IDs, there are 262,140 possible XML element names for custom field values. For performance purposes, the XML elements that Project 2007 uses to store enterprise custom field values are not defined in the core Project XML Data Interchange Schema (mspdi\_pj12.xsd). Instead, these elements are defined in the supplemental schema files included in the Project 2007 SDK download. For a link to the Project 2007 SDK download, see [Welcome to the Microsoft Office Project 2007 SDK](https://msdn.microsoft.com/en-us/library/ms512767).

The core schema includes annotations with the searchable string "\#\#" to indicate the location to which Project 2007 writes the enterprise custom field value elements that are not defined in mspdi\_pj12.xsd.

### Local Custom Field Values

Project 2007 represents local custom field values in XML in one of two ways. Assignment local custom field values are written to XML in the same format used for enterprise custom field values, while project, task, and resource local custom field values are written to XML in the same format used by Microsoft Office Project 2003.

The following sections contain more detailed information about how local custom field values are represented in XML by Project 2007:

  - Assignment Local Custom Field Values in XML

  - Project, Task, and Resource Local Custom Field Values in XML

#### Assignment Local Custom Field Values in XML

Project 2007 writes assignment local custom field values using the same format as enterprise custom field values, and satisfies the three requirements for storing a custom field value in XML in the same way.

Table 2 shows the valid range of custom field IDs for assignment local custom fields. The mspdi\_pj12.xsd core schema defines the 200 possible XML elements for assignment local custom field values.

Table 2. Assignment local custom field IDs

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Local Custom Field Value Configuration</p></th>
<th><p>Custom Field ID Range (Decimal)</p></th>
<th><p>Custom Field ID Range (Hexadecimal)</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>Assignment level</p></td>
<td><p>255868928 – 255869128</p></td>
<td><p>f404000 – f4040c8</p></td>
</tr>
</tbody>
</table>

#### Project, Task, and Resource Local Custom Field Values in XML

Project 2007 writes project, task, and resource local custom field values in the format shown in the following example. This is the same format used by Project 2003 for all custom field values.

``` xml
    <Task>
        ...
        <ExtendedAttribute>
          <FieldID>188743731</FieldID>
          <Value>This is the value of Text1</Value>
        </ExtendedAttribute>
        ...
    </Task>
```

This XML satisfies the three requirements for storing a custom field value in XML as follows:

  - The custom field value is written to the summary task, task, resource, or assignment section of the XML output that the value is configured for. This associates the custom field value with the correct Project entity, in this case a particular task.

  - The custom field ID is used to link the custom field value to the custom field definition. The custom field ID is stored in the FieldID element in the XML representing both the custom field definition and the custom field value.

  - The custom field value is stored inside the Value element.

## See Also

#### Concepts

[Introduction to Project XML Data](introduction-to-project-xml-data.md)

[Project Data Interchange Elements](project-data-interchange-elements.md)

