---
title: ExtendedAttribute Elements and XML Structure
TOCTitle: ExtendedAttribute Elements and XML Structure
ms:assetid: 88acf5ad-cdb2-4fda-b178-ad43dc572684
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968579(v=office.12)
ms:contentKeyID: 13188270
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

# ExtendedAttribute Elements and XML Structure

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

This section contains information about children of the ExtendedAttributes element defined in the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd). The XML elements in an ExtendedAttribute represent data for a custom field.

ExtendedAttributes is a child of the Project element. For more information, see [Project Elements and XML Structure](bb968439\(v=office.12\).md). A Task, Resource, or Assignment element can also contain individual ExtendedAttribute elements. For more information, see [Task Elements and XML Structure](bb968475\(v=office.12\).md), [Resource Elements and XML Structure](bb968445\(v=office.12\).md), and [Assignment Elements and XML Structure](bb968738\(v=office.12\).md).

## XML Structure of ExtendedAttributes

The following shows the XML structure of the elements defined by the ExtendedAttribute schema section of mspdi\_pj12.xsd. The data type is indicated for those elements that require a text value. You can find more detailed information about valid text values for each element in the documentation annotations that are embedded in the [XML Schema for the ExtendedAttributes Element](bb968705\(v=office.12\).md).

For more information about the data types used in the Project 2007 XML Data Interchange Schema, see [Introduction to Project XML Data](bb968652\(v=office.12\).md).

\<[ExtendedAttributes](bb968426\(v=office.12\).md)\>

    \<[ExtendedAttribute](bb968669\(v=office.12\).md)\>

        \<[FieldID](bb968474\(v=office.12\).md)\>string\</FieldID\>

        \<[FieldName](bb968619\(v=office.12\).md)\>string\</FieldName\>

        \<[CFType](bb968675\(v=office.12\).md)\>integer\</CFType\>

        \<[Guid](bb968441\(v=office.12\).md)\>string\</Guid\>

        \<[ElemType](bb968655\(v=office.12\).md)\>integer\</ElemType\>

        \<[MaxMultiValues](bb968512\(v=office.12\).md)\>integer\</MaxMultiValues\>

        \<[UserDef](bb968649\(v=office.12\).md)\>boolean\</UserDef\>

        \<[Alias](bb968395\(v=office.12\).md)\>string\</Alias\>

        \<[SecondaryPID](bb968460\(v=office.12\).md)\>string\</SecondaryPID\>

        \<[AutoRollDown](bb968428\(v=office.12\).md)\>boolean\</AutoRollDown\>

        \<[DefaultGuid](bb968436\(v=office.12\).md)\>string\</DefaultGuid\>

        \<[Ltuid](bb968607\(v=office.12\).md)\>string\</Ltuid\>

        \<[PhoneticAlias](bb968672\(v=office.12\).md)\>string\</PhoneticAlias\>

        \<[RollupType](bb968480\(v=office.12\).md)\>integer\</RollupType\>

        \<[CalculationType](bb968490\(v=office.12\).md)\>integer\</CalculationType\>

        \<[Formula](bb968523\(v=office.12\).md)\>string\</Formula\>

        \<[RestrictValues](bb968626\(v=office.12\).md)\>boolean\</RestrictValues\>

        \<[ValuelistSortOrder](bb968427\(v=office.12\).md)\>integer\</ValuelistSortOrder\>

        \<[AppendNewValues](bb968723\(v=office.12\).md)\>boolean\</AppendNewValues\>

        \<[Default](bb968745\(v=office.12\).md)\>string\</Default\>

        \<[ValueList](bb968702\(v=office.12\).md)\>

            \<[Value](bb968696\(v=office.12\).md)\>

                \<[ID](bb968437\(v=office.12\).md)\>integer\</ID\>

                \<[Value](bb968696\(v=office.12\).md)\>string\</Value\>

                \<[Description](bb968567\(v=office.12\).md)\>string\</Description\>

                \<[Phonetic](bb968486\(v=office.12\).md)\>string\</Phonetic\>

            \</Value\>

        \</ValueList\>

    \</ExtendedAttribute\>

\</ExtendedAttributes\>

## See Also

#### Concepts

[Introduction to Project XML Data](bb968652\(v=office.12\).md)

[XML Schema for the ExtendedAttributes Element](bb968705\(v=office.12\).md)

[Custom Field Data in XML](bb968687\(v=office.12\).md)

[Project Elements and XML Structure](bb968439\(v=office.12\).md)

[Task Elements and XML Structure](bb968475\(v=office.12\).md)

[Resource Elements and XML Structure](bb968445\(v=office.12\).md)

[Assignment Elements and XML Structure](bb968738\(v=office.12\).md)

