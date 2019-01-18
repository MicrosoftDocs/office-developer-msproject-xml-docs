---
title: Project Data Interchange Elements
TOCTitle: Project Data Interchange Elements
ms:assetid: c0382453-e552-402c-be05-fa50af11e71d
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968664(v=office.12)
ms:contentKeyID: 13188355
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- XML and Project
- XML schema [Project 2007]
- Project XML elements
- Project 2007 XML
monikerRange: '>= project-client-2007 || project-client-odc'
localization_priority: Normal
---

# Project Data Interchange Elements




This section contains information about the elements defined by the Project XML Data Interchange Schema, as well as additional XML elements used by Microsoft Office Project 2007 to represent custom field values.

This topic includes the following sections:

  - Project Data Interchange XML Element Structure
    
      - General Element Structure
    
      - Detailed Element Structure

## Project Data Interchange XML Element Structure

The Project Data Interchange Schema is included in the Project 2007 SDK download. For a link to the Project 2007 SDK download, see [Welcome to the Microsoft Office Project 2007 SDK](https://msdn.microsoft.com/en-us/library/ms512767).

For a list of all elements in the schema, see [Alphabetical List of Elements and Types](alphabetical-list-of-elements-and-types.md).

Many elements in the Project Data Interchange Schema represent data fields in Microsoft Office Project Professional 2007. For more information about fields in Project Professional 2007 and Project Standard 2007, see [Fields Reference](http://office.microsoft.com/en-us/project/ch100788901033.aspx).

### General Element Structure

The following outline shows the high-level XML element structure of the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd). Links in the outline go to individual element descriptions. For the XML structure of each of the following elements, see Detailed Element Structure.

\<[Project](project-element.md)\>

    \<\!-- … additional child elements of Project --\>

    \<[OutlineCodes](outlinecodes-element.md)\> … \</OutlineCodes\>

    \<[WBSMasks](wbsmasks-element.md)\> … \</WBSMasks\>

    \<[ExtendedAttributes](extendedattributes-element.md)\> … \</ExtendedAttributes\>

    \<[Calendars](calendars-element.md)\> … \</Calendars\>

    \<[Tasks](tasks-element.md)\> … \</Tasks\>

    \<[Resources](resources-element.md)\> … \</Resources\>

    \<[Assignments](assignments-element.md)\> … \</Assignments\>

\</Project\>

### Detailed Element Structure

For details of the XML structure of each of the major elements, see the following topics:

  - [Project Elements and XML Structure](project-elements-and-xml-structure.md)

  - [OutlineCode Elements and XML Structure](outlinecode-elements-and-xml-structure.md)

  - [WBSMask Elements and XML Structure](wbsmask-elements-and-xml-structure.md)

  - [ExtendedAttribute Elements and XML Structure](extendedattribute-elements-and-xml-structure.md)

  - [Calendar Elements and XML Structure](calendar-elements-and-xml-structure.md)

  - [Task Elements and XML Structure](task-elements-and-xml-structure.md)

  - [Resource Elements and XML Structure](resource-elements-and-xml-structure.md)

  - [Assignment Elements and XML Structure](assignment-elements-and-xml-structure.md)

  - [TimephasedDataType Elements and XML Structure](timephaseddatatype-elements-and-xml-structure.md)

## See Also

#### Concepts

[Introduction to Project XML Data](introduction-to-project-xml-data.md)

#### Other Resources

[Changes in the Project 2007 XML Data Interchange Schema](changes-in-the-project-2007-xml-data-interchange-schema.md)

[Working with Project XML Data Interchange Files](working-with-project-xml-data-interchange-files.md)

[Fields Reference](http://office.microsoft.com/en-us/project/ch100788901033.aspx)

