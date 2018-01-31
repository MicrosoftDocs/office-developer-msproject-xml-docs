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
---

# OutlineCode Elements and XML Structure

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

This section contains information about children of the OutlineCodes element defined in the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd). The elements represent outline code data when you save a project in the XML format.

OutlineCodes is a child of the Project element. For more information, see [Project Elements and XML Structure](bb968439\(v=office.12\).md).

## XML Structure of OutlineCode Elements

The following shows the XML structure of the elements defined by the OutlineCode schema section of mspdi\_pj12.xsd. The data type is indicated for those elements that require a text value. You can find more detailed information about valid text values for each element in the documentation annotations that are embedded in the [XML Schema for the OutlineCodes Element](bb968584\(v=office.12\).md).

For more information on the data types used in the Project 2007 XML Data Interchange Schema, see [Introduction to Project XML Data](bb968652\(v=office.12\).md).

\<[OutlineCodes](bb968732\(v=office.12\).md)\>

    \<[OutlineCode](bb968410\(v=office.12\).md)\>

        \<[Guid](bb968441\(v=office.12\).md)\>string\</Guid\>

        \<[FieldID](bb968474\(v=office.12\).md)\>string\</FieldID\>

        \<[FieldName](bb968619\(v=office.12\).md)\>string\</FieldName\>

        \<[Alias](bb968395\(v=office.12\).md)\>string\</Alias\>

        \<[PhoneticAlias](bb968672\(v=office.12\).md)\>string\</PhoneticAlias\>

        \<[Values](bb968604\(v=office.12\).md)\>

            \<[Value](bb968696\(v=office.12\).md)\>

                \<[ValueID](bb968406\(v=office.12\).md)\>integer\</ValueID\>

                \<[FieldGUID](bb968634\(v=office.12\).md)\>string\</FieldGUID\>

                \<[Type](bb968434\(v=office.12\).md)\>integer\</Type\>

                \<[ParentValueID](bb968739\(v=office.12\).md)\>integer\</ParentValueID\>

                \<[Value](bb968696\(v=office.12\).md)\>string\</Value\>

                \<[Description](bb968567\(v=office.12\).md)\>string\</Description\>

            \</Value\>

        \</Values\>

        \<[Enterprise](bb968519\(v=office.12\).md)\>boolean\</Enterprise\>

        \<[EnterpriseOutlineCodeAlias](bb968491\(v=office.12\).md)\>integer\</EnterpriseOutlineCodeAlias\>

        \<[ResourceSubstitutionEnabled](bb968443\(v=office.12\).md)\>boolean\</ResourceSubstitutionEnabled\>

        \<[LeafOnly](bb968419\(v=office.12\).md)\>boolean\</LeafOnly\>

        \<[AllLevelsRequired](bb968417\(v=office.12\).md)\>boolean\</AllLevelsRequired\>

        \<[OnlyTableValuesAllowed](bb968454\(v=office.12\).md)\>boolean\</OnlyTableValuesAllowed\>

        \<[Masks](bb968478\(v=office.12\).md)\>

            \<[Mask](bb968659\(v=office.12\).md)\>

                \<[Level](bb968635\(v=office.12\).md)\>integer\</Level\>

                \<[Type](bb968434\(v=office.12\).md)\>integer\</Type\>

                \<[Length](bb968526\(v=office.12\).md)\>integer\</Length\>

                \<[Separator](bb968421\(v=office.12\).md)\>string\</Separator\>

            \</Mask\>

        \</Masks\>

    \</OutlineCode\>

\</OutlineCodes\>

## See Also

#### Concepts

[Introduction to Project XML Data](bb968652\(v=office.12\).md)

[XML Schema for the OutlineCodes Element](bb968584\(v=office.12\).md)

[Project Elements and XML Structure](bb968439\(v=office.12\).md)

