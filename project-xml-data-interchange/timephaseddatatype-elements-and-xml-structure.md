---
title: TimephasedDataType Elements and XML Structure
TOCTitle: TimephasedDataType Elements and XML Structure
ms:assetid: ed317823-7111-4dfd-ae38-50a06c6cb70f
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968722(v=office.12)
ms:contentKeyID: 13188412
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- XML and Project
- XML in Project
- XML structure in Project
- Project and XML
- Project XML elements
- Project 2007 XML
- Project XML structure
monikerRange: '>= project-client-2007 || project-client-odc'
---

# TimephasedDataType Elements and XML Structure

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

This section contains information about elements in the TimephasedDataType complex type defined in the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd). The TimephasedData element is of type TimephasedDataType that represents timephased data, for example, the number of hours of work per day over a period of days. Task, Resource, Assignment, and Baseline elements can include TimephasedData.

## XML Structure of TimephasedData Elements

The following shows the XML structure of the elements defined by the TimephasedDataType schema section of mspdi\_pj12.xsd. The data type is indicated for those elements that require a text value. You can find more detailed information about valid text values for each element in the documentation annotations that are embedded in the [XML Schema for the TimephasedDataType Complex Type](bb968734\(v=office.12\).md).

\<[TimephasedData](bb968479\(v=office.12\).md)\>

    \<[Type](bb968434\(v=office.12\).md)\>integer\</Type\>

    \<[UID](bb968590\(v=office.12\).md)\>integer\</UID\>

    \<[Start](bb968645\(v=office.12\).md) \>dateTime\</Start\>

    \<[Finish](bb968534\(v=office.12\).md)\>dateTime\</Finish\>

    \<[Unit](bb968545\(v=office.12\).md)\>integer\</Unit\>

    \<[Value](bb968696\(v=office.12\).md)\>string\</Value\>

\</TimephasedData\>

For more information about the data types used in the Project 2007 XML Data Interchange Schema, see [Introduction to Project XML Data](bb968652\(v=office.12\).md).

## See Also

#### Reference

[Baseline Element](bb968599\(v=office.12\).md)

#### Concepts

[XML Schema for the TimephasedDataType Complex Type](bb968734\(v=office.12\).md)

[Task Elements and XML Structure](bb968475\(v=office.12\).md)

[Resource Elements and XML Structure](bb968445\(v=office.12\).md)

[Assignment Elements and XML Structure](bb968738\(v=office.12\).md)

