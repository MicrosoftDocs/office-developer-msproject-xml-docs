---
title: XML Schema for the Tasks Element
TOCTitle: XML Schema for the Tasks Element
ms:assetid: 0ff12ab6-ac7f-4d45-aadc-7f6fce6c082c
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968415(v=office.12)
ms:contentKeyID: 13188108
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
localization_priority: Normal
---

# XML Schema for the Tasks Element

The following shows the section of the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd) that defines the Tasks element.

The complete Project XML Data Interchange Schema is included in the Project 2007 SDK download. For a link to the Project 2007 SDK download, see [Welcome to the Microsoft Office Project 2007 SDK](https://msdn.microsoft.com/en-us/library/ms512767).

## Tasks Schema

``` xml
<?xml version="1.0" encoding="utf-8"?>
. . .
<!-- @Task schema -->
<xsd:element name="Tasks" minOccurs="0">
  <xsd:annotation>
    <xsd:documentation>The collection of tasks that make up the project.</xsd:documentation>
  </xsd:annotation>
  <xsd:complexType>
    <xsd:sequence>
      <xsd:element name="Task" minOccurs="0" maxOccurs="unbounded">
        <xsd:annotation>
          <xsd:documentation>There must be at least one task in each Tasks collection.</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="UID" type="xsd:integer">
              <xsd:annotation>
                <xsd:documentation>The unique ID of the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ID" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The position identifier of the task within the list of tasks.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Name" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The name of the task.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="512" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="Type" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The type of task. Values are: 0=Fixed Units, 1=Fixed Duration, 2=Fixed Work.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:integer">
                  <xsd:enumeration value="0" />
                  <xsd:enumeration value="1" />
                  <xsd:enumeration value="2" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="IsNull" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Specifies whether the task is null.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="CreateDate" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The date that the task was created.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Contact" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The contact person for the task.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="512" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="WBS" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The work breakdown structure (WBS) code of the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="WBSLevel" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The right-most WBS level of the task. For example, if the task level was A.01.03, the right-most level would be 03.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="OutlineNumber" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The outline number of the task.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="512" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="OutlineLevel" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The outline level of the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Priority" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The priority of the task from 0 to 1000.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Start" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The scheduled start date of the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Finish" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The scheduled finish date of the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Duration" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The planned duration of the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="DurationFormat" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The format for expressing the Duration of the Task.  Values are: 3=m, 4=em, 5=h, 6=eh, 7=d, 8=ed, 9=w, 10=ew, 11=mo, 12=emo, 19=%, 20=e%, 21=null, 35=m?, 36=em?, 37=h?, 38=eh?, 39=d?, 40=ed?, 41=w?, 42=ew?, 43=mo?, 44=emo?, 51=%?, 52=e%? and 53=null.</xsd:documentation>
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
            <xsd:element name="Work" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The amount of scheduled work for the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Stop" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The date that the task was stopped.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Resume" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The date that the task resumed.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ResumeValid" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether the task can be resumed.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="EffortDriven" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether the task is effort-driven.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Recurring" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether the task is a recurring task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="OverAllocated" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether the task is overallocated. This element is for information only.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Estimated" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether the task is estimated.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Milestone" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether the task is a milestone.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Summary" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether the task is a summary task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Critical" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether the task is in the critical chain.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="IsSubproject" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether the task is an inserted project.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="IsSubprojectReadOnly" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether the inserted project is read-only.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="SubprojectName" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The source location of the inserted project.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="512" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="ExternalTask" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether the task is external.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ExternalTaskProject" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The source location and task identifier of the external task.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="512" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="EarlyStart" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The early start date of the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="EarlyFinish" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The early finish date of the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="LateStart" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The late start date of the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="LateFinish" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The late finish date of the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="StartVariance" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The variance of the task start date from the baseline start date as minutes x 1000.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="FinishVariance" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The variance of the task finish date from the baseline finish date as minutes x 1000.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="WorkVariance" type="xsd:float" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The variance of task work from the baseline task work as minutes x 1000.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="FreeSlack" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The amount of free slack.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="TotalSlack" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The amount of total slack.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="FixedCost" type="xsd:float" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The fixed cost of the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="FixedCostAccrual" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>How the fixed cost is accrued against the task. Values are: 1=Start, 2=Prorated and 3=End.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:enumeration value="1" />
                  <xsd:enumeration value="2" />
                  <xsd:enumeration value="3" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="PercentComplete" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The percentage of the task duration completed.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="PercentWorkComplete" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The percentage of the task work completed.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Cost" type="xsd:decimal" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The projected or scheduled cost of the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="OvertimeCost" type="xsd:decimal" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The sum of the actual and remaining overtime cost of the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="OvertimeWork" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The amount of overtime work scheduled for the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ActualStart" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The actual start date of the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ActualFinish" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The actual finish date of the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ActualDuration" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The actual duration of the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ActualCost" type="xsd:decimal" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The actual cost of the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ActualOvertimeCost" type="xsd:decimal" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The actual overtime cost of the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ActualWork" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The actual work for the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ActualOvertimeWork" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The actual overtime work for the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="RegularWork" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The amount of non-overtime work scheduled for the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="RemainingDuration" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The amount of time required to complete the unfinished portion of the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="RemainingCost" type="xsd:decimal" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The remaining projected cost of completing the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="RemainingWork" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The remaining work scheduled to complete the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="RemainingOvertimeCost" type="xsd:decimal" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The remaining overtime cost projected to finish the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="RemainingOvertimeWork" type="xsd:duration" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The remaining overtime work scheduled to finish the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ACWP" type="xsd:float" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The actual cost of work performed on the task to date.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="CV" type="xsd:float" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Earned value cost variance.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ConstraintType" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The constraint on the start or finish date of the task. Values are: 0=As Soon As Possible, 1=As Late As Possible, 2=Must Start On, 3=Must Finish On, 4=Start No Earlier Than, 5=Start No Later Than, 6=Finish No Earlier Than and 7=Finish No Later Than.</xsd:documentation>
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
            <xsd:element name="CalendarUID" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The task calendar. Refers to a valid UID in the Calendars element of the Microsoft Office Project 2007 XML Schema.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="ConstraintDate" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The date argument for the task constraint type.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Deadline" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The deadline for the task to be completed.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="LevelAssignments" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether leveling can adjust assignments.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="LevelingCanSplit" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether leveling can split the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="LevelingDelay" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The delay caused by leveling the task.</xsd:documentation>
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
            <xsd:element name="PreLeveledStart" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The start date of the task before it was leveled.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="PreLeveledFinish" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The finish date of the task before it was leveled.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Hyperlink" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The title of the hyperlink associated with the task.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="512" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="HyperlinkAddress" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The hyperlink associated with the task.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="512" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="HyperlinkSubAddress" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The document bookmark of the hyperlink associated with the task.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="512" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="IgnoreResourceCalendar" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether the task ignores the resource calendar.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Notes" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Text notes associated with the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="HideBar" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether the GANTT bar of the task is hidden when displayed in Microsoft Office Project.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Rollup" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether the task is rolled up.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="BCWS" type="xsd:float" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The budgeted cost of work scheduled for the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="BCWP" type="xsd:float" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The budgeted cost of work performed on the task to date.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="PhysicalPercentComplete" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The percentage complete value entered by the Project Manager.  This can be used as an alternative for calculating the budgeted cost of work performed (BCWP).</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="EarnedValueMethod" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The method for calculating earned value. Values are: 0=Percent Complete, 1=Physical Percent Complete.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:integer">
                  <xsd:enumeration value="0" />
                  <xsd:enumeration value="1" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="PredecessorLink" minOccurs="0" maxOccurs="unbounded">
              <xsd:annotation>
                <xsd:documentation>Defines the predecessor task of the task that contains it.</xsd:documentation>
              </xsd:annotation>
              <xsd:complexType>
                <xsd:sequence>
                  <xsd:element name="PredecessorUID" type="xsd:integer" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The unique identifier of the predecessor task.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="Type" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The link type.  Values are 0=FF, 1=FS, 2=SF and 3=SS.</xsd:documentation>
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
                  <xsd:element name="CrossProject" type="xsd:boolean" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>Whether the predecessor is part of another project.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="CrossProjectName" type="xsd:string" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The external predecessor project.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="LinkLag" type="xsd:integer" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The amount of lag in tenths of a minute.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="LagFormat" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The format for expressing the lag format.  Values are: 3=m, 4=em, 5=h, 6=eh, 7=d, 8=ed, 9=w, 10=ew, 11=mo, 12=emo, 19=%, 20=e%, 35=m?, 36=em?, 37=h?, 38=eh?, 39=d?, 40=ed?, 41=w?, 42=ew?, 43=mo?, 44=emo?, 51=%? and 52=e%?.</xsd:documentation>
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
                <xsd:documentation>The collection of baseline values of the task.</xsd:documentation>
              </xsd:annotation>
              <xsd:complexType>
                <xsd:sequence>
                  <xsd:element name="TimephasedData" type="TimephasedDataType" minOccurs="0" maxOccurs="unbounded">
                    <xsd:annotation>
                      <xsd:documentation>The timephased data block associated with the task baseline.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="Number" type="xsd:integer" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The unique number of the baseline data record.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="Interim" type="xsd:boolean" default="false" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>Whether this is an interim baseline.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="Start" type="xsd:dateTime" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The scheduled start date of the task when the baseline was saved.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="Finish" type="xsd:dateTime" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The scheduled finish date of the task when the baseline was saved.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="Duration" type="xsd:duration" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The scheduled duration of the task when the baseline was saved.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="DurationFormat" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The format for expressing the Duration of the Task baseline.  Values are: 3=m, 4=em, 5=h, 6=eh, 7=d, 8=ed, 9=w, 10=ew, 11=mo, 12=emo, 19=%, 20=e%, 21=null, 35=m?, 36=em?, 37=h?, 38=eh?, 39=d?, 40=ed?, 41=w?, 42=ew?, 43=mo?, 44=emo?, 51=%?, 52=e%? and 53=null.</xsd:documentation>
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
                  <xsd:element name="EstimatedDuration" type="xsd:boolean" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>Whether the baseline duration of the task was estimated.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="Work" type="xsd:duration" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The scheduled work of the task when the baseline was saved.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="Cost" type="xsd:decimal" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The projected cost of the task when the baseline was saved.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="BCWS" type="xsd:float" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The budgeted cost of work scheduled for the task.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="BCWP" type="xsd:float" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The budgeted cost of work performed on the task to date.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="FixedCost" type="xsd:float" minOccurs="0">
                    <xsd:annotation>
                      <xsd:documentation>The fixed cost of the task when the baseline was saved.</xsd:documentation>
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
            <xsd:element name="IsPublished" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Specifies whether the task is published.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="StatusManager" type="xsd:string" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The name of the task status manager.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="CommitmentStart" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The start date of the deliverable.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="CommitmentFinish" type="xsd:dateTime" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The finish date of the deliverable.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="CommitmentType" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Specifies whether the task has an associated deliverable or a dependency on an associated deliverable. Values are: 0=The task has no deliverable or dependency on a deliverable, 1=The task has an associated deliverable, 2=The task has a dependency on an associated deliverable.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:integer">
                  <xsd:enumeration value="0" />
                  <xsd:enumeration value="1" />
                  <xsd:enumeration value="2" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <!-- ##New Project 2007 project enterprise custom field elements are written here.  See ProjEntCF.xsd for element definitions. See the document ReadMe-XML Schemas in the C:\2007 Office System Developer Resources\Project 2007 SDK\Schemas directory for more information. -->
            <!-- ##New Project 2007 task enterprise custom field elements are written here.  See TaskEntCF.xsd for element definitions. See the document ReadMe-XML Schemas in the C:\2007 Office System Developer Resources\Project 2007 SDK\Schemas directory for more information. -->
            <!-- ##Local custom field data is written here.  See the document ReadMe-XML Schemas in the C:\2007 Office System Developer Resources\Project 2007 SDK\Schemas directory for more information. -->
            <xsd:element name="TimephasedData" type="TimephasedDataType" minOccurs="0" maxOccurs="unbounded">
              <xsd:annotation>
                <xsd:documentation>The time phased data block associated with the task.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <!-- #End new Project 2007 element definitions -->
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
</xsd:element>
```

## See Also

#### Concepts

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[Custom Field Data in XML](custom-field-data-in-xml.md)

