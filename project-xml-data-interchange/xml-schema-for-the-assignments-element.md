---
title: XML Schema for the Assignments Element
TOCTitle: XML Schema for the Assignments Element
ms:assetid: 0f1de37d-fa67-4120-9d24-c98d7067f842
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968414(v=office.12)
ms:contentKeyID: 13188107
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

# XML Schema for the Assignments Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

The following shows the section of the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd) that defines the Assignments element.

The complete Project XML Data Interchange Schema is included in the Project 2007 SDK download. For a link to the Project 2007 SDK download, see [Welcome to the Microsoft Office Project 2007 SDK](https://msdn.microsoft.com/en-us/library/ms512767).

## Assignments Schema

``` xml
<?xml version="1.0" encoding="utf-8"?>
. . .
<!-- @Assignment schema -->
<xsd:element name="Assignments" minOccurs="0">
  <xsd:annotation>
    <xsd:documentation>The collection of assignments that make up the project.</xsd:documentation>
  </xsd:annotation>
  <xsd:complexType>
    <xsd:sequence>
      <xsd:element name="Assignment" minOccurs="0" maxOccurs="unbounded">
        <xsd:annotation>
          <xsd:documentation>There must be at least one assignment in each Assignments collection.</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="UID" type="xsd:integer">
              <xsd:annotation>
                <xsd:documentation>The unique identifier of the assignment.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="TaskUID" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The unique identifier of the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ResourceUID" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The unique identifier of the resource.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="PercentWorkComplete" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The amount of work completed on the assignment.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ActualCost" type="xsd:decimal" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The actual cost incurred on the assignment.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ActualFinish" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The actual finish date of the assignment.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ActualOvertimeCost" type="xsd:decimal" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The actual overtime cost incurred on the assignment.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ActualOvertimeWork" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The actual amount of overtime work incurred on the assignment.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ActualStart" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The actual start date of the assignment.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ActualWork" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The actual amount of work incurred on the assignment.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ACWP" type="xsd:float" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The actual cost of work performed on the assignment to date.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Confirmed" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether the Resource has accepted all of his or her assignments.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Cost" type="xsd:decimal" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The projected or scheduled cost of the assignment.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="CostRateTable" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The cost rate table used for the assignment.</xsd:documentation>
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
            <xsd:element name="CostVariance" type="xsd:float" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The difference between the cost and baseline cost for a resource.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="CV" type="xsd:float" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Earned value cost variance.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Delay" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The amount that the assignment is delayed.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Finish" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The scheduled finish date of the assignment.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="FinishVariance" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The variance of the assignment finish date from the baseline finish date.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Hyperlink" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The title of the hyperlink associated with the assignment.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="512" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="HyperlinkAddress" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The hyperlink associated with the assignment.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="512" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="HyperlinkSubAddress" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The document bookmark of the hyperlink associated with the assignment.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="512" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="WorkVariance" type="xsd:float" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The variance of assignment work from the baseline work as minutes x 1000.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="HasFixedRateUnits" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether the Units are Fixed Rate.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="FixedMaterial" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether the consumption of the assigned material resource occurs in a single, fixed amount.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="LevelingDelay" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The delay caused by leveling.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="LevelingDelayFormat" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The format for expressing the duration of the delay.  Values are: 3=m, 4=em, 5=h, 6=eh, 7=d, 8=ed, 9=w, 10=ew, 11=mo, 12=emo, 19=%, 20=e%, 21=null, 35=m?, 36=em?, 37=h?, 38=eh?, 39=d?, 40=ed?, 41=w?, 42=ew?, 43=mo?, 44=emo?, 51=%?, 52=e%? and 53=null.</xsd:documentation>
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
            <xsd:element name="LinkedFields" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether the project is linked to another OLE object.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Milestone" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether the assignment is a milestone.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Notes" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Text notes associated with the assignment.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Overallocated" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether the assignment is overallocated.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="OvertimeCost" type="xsd:decimal" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The sum of the actual and remaining overtime cost of the assignment.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="OvertimeWork" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The scheduled overtime work scheduled for the assignment.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="PeakUnits" type="xsd:float" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The largest number of units that a resource is assigned for a task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="RegularWork" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The amount of non-overtime work scheduled for the assignment.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="RemainingCost" type="xsd:decimal" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The remaining projected cost of completing the assignment.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="RemainingOvertimeCost" type="xsd:decimal" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The remaining projected overtime cost of completing the assignment.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="RemainingOvertimeWork" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The remaining overtime work scheduled to complete the assignment.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="RemainingWork" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The remaining work scheduled to complete the assignment.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ResponsePending" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>True if a response has not been received for a TeamAssign message. </xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Start" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The scheduled start date of the assignment.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Stop" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The date that the assignment was stopped.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Resume" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The date that the assignment resumed.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="StartVariance" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The variance of the assignment start date from the baseline start date.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Summary" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Specifies whether the task is a summary task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="SV" type="xsd:float" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Earned value schedule variance, through the project status date.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Units" type="xsd:float" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The number of units for the assignment.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="UpdateNeeded" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>True if the resource assigned to a task needs to be updated as to the status of the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="VAC" type="xsd:float" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The difference between basline cost and total cost.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Work" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The amount of scheduled work for the assignment.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="WorkContour" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The work contour of the assignment. Values are: 0=Flat, 1=Back Loaded, 2=Front Loaded, 3=Double Peak, 4=Early Peak, 5=Late Peak, 6=Bell, 7=Turtle, 8=Contoured.</xsd:documentation>
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
                  <xsd:enumeration value="8" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="BCWS" type="xsd:float" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The budgeted cost of work on the assignment.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="BCWP" type="xsd:float" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The budgeted cost of work performed on the assignment to date.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="BookingType" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Specifies the booking type of the assignment. 1=Commited, 2=Proposed.</xsd:documentation>
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
            <xsd:element name="CreationDate" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The date that the assignment was created.</xsd:documentation>
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
            <xsd:element name="BudgetCost" type="xsd:decimal" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The budgeted amount for cost resources on this assignment.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="BudgetWork" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The budgeted work amount for work or material resources on this assignment.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ExtendedAttribute" minOccurs="0" maxOccurs="unbounded">
              <xsd:annotation>
                <xsd:documentation>The value of an extended attribute.  Two pieces of data are needed: a pointer back to the extended attribute table that is specified either by the unique ID or the Field ID, and the value that is specified either with the value or a pointer back to the value list.</xsd:documentation>
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
                <xsd:documentation>The collection of baseline values associated with the assignment.</xsd:documentation>
              </xsd:annotation>
              <xsd:complexType>
                <xsd:sequence>
                  <xsd:element name="TimephasedData" type="TimephasedDataType" minOccurs="0" maxOccurs="unbounded">
                    <xsd:annotation>
                      <xsd:documentation>The time phased data associated with the Baseline.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="Number" type="xsd:string">
                    <xsd:annotation>
                      <xsd:documentation>The unique number of the baseline data record.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="Start" type="xsd:string" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The scheduled start date of the assignment when the baseline was saved.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="Finish" type="xsd:string" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The scheduled finish date of the assignment when the baseline was saved.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="Work" type="xsd:duration" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The total amount of work scheduled on the assignment when the baseline was saved.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="Cost" type="xsd:string" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The total projected cost of the assignment when the baseline was saved.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="BCWS" type="xsd:float" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The budgeted cost of work on the assignment.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="BCWP" type="xsd:float" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The budgeted cost of work performed on the assignment to date.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                </xsd:sequence>
              </xsd:complexType>
            </xsd:element>
            <!-- ##New Project 2007 assignment enterprise custom field elements are written here.  See AssnEntCF.xsd for element definitions. See the document ReadMe-XML Schemas in the C:\2007 Office System Developer Resources\Project 2007 SDK\Schemas directory for more information. -->
            <!-- Element defintions for assignment local custom field data. -->
            <xsd:element name="f404000" minOccurs="0" />
            <xsd:element name="f404001" minOccurs="0" />
            <xsd:element name="f404002" minOccurs="0" />
            <xsd:element name="f404003" minOccurs="0" />
            <xsd:element name="f404004" minOccurs="0" />
            <xsd:element name="f404005" minOccurs="0" />
            <xsd:element name="f404006" minOccurs="0" />
            <xsd:element name="f404007" minOccurs="0" />
            <xsd:element name="f404008" minOccurs="0" />
            <xsd:element name="f404009" minOccurs="0" />
            <xsd:element name="f40400a" minOccurs="0" />
            <xsd:element name="f40400b" minOccurs="0" />
            <xsd:element name="f40400c" minOccurs="0" />
            <xsd:element name="f40400d" minOccurs="0" />
            <xsd:element name="f40400e" minOccurs="0" />
            <xsd:element name="f40400f" minOccurs="0" />
            <xsd:element name="f404010" minOccurs="0" />
            <xsd:element name="f404011" minOccurs="0" />
            <xsd:element name="f404012" minOccurs="0" />
            <xsd:element name="f404013" minOccurs="0" />
            <xsd:element name="f404014" minOccurs="0" />
            <xsd:element name="f404015" minOccurs="0" />
            <xsd:element name="f404016" minOccurs="0" />
            <xsd:element name="f404017" minOccurs="0" />
            <xsd:element name="f404018" minOccurs="0" />
            <xsd:element name="f404019" minOccurs="0" />
            <xsd:element name="f40401a" minOccurs="0" />
            <xsd:element name="f40401b" minOccurs="0" />
            <xsd:element name="f40401c" minOccurs="0" />
            <xsd:element name="f40401d" minOccurs="0" />
            <xsd:element name="f40401e" minOccurs="0" />
            <xsd:element name="f40401f" minOccurs="0" />
            <xsd:element name="f404020" minOccurs="0" />
            <xsd:element name="f404021" minOccurs="0" />
            <xsd:element name="f404022" minOccurs="0" />
            <xsd:element name="f404023" minOccurs="0" />
            <xsd:element name="f404024" minOccurs="0" />
            <xsd:element name="f404025" minOccurs="0" />
            <xsd:element name="f404026" minOccurs="0" />
            <xsd:element name="f404027" minOccurs="0" />
            <xsd:element name="f404028" minOccurs="0" />
            <xsd:element name="f404029" minOccurs="0" />
            <xsd:element name="f40402a" minOccurs="0" />
            <xsd:element name="f40402b" minOccurs="0" />
            <xsd:element name="f40402c" minOccurs="0" />
            <xsd:element name="f40402d" minOccurs="0" />
            <xsd:element name="f40402e" minOccurs="0" />
            <xsd:element name="f40402f" minOccurs="0" />
            <xsd:element name="f404030" minOccurs="0" />
            <xsd:element name="f404031" minOccurs="0" />
            <xsd:element name="f404032" minOccurs="0" />
            <xsd:element name="f404033" minOccurs="0" />
            <xsd:element name="f404034" minOccurs="0" />
            <xsd:element name="f404035" minOccurs="0" />
            <xsd:element name="f404036" minOccurs="0" />
            <xsd:element name="f404037" minOccurs="0" />
            <xsd:element name="f404038" minOccurs="0" />
            <xsd:element name="f404039" minOccurs="0" />
            <xsd:element name="f40403a" minOccurs="0" />
            <xsd:element name="f40403b" minOccurs="0" />
            <xsd:element name="f40403c" minOccurs="0" />
            <xsd:element name="f40403d" minOccurs="0" />
            <xsd:element name="f40403e" minOccurs="0" />
            <xsd:element name="f40403f" minOccurs="0" />
            <xsd:element name="f404040" minOccurs="0" />
            <xsd:element name="f404041" minOccurs="0" />
            <xsd:element name="f404042" minOccurs="0" />
            <xsd:element name="f404043" minOccurs="0" />
            <xsd:element name="f404044" minOccurs="0" />
            <xsd:element name="f404045" minOccurs="0" />
            <xsd:element name="f404046" minOccurs="0" />
            <xsd:element name="f404047" minOccurs="0" />
            <xsd:element name="f404048" minOccurs="0" />
            <xsd:element name="f404049" minOccurs="0" />
            <xsd:element name="f40404a" minOccurs="0" />
            <xsd:element name="f40404b" minOccurs="0" />
            <xsd:element name="f40404c" minOccurs="0" />
            <xsd:element name="f40404d" minOccurs="0" />
            <xsd:element name="f40404e" minOccurs="0" />
            <xsd:element name="f40404f" minOccurs="0" />
            <xsd:element name="f404050" minOccurs="0" />
            <xsd:element name="f404051" minOccurs="0" />
            <xsd:element name="f404052" minOccurs="0" />
            <xsd:element name="f404053" minOccurs="0" />
            <xsd:element name="f404054" minOccurs="0" />
            <xsd:element name="f404055" minOccurs="0" />
            <xsd:element name="f404056" minOccurs="0" />
            <xsd:element name="f404057" minOccurs="0" />
            <xsd:element name="f404058" minOccurs="0" />
            <xsd:element name="f404059" minOccurs="0" />
            <xsd:element name="f40405a" minOccurs="0" />
            <xsd:element name="f40405b" minOccurs="0" />
            <xsd:element name="f40405c" minOccurs="0" />
            <xsd:element name="f40405d" minOccurs="0" />
            <xsd:element name="f40405e" minOccurs="0" />
            <xsd:element name="f40405f" minOccurs="0" />
            <xsd:element name="f404060" minOccurs="0" />
            <xsd:element name="f404061" minOccurs="0" />
            <xsd:element name="f404062" minOccurs="0" />
            <xsd:element name="f404063" minOccurs="0" />
            <xsd:element name="f404064" minOccurs="0" />
            <xsd:element name="f404065" minOccurs="0" />
            <xsd:element name="f404066" minOccurs="0" />
            <xsd:element name="f404067" minOccurs="0" />
            <xsd:element name="f404068" minOccurs="0" />
            <xsd:element name="f404069" minOccurs="0" />
            <xsd:element name="f40406a" minOccurs="0" />
            <xsd:element name="f40406b" minOccurs="0" />
            <xsd:element name="f40406c" minOccurs="0" />
            <xsd:element name="f40406d" minOccurs="0" />
            <xsd:element name="f40406e" minOccurs="0" />
            <xsd:element name="f40406f" minOccurs="0" />
            <xsd:element name="f404070" minOccurs="0" />
            <xsd:element name="f404071" minOccurs="0" />
            <xsd:element name="f404072" minOccurs="0" />
            <xsd:element name="f404073" minOccurs="0" />
            <xsd:element name="f404074" minOccurs="0" />
            <xsd:element name="f404075" minOccurs="0" />
            <xsd:element name="f404076" minOccurs="0" />
            <xsd:element name="f404077" minOccurs="0" />
            <xsd:element name="f404078" minOccurs="0" />
            <xsd:element name="f404079" minOccurs="0" />
            <xsd:element name="f40407a" minOccurs="0" />
            <xsd:element name="f40407b" minOccurs="0" />
            <xsd:element name="f40407c" minOccurs="0" />
            <xsd:element name="f40407d" minOccurs="0" />
            <xsd:element name="f40407e" minOccurs="0" />
            <xsd:element name="f40407f" minOccurs="0" />
            <xsd:element name="f404080" minOccurs="0" />
            <xsd:element name="f404081" minOccurs="0" />
            <xsd:element name="f404082" minOccurs="0" />
            <xsd:element name="f404083" minOccurs="0" />
            <xsd:element name="f404084" minOccurs="0" />
            <xsd:element name="f404085" minOccurs="0" />
            <xsd:element name="f404086" minOccurs="0" />
            <xsd:element name="f404087" minOccurs="0" />
            <xsd:element name="f404088" minOccurs="0" />
            <xsd:element name="f404089" minOccurs="0" />
            <xsd:element name="f40408a" minOccurs="0" />
            <xsd:element name="f40408b" minOccurs="0" />
            <xsd:element name="f40408c" minOccurs="0" />
            <xsd:element name="f40408d" minOccurs="0" />
            <xsd:element name="f40408e" minOccurs="0" />
            <xsd:element name="f40408f" minOccurs="0" />
            <xsd:element name="f404090" minOccurs="0" />
            <xsd:element name="f404091" minOccurs="0" />
            <xsd:element name="f404092" minOccurs="0" />
            <xsd:element name="f404093" minOccurs="0" />
            <xsd:element name="f404094" minOccurs="0" />
            <xsd:element name="f404095" minOccurs="0" />
            <xsd:element name="f404096" minOccurs="0" />
            <xsd:element name="f404097" minOccurs="0" />
            <xsd:element name="f404098" minOccurs="0" />
            <xsd:element name="f404099" minOccurs="0" />
            <xsd:element name="f40409a" minOccurs="0" />
            <xsd:element name="f40409b" minOccurs="0" />
            <xsd:element name="f40409c" minOccurs="0" />
            <xsd:element name="f40409d" minOccurs="0" />
            <xsd:element name="f40409e" minOccurs="0" />
            <xsd:element name="f40409f" minOccurs="0" />
            <xsd:element name="f4040a0" minOccurs="0" />
            <xsd:element name="f4040a1" minOccurs="0" />
            <xsd:element name="f4040a2" minOccurs="0" />
            <xsd:element name="f4040a3" minOccurs="0" />
            <xsd:element name="f4040a4" minOccurs="0" />
            <xsd:element name="f4040a5" minOccurs="0" />
            <xsd:element name="f4040a6" minOccurs="0" />
            <xsd:element name="f4040a7" minOccurs="0" />
            <xsd:element name="f4040a8" minOccurs="0" />
            <xsd:element name="f4040a9" minOccurs="0" />
            <xsd:element name="f4040aa" minOccurs="0" />
            <xsd:element name="f4040ab" minOccurs="0" />
            <xsd:element name="f4040ac" minOccurs="0" />
            <xsd:element name="f4040ad" minOccurs="0" />
            <xsd:element name="f4040ae" minOccurs="0" />
            <xsd:element name="f4040af" minOccurs="0" />
            <xsd:element name="f4040b0" minOccurs="0" />
            <xsd:element name="f4040b1" minOccurs="0" />
            <xsd:element name="f4040b2" minOccurs="0" />
            <xsd:element name="f4040b3" minOccurs="0" />
            <xsd:element name="f4040b4" minOccurs="0" />
            <xsd:element name="f4040b5" minOccurs="0" />
            <xsd:element name="f4040b6" minOccurs="0" />
            <xsd:element name="f4040b7" minOccurs="0" />
            <xsd:element name="f4040b8" minOccurs="0" />
            <xsd:element name="f4040b9" minOccurs="0" />
            <xsd:element name="f4040ba" minOccurs="0" />
            <xsd:element name="f4040bb" minOccurs="0" />
            <xsd:element name="f4040bc" minOccurs="0" />
            <xsd:element name="f4040bd" minOccurs="0" />
            <xsd:element name="f4040be" minOccurs="0" />
            <xsd:element name="f4040bf" minOccurs="0" />
            <xsd:element name="f4040c0" minOccurs="0" />
            <xsd:element name="f4040c1" minOccurs="0" />
            <xsd:element name="f4040c2" minOccurs="0" />
            <xsd:element name="f4040c3" minOccurs="0" />
            <xsd:element name="f4040c4" minOccurs="0" />
            <xsd:element name="f4040c5" minOccurs="0" />
            <xsd:element name="f4040c6" minOccurs="0" />
            <xsd:element name="f4040c7" minOccurs="0" />
            <xsd:element name="f4040c8" minOccurs="0" />
            <xsd:element name="TimephasedData" type="TimephasedDataType" minOccurs="0" maxOccurs="unbounded">
              <xsd:annotation>
                <xsd:documentation>The time phased data associated with the assignment.</xsd:documentation>
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

[Assignment Elements and XML Structure](bb968738\(v=office.12\).md)

[Custom Field Data in XML](bb968687\(v=office.12\).md)

