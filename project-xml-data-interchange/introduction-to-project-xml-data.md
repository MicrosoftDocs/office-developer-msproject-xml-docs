---
title: Introduction to Project XML Data
TOCTitle: Introduction to Project XML Data
ms:assetid: b4d72252-5b88-4244-b350-8f026c3e60cf
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968652(v=office.12)
ms:contentKeyID: 13188343
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- XML and Project
- XML in Project
- Project 2007, XML
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: high
---

# Introduction to Project XML Data




Microsoft Office Project 2007 can save and import project data in an XML file for exchanging data with other applications. The Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd) defines the XML elements used to represent Project 2007 data in XML format.

## In This Section

  - [Changes in the Project 2007 XML Data Interchange Schema](changes-in-the-project-2007-xml-data-interchange-schema.md) includes a list of new XML elements in Project 2007 and explains changes in XML data for custom fields.

  - [Working with Project XML Data Interchange Files](working-with-project-xml-data-interchange-files.md) explains how to save and open projects in XML format and shows how to use XSLT transformations to create reports with Project XML data.

  - [Project Data Interchange Elements](project-data-interchange-elements.md) includes an alphabetical list of elements and types and a reference for each main section of the Project 2007 XML Data Interchange Schema.

## Project Data Interchange Schema Reference Structure

The Project XML Data Interchange Schema Reference is structured into the following main sections:

  - [Project Elements and XML Structure](project-elements-and-xml-structure.md)

  - [OutlineCode Elements and XML Structure](outlinecode-elements-and-xml-structure.md)

  - [WBSMask Elements and XML Structure](wbsmask-elements-and-xml-structure.md)

  - [ExtendedAttribute Elements and XML Structure](extendedattribute-elements-and-xml-structure.md)

  - [Calendar Elements and XML Structure](calendar-elements-and-xml-structure.md)

  - [Task Elements and XML Structure](task-elements-and-xml-structure.md)

  - [Resource Elements and XML Structure](resource-elements-and-xml-structure.md)

  - [Assignment Elements and XML Structure](assignment-elements-and-xml-structure.md)

  - [TimephasedDataType Elements and XML Structure](timephaseddatatype-elements-and-xml-structure.md)

## Data Types

The XML elements defined in the Project Data Interchange Schema use the following data types for text values.

Table 1. Data types for text values

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Data Type</p></th>
<th><p>Data Format</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>boolean</p></td>
<td><p>A Boolean value. Valid values are <strong>true</strong> (1) and <strong>false</strong> (0).</p></td>
</tr>
<tr class="even">
<td><p>dateTime</p></td>
<td><p>Date and time data, provided in the format YYYY-MM-DDTHH:MM:SS.</p></td>
</tr>
<tr class="odd">
<td><p>decimal</p></td>
<td><p>An arbitrary precision number.</p></td>
</tr>
<tr class="even">
<td><p>duration</p></td>
<td><p>A duration of time, provided in the format PnYnMnDTnHnMnS where <em>n</em>Y represents the number of years, <em>n</em>M the number of months, <em>n</em>D the number of days, T the date/time separator, <em>n</em>H the number of hours, <em>n</em>M the number of minutes, and <em>n</em>S the number of seconds.</p>
<p>For example, to indicate a duration of 1 year, 2 months, 3 days, 10 hours, and 30 minutes, you write: P1Y2M3DT10H30M. You could also indicate a duration of minus 120 days as -P120D.</p></td>
</tr>
<tr class="odd">
<td><p>float</p></td>
<td><p>A single-precision, 32-bit floating point number.</p></td>
</tr>
<tr class="even">
<td><p>integer</p></td>
<td><p>A sequence of decimal digits with an optional leading sign (+ or -). This data type is derived from decimal.</p></td>
</tr>
<tr class="odd">
<td><p>string</p></td>
<td><p>A character string.</p></td>
</tr>
<tr class="even">
<td><p>time</p></td>
<td><p>Time data, provided in the format HH:MM:SS.</p></td>
</tr>
<tr class="odd">
<td><p>TimephasedDataType</p></td>
<td><p>A complex data type that contains information about a task, resource, or assignment that is distributed over time. The TimephasedData element is of this type.</p></td>
</tr>
</tbody>
</table>

## See Also

#### Concepts

[Project Data Interchange Elements](project-data-interchange-elements.md)

