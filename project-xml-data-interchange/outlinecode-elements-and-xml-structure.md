---
title: OutlineCode Elements and XML Structure
TOCTitle: OutlineCode Elements and XML Structure
ms:assetid: 9765ae1e-5f80-4932-a576-467833fbc42b
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968596(v=office.12)
ms:contentKeyID: 13188287
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

# OutlineCode Elements and XML Structure




This section contains information about children of the OutlineCodes element defined in the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd). The elements represent outline code data when you save a project in the XML format.

OutlineCodes is a child of the Project element. For more information, see [Project Elements and XML Structure](project-elements-and-xml-structure.md).

## XML Structure of OutlineCode Elements

The following shows the XML structure of the elements defined by the OutlineCode schema section of mspdi\_pj12.xsd. The data type is indicated for those elements that require a text value. You can find more detailed information about valid text values for each element in the documentation annotations that are embedded in the [XML Schema for the OutlineCodes Element](xml-schema-for-the-outlinecodes-element.md).

For more information on the data types used in the Project 2007 XML Data Interchange Schema, see [Introduction to Project XML Data](introduction-to-project-xml-data.md).

\<[OutlineCodes](outlinecodes-element.md)\>

    \<[OutlineCode](outlinecode-element.md)\>

        \<[Guid](guid-element-multiple-parents.md)\>string\</Guid\>

        \<[FieldID](fieldid-element.md)\>string\</FieldID\>

        \<[FieldName](fieldname-element.md)\>string\</FieldName\>

        \<[Alias](alias-element.md)\>string\</Alias\>

        \<[PhoneticAlias](phoneticalias-element.md)\>string\</PhoneticAlias\>

        \<[Values](values-element.md)\>

            \<[Value](value-element.md)\>

                \<[ValueID](valueid-element.md)\>integer\</ValueID\>

                \<[FieldGUID](fieldguid-element.md)\>string\</FieldGUID\>

                \<[Type](type-element-multiple-parents.md)\>integer\</Type\>

                \<[ParentValueID](parentvalueid-element.md)\>integer\</ParentValueID\>

                \<[Value](value-element.md)\>string\</Value\>

                \<[Description](description-element.md)\>string\</Description\>

            \</Value\>

        \</Values\>

        \<[Enterprise](enterprise-element.md)\>boolean\</Enterprise\>

        \<[EnterpriseOutlineCodeAlias](enterpriseoutlinecodealias-element.md)\>integer\</EnterpriseOutlineCodeAlias\>

        \<[ResourceSubstitutionEnabled](resourcesubstitutionenabled-element.md)\>boolean\</ResourceSubstitutionEnabled\>

        \<[LeafOnly](leafonly-element.md)\>boolean\</LeafOnly\>

        \<[AllLevelsRequired](alllevelsrequired-element.md)\>boolean\</AllLevelsRequired\>

        \<[OnlyTableValuesAllowed](onlytablevaluesallowed-element.md)\>boolean\</OnlyTableValuesAllowed\>

        \<[Masks](masks-element.md)\>

            \<[Mask](mask-element.md)\>

                \<[Level](level-element.md)\>integer\</Level\>

                \<[Type](type-element-multiple-parents.md)\>integer\</Type\>

                \<[Length](length-element.md)\>integer\</Length\>

                \<[Separator](separator-element.md)\>string\</Separator\>

            \</Mask\>

        \</Masks\>

    \</OutlineCode\>

\</OutlineCodes\>

## See Also

#### Concepts

[Introduction to Project XML Data](introduction-to-project-xml-data.md)

[XML Schema for the OutlineCodes Element](xml-schema-for-the-outlinecodes-element.md)

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

