---
title: ExtendedAttribute Elements and XML Structure
TOCTitle: ExtendedAttribute Elements and XML Structure
ms:assetid: 88acf5ad-cdb2-4fda-b178-ad43dc572684
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968579(v=office.12)
ms:contentKeyID: 13188270
ms.date: 03/14/2018
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




This section contains information about children of the ExtendedAttributes element defined in the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd). The XML elements in an ExtendedAttribute represent data for a custom field.

ExtendedAttributes is a child of the Project element. For more information, see [Project Elements and XML Structure](project-elements-and-xml-structure.md). A Task, Resource, or Assignment element can also contain individual ExtendedAttribute elements. For more information, see [Task Elements and XML Structure](task-elements-and-xml-structure.md), [Resource Elements and XML Structure](resource-elements-and-xml-structure.md), and [Assignment Elements and XML Structure](assignment-elements-and-xml-structure.md).

## XML Structure of ExtendedAttributes

The following shows the XML structure of the elements defined by the ExtendedAttribute schema section of mspdi\_pj12.xsd. The data type is indicated for those elements that require a text value. You can find more detailed information about valid text values for each element in the documentation annotations that are embedded in the [XML Schema for the ExtendedAttributes Element](xml-schema-for-the-extendedattributes-element.md).

For more information about the data types used in the Project 2007 XML Data Interchange Schema, see [Introduction to Project XML Data](introduction-to-project-xml-data.md).

\<[ExtendedAttributes](extendedattributes-element.md)\>

    \<[ExtendedAttribute](extendedattribute-element.md)\>

        \<[FieldID](fieldid-element.md)\>string\</FieldID\>

        \<[FieldName](fieldname-element.md)\>string\</FieldName\>

        \<[CFType](cftype-element.md)\>integer\</CFType\>

        \<[Guid](guid-element-multiple-parents.md)\>string\</Guid\>

        \<[ElemType](elemtype-element.md)\>integer\</ElemType\>

        \<[MaxMultiValues](maxmultivalues-element.md)\>integer\</MaxMultiValues\>

        \<[UserDef](userdef-element.md)\>boolean\</UserDef\>

        \<[Alias](alias-element.md)\>string\</Alias\>

        \<[SecondaryPID](secondarypid-element.md)\>string\</SecondaryPID\>

        \<[AutoRollDown](autorolldown-element.md)\>boolean\</AutoRollDown\>

        \<[DefaultGuid](defaultguid-element.md)\>string\</DefaultGuid\>

        \<[Ltuid](ltuid-element.md)\>string\</Ltuid\>

        \<[PhoneticAlias](phoneticalias-element.md)\>string\</PhoneticAlias\>

        \<[RollupType](rolluptype-element.md)\>integer\</RollupType\>

        \<[CalculationType](calculationtype-element.md)\>integer\</CalculationType\>

        \<[Formula](formula-element.md)\>string\</Formula\>

        \<[RestrictValues](restrictvalues-element.md)\>boolean\</RestrictValues\>

        \<[ValuelistSortOrder](valuelistsortorder-element.md)\>integer\</ValuelistSortOrder\>

        \<[AppendNewValues](appendnewvalues-element.md)\>boolean\</AppendNewValues\>

        \<[Default](default-element-extendedattribute.md)\>string\</Default\>

        \<[ValueList](valuelist-element.md)\>

            \<[Value](value-element.md)\>

                \<[ID](id-element.md)\>integer\</ID\>

                \<[Value](value-element.md)\>string\</Value\>

                \<[Description](description-element.md)\>string\</Description\>

                \<[Phonetic](phonetic-element.md)\>string\</Phonetic\>

            \</Value\>

        \</ValueList\>

    \</ExtendedAttribute\>

\</ExtendedAttributes\>

## See Also

#### Concepts

[Introduction to Project XML Data](introduction-to-project-xml-data.md)

[XML Schema for the ExtendedAttributes Element](xml-schema-for-the-extendedattributes-element.md)

[Custom Field Data in XML](custom-field-data-in-xml.md)

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[Resource Elements and XML Structure](resource-elements-and-xml-structure.md)

[Assignment Elements and XML Structure](assignment-elements-and-xml-structure.md)

