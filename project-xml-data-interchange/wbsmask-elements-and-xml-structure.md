---
title: WBSMask Elements and XML Structure
TOCTitle: WBSMask Elements and XML Structure
ms:assetid: 101c3fa6-ccbf-4b34-ac5a-584c12fabbbd
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968416(v=office.12)
ms:contentKeyID: 13188109
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

# WBSMask Elements and XML Structure

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

This section contains information about children of the WBSMasks element defined in the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd). The XML elements represent work breakdown structure (WBS) code mask data when you save a project in the XML format.

WBSMasks is a child of the Project element. For more information, see [Project Elements and XML Structure](bb968439\(v=office.12\).md).

## XML Structure of WBSMasks Elements

The following shows the XML structure of the elements defined by the WBSMask schema section of mspdi\_pj12.xsd. The data type is indicated for those elements that require a text value. You can find more detailed information about valid text values for each element in the documentation annotations that are embedded in the [XML Schema for the Resources Element](bb968511\(v=office.12\).md).

For more information about the data types used in the Project 2007 XML Data Interchange Schema, see [Introduction to Project XML Data](bb968652\(v=office.12\).md).

\<[WBSMasks](bb968580\(v=office.12\).md)\>

    \<[VerifyUniqueCodes](bb968528\(v=office.12\).md)\>boolean\</VerifyUniqueCodes\>

    \<[GenerateCodes](bb968704\(v=office.12\).md)\>boolean\</GenerateCodes\>

    \<[Prefix](bb968516\(v=office.12\).md)\>string\<Prefix\>

    \<[WBSMask](bb968641\(v=office.12\).md)\>

        \<[Level](bb968635\(v=office.12\).md)\>integer\</Level\>

        \<[Type](bb968434\(v=office.12\).md)\>integer\</Type\>

        \<[Length](bb968526\(v=office.12\).md)\>string\</Length\>

        \<[Separator](bb968421\(v=office.12\).md)\>string\</Separator\>

    \</WBSMask\>

\</WBSMasks\>

## See Also

#### Concepts

[Introduction to Project XML Data](bb968652\(v=office.12\).md)

[XML Schema for the WBSMasks Element](bb968565\(v=office.12\).md)

[Project Elements and XML Structure](bb968439\(v=office.12\).md)

