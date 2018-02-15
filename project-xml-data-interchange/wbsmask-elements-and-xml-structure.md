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




This section contains information about children of the WBSMasks element defined in the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd). The XML elements represent work breakdown structure (WBS) code mask data when you save a project in the XML format.

WBSMasks is a child of the Project element. For more information, see [Project Elements and XML Structure](project-elements-and-xml-structure.md).

## XML Structure of WBSMasks Elements

The following shows the XML structure of the elements defined by the WBSMask schema section of mspdi\_pj12.xsd. The data type is indicated for those elements that require a text value. You can find more detailed information about valid text values for each element in the documentation annotations that are embedded in the [XML Schema for the Resources Element](xml-schema-for-the-resources-element.md).

For more information about the data types used in the Project 2007 XML Data Interchange Schema, see [Introduction to Project XML Data](introduction-to-project-xml-data.md).

\<[WBSMasks](wbsmasks-element.md)\>

    \<[VerifyUniqueCodes](verifyuniquecodes-element.md)\>boolean\</VerifyUniqueCodes\>

    \<[GenerateCodes](generatecodes-element.md)\>boolean\</GenerateCodes\>

    \<[Prefix](prefix-element.md)\>string\<Prefix\>

    \<[WBSMask](wbsmask-element.md)\>

        \<[Level](level-element.md)\>integer\</Level\>

        \<[Type](type-element-multiple-parents.md)\>integer\</Type\>

        \<[Length](length-element.md)\>string\</Length\>

        \<[Separator](separator-element.md)\>string\</Separator\>

    \</WBSMask\>

\</WBSMasks\>

## See Also

#### Concepts

[Introduction to Project XML Data](introduction-to-project-xml-data.md)

[XML Schema for the WBSMasks Element](xml-schema-for-the-wbsmasks-element.md)

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

