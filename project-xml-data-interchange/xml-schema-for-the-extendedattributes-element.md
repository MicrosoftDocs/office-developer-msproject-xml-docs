---
title: XML Schema for the ExtendedAttributes Element
TOCTitle: XML Schema for the ExtendedAttributes Element
ms:assetid: db014a14-2934-4f15-8766-0ab0dd0add22
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968705(v=office.12)
ms:contentKeyID: 13188395
ms.date: 03/14/2018
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

# XML Schema for the ExtendedAttributes Element




The following shows the section of the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd) that defines the ExtendedAttributes element.

The complete Project Data Interchange Schema is included in the Project 2007 SDK download. For a link to the Project 2007 SDK download, see [Welcome to the Microsoft Office Project 2007 SDK](https://msdn.microsoft.com/en-us/library/ms512767).

## ExtendedAttributes Schema

``` xml
<?xml version="1.0" encoding="utf-8"?>
. . .
<!-- @ExtendedAttribute schema -->
<xsd:element name="ExtendedAttributes" minOccurs="0">
  <xsd:annotation>
    <xsd:documentation>The collection of extended attribute (custom field) definitions associated with the project.</xsd:documentation>
  </xsd:annotation>
  <xsd:complexType>
    <xsd:sequence>
      <xsd:element name="ExtendedAttribute" minOccurs="0" maxOccurs="unbounded">
        <xsd:annotation>
          <xsd:documentation>Each of the individual entries in the extended attributes definition collection.  There are no limits to the number of children that may appear, but Project only understands Flag1-Flag10, etc.  There must be at least one ExtendedAttribute in each ExtendedAttributes collection.</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="FieldID" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>This corresponds to the PID of the custom field.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="FieldName" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The name of the custom field.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="CFType" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The custom field type. Values are: 0=Cost, 1=Date, 2=Duration, 3=Finish, 4=Flag, 5=Number, 6=Start, 7=Text.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:integer">
                  <xsd:enumeration value="0" />
                  <xsd:enumeration value="1" />
                  <xsd:enumeration value="2" />
                  <xsd:enumeration value="3" />
                  <xsd:enumeration value="4" />
                  <xsd:enumeration value="5" />
                  <xsd:enumeration value="6" />
                  <xsd:enumeration value="7" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="Guid" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The GUID of the custom field.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ElemType" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Specifies whether the extended attribute is associated with a task, a resource, or an assignment. Values are: 20=Task, 21=Resource, 22=Calendar, 23=Assignment.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:integer">
                  <xsd:enumeration value="20" />
                  <xsd:enumeration value="21" />
                  <xsd:enumeration value="22" />
                  <xsd:enumeration value="23" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="MaxMultiValues" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Specifies the maximum number of values you can set in a picklist.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="UserDef" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Specifies whether the custom field is user-defined.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Alias" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The alias of the custom field.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="50" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="SecondaryPID" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The secondary PID of the custom field.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="AutoRollDown" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Specifies whether automatic rolldown to assignments is enabled.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="DefaultGuid" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Specifies the GUID of the default lookup table entry.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Ltuid" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The GUID of the lookup table associated with the custom field.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="PhoneticAlias" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The phonetic pronunciation of the alias of the custom field.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="50" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="RollupType" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>How rollups are calculated. Values are: 0=Maximum (OR for flag fields), 1=Minimum (AND for flag fields), 2=Count all, 3=Sum, 4=Average, 5=Average First Sublevel, 6=Count First Sublevel, 7=Count Nonsummaries.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:integer">
                  <xsd:enumeration value="0" />
                  <xsd:enumeration value="1" />
                  <xsd:enumeration value="2" />
                  <xsd:enumeration value="3" />
                  <xsd:enumeration value="4" />
                  <xsd:enumeration value="5" />
                  <xsd:enumeration value="6" />
                  <xsd:enumeration value="7" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="CalculationType" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether rollups are calculated for task and group summary rows. Values are: 0=None, 1=Rollup, 2=Calculation.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:integer">
                  <xsd:enumeration value="0" />
                  <xsd:enumeration value="1" />
                  <xsd:enumeration value="2" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="Formula" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The formula that Microsoft Project uses to populate the custom task field.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="RestrictValues" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>If RestrictValues=True then only values in the list are allowed in the file.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ValuelistSortOrder" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>How value lists are sorted. Values are: 0=Descending, 1=Ascending.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:integer">
                  <xsd:enumeration value="0" />
                  <xsd:enumeration value="1" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="AppendNewValues" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>If AppendNewValues=True then any new values added in a project are automatically appended to the list.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Default" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>This points to the default value in the list.  Not present if no default is set.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ValueList" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>When values of extended attributes are specified as properties of elements in the schema, they can be specified either by values or by references to the values contained in this list.  Applications can assume ordering of the list by ordering specified here.</xsd:documentation>
              </xsd:annotation>
              <xsd:complexType>
                <xsd:sequence>
                  <xsd:element name="Value" maxOccurs="unbounded">
                    <xsd:annotation>
                      <xsd:documentation>The values that make up the value list.</xsd:documentation>
                    </xsd:annotation>
                    <xsd:complexType>
                      <xsd:all>
                        <xsd:element name="ID" type="xsd:integer">
                          <xsd:annotation>
                            <xsd:documentation>Unique ID of value across the project.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <xsd:element name="Value" type="xsd:string" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The actual value.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <xsd:element name="Description" type="xsd:string" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The description of the value in the list.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <xsd:element name="Phonetic" type="xsd:string" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>Phonetic information for custom field names.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                      </xsd:all>
                    </xsd:complexType>
                  </xsd:element>
                </xsd:sequence>
              </xsd:complexType>
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

[ExtendedAttribute Elements and XML Structure](extendedattribute-elements-and-xml-structure.md)

[Custom Field Data in XML](custom-field-data-in-xml.md)

