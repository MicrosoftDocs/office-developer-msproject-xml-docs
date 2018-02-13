---
title: Project Data Interchange Elements
TOCTitle: Project Data Interchange Elements
ms:assetid: c0382453-e552-402c-be05-fa50af11e71d
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968664(v=office.12)
ms:contentKeyID: 13188355
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- XML and Project
- XML schema [Project 2007]
- Project XML elements
- Project 2007 XML
monikerRange: '>= project-client-2007 || project-client-odc'
---

# Project Data Interchange Elements

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

This section contains information about the elements defined by the Project XML Data Interchange Schema, as well as additional XML elements used by Microsoft Office Project 2007 to represent custom field values.

This topic includes the following sections:

  - Project Data Interchange XML Element Structure
    
      - General Element Structure
    
      - Detailed Element Structure

## Project Data Interchange XML Element Structure

The Project Data Interchange Schema is included in the Project 2007 SDK download. For a link to the Project 2007 SDK download, see [Welcome to the Microsoft Office Project 2007 SDK](https://msdn.microsoft.com/en-us/library/ms512767).

For a list of all elements in the schema, see [Alphabetical List of Elements and Types](bb968673\(v=office.12\).md).

Many elements in the Project Data Interchange Schema represent data fields in Microsoft Office Project Professional 2007. For more information about fields in Project Professional 2007 and Project Standard 2007, see [Fields Reference](http://office.microsoft.com/en-us/project/ch100788901033.aspx).

### General Element Structure

The following outline shows the high-level XML element structure of the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd). Links in the outline go to individual element descriptions. For the XML structure of each of the following elements, see Detailed Element Structure.

\<[Project](bb968701\(v=office.12\).md)\>

    \<\!-- … additional child elements of Project --\>

    \<[OutlineCodes](bb968732\(v=office.12\).md)\> … \</OutlineCodes\>

    \<[WBSMasks](bb968580\(v=office.12\).md)\> … \</WBSMasks\>

    \<[ExtendedAttributes](bb968426\(v=office.12\).md)\> … \</ExtendedAttributes\>

    \<[Calendars](bb968499\(v=office.12\).md)\> … \</Calendars\>

    \<[Tasks](bb968617\(v=office.12\).md)\> … \</Tasks\>

    \<[Resources](bb968730\(v=office.12\).md)\> … \</Resources\>

    \<[Assignments](bb968684\(v=office.12\).md)\> … \</Assignments\>

\</Project\>

### Detailed Element Structure

For details of the XML structure of each of the major elements, see the following topics:

  - [Project Elements and XML Structure](bb968439\(v=office.12\).md)

  - [OutlineCode Elements and XML Structure](bb968596\(v=office.12\).md)

  - [WBSMask Elements and XML Structure](bb968416\(v=office.12\).md)

  - [ExtendedAttribute Elements and XML Structure](bb968579\(v=office.12\).md)

  - [Calendar Elements and XML Structure](bb968563\(v=office.12\).md)

  - [Task Elements and XML Structure](bb968475\(v=office.12\).md)

  - [Resource Elements and XML Structure](bb968445\(v=office.12\).md)

  - [Assignment Elements and XML Structure](bb968738\(v=office.12\).md)

  - [TimephasedDataType Elements and XML Structure](bb968722\(v=office.12\).md)

## See Also

#### Concepts

[Introduction to Project XML Data](bb968652\(v=office.12\).md)

#### Other Resources

[Changes in the Project 2007 XML Data Interchange Schema](bb968543\(v=office.12\).md)

[Working with Project XML Data Interchange Files](bb968469\(v=office.12\).md)

[Fields Reference](http://office.microsoft.com/en-us/project/ch100788901033.aspx)

