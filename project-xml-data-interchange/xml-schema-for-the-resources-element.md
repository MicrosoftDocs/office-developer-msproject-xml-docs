---
title: XML Schema for the Resources Element
TOCTitle: XML Schema for the Resources Element
ms:assetid: 56a91683-2a3e-4879-a0ef-dcb7918c4965
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968511(v=office.12)
ms:contentKeyID: 13188203
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

# XML Schema for the Resources Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

The following shows the section of the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd) that defines the Resources element.

The complete Project XML Data Interchange Schema is included in the Project 2007 SDK download. For a link to the Project 2007 SDK download, see [Welcome to the Microsoft Office Project 2007 SDK](https://msdn.microsoft.com/en-us/library/ms512767).

## Resources Schema

``` xml
<?xml version="1.0" encoding="utf-8"?>
. . .
<!-- @Resource schema -->
<xsd:element name="Resources" minOccurs="0">
  <xsd:annotation>
    <xsd:documentation>The collection of resources that make up the project.</xsd:documentation>
  </xsd:annotation>
  <xsd:complexType>
    <xsd:sequence>
      <xsd:element name="Resource" minOccurs="0" maxOccurs="unbounded">
        <xsd:annotation>
          <xsd:documentation>There must be at least one resource in each Resources collection.</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="UID" type="xsd:integer">
              <xsd:annotation>
                <xsd:documentation>The unique identifier of the resource.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ID" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The position identifier of the resource within the list of resources.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Name" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The name of the resource.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="512" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="Type" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The type of resource. Values are: 0=Material, 1=Work.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:integer">
                  <xsd:enumeration value="0" />
                  <xsd:enumeration value="1" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="IsNull" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Specifies whether the resource is null.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Initials" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The initials of the resource.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="512" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="Phonetics" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The phonetic spelling of the resource name.  For use with Japanese only.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="512" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="NTAccount" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The NT account associated with the resource.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="512" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="MaterialLabel" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The unit of measure for the material resource.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="512" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="Code" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The code or other information about the resource.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="512" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="Group" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The group to which the resource belongs.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="512" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="WorkGroup" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The type of workgroup to which the resource belongs. Values are: 0=Default, 1=None, 2=Email, 3=Web.</xsd:documentation>
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
            <xsd:element name="EmailAddress" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The e-mail address of the resource.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="512" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="Hyperlink" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The title of the hyperlink associated with the resource.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="512" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="HyperlinkAddress" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The hyperlink associated with the resource.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="512" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="HyperlinkSubAddress" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The document bookmark of the hyperlink associated with the resource.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="512" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="MaxUnits" type="xsd:float" default="1.0" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The maximum number of units that the resource is available.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="PeakUnits" type="xsd:float" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The largest number of units assigned to the resource at any time.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="OverAllocated" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether the resource is overallocated.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="AvailableFrom" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The first date that the resource is available.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="AvailableTo" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The last date the resource is available.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Start" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The scheduled start date of the resource.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Finish" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The scheduled finish date of the resource.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="CanLevel" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether the resource can be leveled.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="AccrueAt" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>How cost is accrued against the resource. Values are: 1=Start, 2=End, 3=Prorated, $New4=Invalid.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:integer">
                  <xsd:enumeration value="1" />
                  <xsd:enumeration value="2" />
                  <xsd:enumeration value="3" />
                  <xsd:enumeration value="4" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="Work" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The total work assigned to the resource across all assigned tasks.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="RegularWork" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The amount of non-overtime work assigned to the resource.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="OvertimeWork" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The amount of overtime work assigned to the resource.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ActualWork" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The amount of actual work performed by the resource.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="RemainingWork" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The amount of remaining work required to complete all assigned tasks.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ActualOvertimeWork" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The amount of actual overtime work performed by the resource.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="RemainingOvertimeWork" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The amount of remaining overtime work required to complete all tasks.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="PercentWorkComplete" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The percentage of work completed across all tasks.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="StandardRate" type="xsd:decimal" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The standard rate of the resource. This value is as of the current date if a rate table exists for the resource.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="StandardRateFormat" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The units used by Microsoft Office Project to display the standard rate.  1=m, 2=h, 3=d, 4=w, 5=mo, 7=y, 8=material resource rate (or blank symbol specified).</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:integer">
                  <xsd:enumeration value="1" />
                  <xsd:enumeration value="2" />
                  <xsd:enumeration value="3" />
                  <xsd:enumeration value="4" />
                  <xsd:enumeration value="5" />
                  <xsd:enumeration value="7" />
                  <xsd:enumeration value="8" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="Cost" type="xsd:decimal" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The total project cost for the resource across all assigned tasks.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="OvertimeRate" type="xsd:decimal" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The overtime rate of the resource. This value is as of the current date if a rate table exists for the resource.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="OvertimeRateFormat" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The units used by Microsoft Office Project to display the overtime rate.  1=m, 2=h, 3=d, 4=w, 5=mo, 7=y.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:integer">
                  <xsd:enumeration value="1" />
                  <xsd:enumeration value="2" />
                  <xsd:enumeration value="3" />
                  <xsd:enumeration value="4" />
                  <xsd:enumeration value="5" />
                  <xsd:enumeration value="7" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="OvertimeCost" type="xsd:decimal" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The total overtime cost for the resource including actual and remaining overtime costs.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="CostPerUse" type="xsd:decimal" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The cost per use of the resource. This value is as of the current date if a rate table exists for the resource.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ActualCost" type="xsd:decimal" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The actual cost incurred by the resource across all assigned tasks.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ActualOvertimeCost" type="xsd:decimal" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The actual overtime cost incurred by the resource across all assigned tasks.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="RemainingCost" type="xsd:decimal" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The remaining projected cost of the resource to complete all assigned tasks.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="RemainingOvertimeCost" type="xsd:decimal" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The remaining projected overtime cost of the resource to complete all assigned tasks.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="WorkVariance" type="xsd:float" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The difference between the baseline work and the work as minutes x 1000.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="CostVariance" type="xsd:float" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The difference between the baseline cost and the cost.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="SV" type="xsd:float" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Earned value schedule variance, through the project status date.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="CV" type="xsd:float" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Earned value cost variance, through the project status date.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ACWP" type="xsd:float" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The actual cost of the work performed by the resource for the project to date.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="CalendarUID" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The resource calendar. Refers to a valid UID in the Calendars element of the Microsoft Office Project 2007 XML Schema.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Notes" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Text notes associated with the resource.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="BCWS" type="xsd:float" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The budget cost of work scheduled for the resource.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="BCWP" type="xsd:float" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The budgeted cost of of the work performed by the resource for the project to date.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="IsGeneric" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Specifies whether the resource is generic.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="IsInactive" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Specifies whether the resource is set to inactive.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="IsEnterprise" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Specifies whether the resource is an Enterprise resource.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="BookingType" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Specifies the booking type of the resource. 1=Commited, 2=Proposed.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:integer">
                  <xsd:enumeration value="0" />
                  <xsd:enumeration value="1" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="ActualWorkProtected" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Specifies the duration through which actual work is protected.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ActualOvertimeWorkProtected" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Specifies the duration through which actual overtime work is protected.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ActiveDirectoryGUID" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The Active Directory GUID for the resource.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="16" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="CreationDate" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The date that the resource was created.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ExtendedAttribute" minOccurs="0" maxOccurs="unbounded">
              <xsd:annotation>
                <xsd:documentation>The value of an extended attribute. Two pieces of data are needed: a pointer back to the extended attribute table that is specified either by the unique ID or the Field ID, and the value that is specified either with the value, or a pointer back to the value list.</xsd:documentation>
              </xsd:annotation>
              <xsd:complexType>
                <xsd:sequence>
                  <xsd:element name="FieldID" type="xsd:string" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The project ID (PID) of the custom field.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="Value" type="xsd:string" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The actual value of the extended attribute.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="ValueGUID" type="xsd:string" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The GUID of the value in the extended attribute lookup table.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="DurationFormat" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The format for expressing the bulk duration.  Values are: 3=m, 4=em, 5=h, 6=eh, 7=d, 8=ed, 9=w, 10=ew, 11=mo, 12=emo, 19=%, 20=e%, 21=null, 35=m?, 36=em?, 37=h?, 38=eh?, 39=d?, 40=ed?, 41=w?, 42=ew?, 43=mo?, 44=emo?, 51=%?, 52=e%? and 53=null.</xsd:documentation>
                    </xsd:annotation>
                    <xsd:simpleType>
                      <xsd:restriction base="xsd:integer">
                        <xsd:enumeration value="3" />
                        <xsd:enumeration value="4" />
                        <xsd:enumeration value="5" />
                        <xsd:enumeration value="6" />
                        <xsd:enumeration value="7" />
                        <xsd:enumeration value="8" />
                        <xsd:enumeration value="9" />
                        <xsd:enumeration value="10" />
                        <xsd:enumeration value="11" />
                        <xsd:enumeration value="12" />
                        <xsd:enumeration value="19" />
                        <xsd:enumeration value="20" />
                        <xsd:enumeration value="21" />
                        <xsd:enumeration value="35" />
                        <xsd:enumeration value="36" />
                        <xsd:enumeration value="37" />
                        <xsd:enumeration value="38" />
                        <xsd:enumeration value="39" />
                        <xsd:enumeration value="40" />
                        <xsd:enumeration value="41" />
                        <xsd:enumeration value="42" />
                        <xsd:enumeration value="43" />
                        <xsd:enumeration value="44" />
                        <xsd:enumeration value="51" />
                        <xsd:enumeration value="52" />
                        <xsd:enumeration value="53" />
                      </xsd:restriction>
                    </xsd:simpleType>
                  </xsd:element>
                </xsd:sequence>
              </xsd:complexType>
            </xsd:element>
            <xsd:element name="Baseline" minOccurs="0" maxOccurs="unbounded">
              <xsd:annotation>
                <xsd:documentation>The baseline values for the resources.</xsd:documentation>
              </xsd:annotation>
              <xsd:complexType>
                <xsd:sequence>
                  <xsd:element name="Number" type="xsd:integer">
                    <xsd:annotation>
                      <xsd:documentation>The unique number of the baseline data record.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="Work" type="xsd:duration" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The work assigned to the resource when the baseline is saved.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="Cost" type="xsd:float" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The projected cost for the resource when the baseline was saved.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="BCWS" type="xsd:float" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The budgeted cost of work scheduled for the resource.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="BCWP" type="xsd:float" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The budgeted cost of the work performed by the resource for the project to date.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                </xsd:sequence>
              </xsd:complexType>
            </xsd:element>
            <xsd:element name="OutlineCode" minOccurs="0" maxOccurs="unbounded">
              <xsd:annotation>
                <xsd:documentation>The value of an outline code.  Two pieces of data are necessary - a pointer to the outline code table that is specified by the FieldID, and the value that is specified either by the ValueID or ValueGUID pointer to the value list.</xsd:documentation>
              </xsd:annotation>
              <xsd:complexType>
                <xsd:sequence>
                  <xsd:element name="FieldID" type="xsd:string">
                    <xsd:annotation>
                      <xsd:documentation>The number value of the custom field project ID (PID).</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="ValueID" type="xsd:integer" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The ID in the value list associated with the definition in the outline code collection.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="ValueGUID" type="xsd:integer" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The GUID of the value in the value list. The ValueGUID matches the FieldGUID in the value list.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                </xsd:sequence>
              </xsd:complexType>
            </xsd:element>
            <xsd:element name="IsCostResource" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Specifies whether the resource is a cost resource.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="AssnOwner" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The name of the assignment owner.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="AssnOwnerGuid" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The GUID of the assignment owner.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="IsBudget" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Specifies whether the resource is a budget resource.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="AvailabilityPeriods" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>A collection of periods during which the resource is available.</xsd:documentation>
              </xsd:annotation>
              <xsd:complexType>
                <xsd:sequence>
                  <xsd:element name="AvailabilityPeriod" minOccurs="0" maxOccurs="unbounded">
                    <xsd:annotation>
                      <xsd:documentation>The period that the resource is available.</xsd:documentation>
                    </xsd:annotation>
                    <xsd:complexType>
                      <xsd:sequence>
                        <xsd:element name="AvailableFrom" type="xsd:dateTime" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The date that the resource becomes available for the specified period.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <xsd:element name="AvailableTo" type="xsd:dateTime" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The last date that the resource is available for the specified period.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <xsd:element name="AvailableUnits" type="xsd:float" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The percentage that the resource is available during the specified period.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                      </xsd:sequence>
                    </xsd:complexType>
                  </xsd:element>
                </xsd:sequence>
              </xsd:complexType>
            </xsd:element>
            <xsd:element name="Rates" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>A collection of periods and the rates associated with each one.</xsd:documentation>
              </xsd:annotation>
              <xsd:complexType>
                <xsd:sequence>
                  <xsd:element name="Rate" minOccurs="0" maxOccurs="25">
                    <xsd:annotation>
                      <xsd:documentation>The definition of a time period, and the rates applicable for the resource during that period.</xsd:documentation>
                    </xsd:annotation>
                    <xsd:complexType>
                      <xsd:sequence>
                        <xsd:element name="RatesFrom" type="xsd:dateTime">
                          <xsd:annotation>
                            <xsd:documentation>The date that the rate becomes effective.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <xsd:element name="RatesTo" type="xsd:dateTime">
                          <xsd:annotation>
                            <xsd:documentation>The last date that the rate is effective.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <xsd:element name="RateTable" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The unique identifier of the rate table for the resource. Values are: 0=A, 1=B, 2=C, 3=D, 4=E.</xsd:documentation>
                          </xsd:annotation>
                          <xsd:simpleType>
                            <xsd:restriction base="xsd:integer">
                              <xsd:enumeration value="0" />
                              <xsd:enumeration value="1" />
                              <xsd:enumeration value="2" />
                              <xsd:enumeration value="3" />
                              <xsd:enumeration value="4" />
                            </xsd:restriction>
                          </xsd:simpleType>
                        </xsd:element>
                        <xsd:element name="StandardRate" type="xsd:decimal" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The standard rate for the resource for the period specified.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <xsd:element name="StandardRateFormat" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The units used by Microsoft Office Project to display the standard rate.  1=m, 2=h, 3=d, 4=w, 5=mo, 7=y.</xsd:documentation>
                          </xsd:annotation>
                          <xsd:simpleType>
                            <xsd:restriction base="xsd:integer">
                              <xsd:enumeration value="1" />
                              <xsd:enumeration value="2" />
                              <xsd:enumeration value="3" />
                              <xsd:enumeration value="4" />
                              <xsd:enumeration value="5" />
                              <xsd:enumeration value="7" />
                            </xsd:restriction>
                          </xsd:simpleType>
                        </xsd:element>
                        <xsd:element name="OvertimeRate" type="xsd:decimal" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The overtime rate for the resource for the period specified.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <xsd:element name="OvertimeRateFormat" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The units used by Microsoft Office Project to display the overtime rate.  1=m, 2=h, 3=d, 4=w, 5=mo, 7=y.</xsd:documentation>
                          </xsd:annotation>
                          <xsd:simpleType>
                            <xsd:restriction base="xsd:integer">
                              <xsd:enumeration value="1" />
                              <xsd:enumeration value="2" />
                              <xsd:enumeration value="3" />
                              <xsd:enumeration value="4" />
                              <xsd:enumeration value="5" />
                              <xsd:enumeration value="7" />
                            </xsd:restriction>
                          </xsd:simpleType>
                        </xsd:element>
                        <xsd:element name="CostPerUse" type="xsd:decimal" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The cost per use of the resource. This value is as of the current date if a rate table exists for the resource.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                      </xsd:sequence>
                    </xsd:complexType>
                  </xsd:element>
                </xsd:sequence>
              </xsd:complexType>
            </xsd:element>
            <!-- ##New Project 2007 resource enterprise custom field elements are written here.  See ResEntCF.xsd for element definitions. See the document ReadMe-XML Schemas in the C:\2007 Office System Developer Resources\Project 2007 SDK\Schemas directory for more information. -->
            <!-- ##Local custom field data is written here.  See the document ReadMe-XML Schemas in the C:\2007 Office System Developer Resources\Project 2007 SDK\Schemas directory for more information. -->
            <xsd:element name="TimephasedData" type="TimephasedDataType" minOccurs="0" maxOccurs="unbounded">
              <xsd:annotation>
                <xsd:documentation>The time phased data.</xsd:documentation>
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

[Resource Elements and XML Structure](bb968445\(v=office.12\).md)

[Custom Field Data in XML](bb968687\(v=office.12\).md)

