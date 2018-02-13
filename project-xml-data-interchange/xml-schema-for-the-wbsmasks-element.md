---
title: XML Schema for the WBSMasks Element
TOCTitle: XML Schema for the WBSMasks Element
ms:assetid: 822ec84d-c92a-419d-a0bf-905f5d1da8cc
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968565(v=office.12)
ms:contentKeyID: 13188256
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- Schemas [Project 2007]
- XML and Project
- XML schema [Project 2007]
- Project schema
- Project XML schema
- XML in Project
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# XML Schema for the WBSMasks Element




The following shows the section of the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd) that defines the WBSMasks element.

The complete Project XML Data Interchange Schema is included in the Project 2007 SDK download. For a link to the Project 2007 SDK download, see [Welcome to the Microsoft Office Project 2007 SDK](https://msdn.microsoft.com/en-us/library/ms512767).

## WBSMasks Schema

``` xml
<?xml version="1.0" encoding="utf-8"?>
. . .
<!-- @WBSMask schema -->
<xsd:element name="WBSMasks" minOccurs="0">
  <xsd:annotation>
    <xsd:documentation>The table of entries that define the outline code mask.</xsd:documentation>
  </xsd:annotation>
  <xsd:complexType>
    <xsd:sequence>
      <xsd:element name="VerifyUniqueCodes" type="xsd:boolean" default="false" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation>Whether work breakdown structure (WBS) codes are unique for new tasks.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="GenerateCodes" type="xsd:boolean" default="false" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation>Whether WBS codes are generated for new tasks.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="Prefix" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation>The prefix for all WBS codes.</xsd:documentation>
        </xsd:annotation>
        <xsd:simpleType>
          <xsd:restriction base="xsd:string">
            <xsd:maxLength value="50" />
          </xsd:restriction>
        </xsd:simpleType>
      </xsd:element>
      <xsd:element name="WBSMask" minOccurs="0" maxOccurs="unbounded">
        <xsd:annotation>
          <xsd:documentation>The WBS mask that is applied to all tasks in the project.</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="Level" type="xsd:integer">
              <xsd:annotation>
                <xsd:documentation>The level of the mask.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Type">
              <xsd:annotation>
                <xsd:documentation>The type of the node value.  The values are: 0=Numbers, 1=Uppercase Letters, 2=Lowercase Letters, 3=Characters.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:integer">
                  <xsd:enumeration value="0" />
                  <xsd:enumeration value="1" />
                  <xsd:enumeration value="2" />
                  <xsd:enumeration value="3" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="Length" type="xsd:string">
              <xsd:annotation>
                <xsd:documentation>The maximum length in characters.  This element is omitted when length is "any".</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Separator" type="xsd:string">
              <xsd:annotation>
                <xsd:documentation>The separator character of the node.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
</xsd:element>
```

## See Also

#### Concepts

[WBSMask Elements and XML Structure](bb968416\(v=office.12\).md)

