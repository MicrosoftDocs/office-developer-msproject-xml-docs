---
title: XML Schema for the Project Element
TOCTitle: XML Schema for the Project Element
ms:assetid: d25633d3-3350-40d6-801d-fbb3809b52b8
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968695(v=office.12)
ms:contentKeyID: 13188385
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

# XML Schema for the Project Element




The following shows the section of the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd) that defines the Project element.

The OutlineCodes, WBSMasks, ExtendedAttributes, Calendars, Tasks, Resources, and Assignments elements are all defined within the Project element; however, detailed schema information for each of these elements is shown in separate topics in this schema reference.

The complete Project XML Data Interchange Schema is included in the Project 2007 SDK download. For a link to the Project 2007 SDK download, see [Welcome to the Microsoft Office Project 2007 SDK](https://msdn.microsoft.com/en-us/library/ms512767).

## Project Schema

``` xml
<?xml version="1.0" encoding="UTF-8"?>

<!--
  The Microsoft Office Project 2007 XML Data Interchange Schema

  Revision date: 2007-11-28

  This schema defines the XML import/export format for project data in 
  Microsoft Office Project 2007. Updates to this document, if any, can 
  be found in the Project 2007 SDK download. For a link to the download, 
  see http://msdn2.microsoft.com/en-us/library/ms512767.aspx.

  Microsoft may have patents, patent applications, trademarks, copyrights,
  or other intellectual property rights covering subject matter in this 
  document. Except as expressly provided in any written license agreement 
  from Microsoft, the furnishing of this document does not give you any 
  license to these patents, trademarks, copyrights, or other intellectual 
  property.

  (c) 2007 Microsoft Corporation. All rights reserved.
-->

<xsd:schema xmlns="http://schemas.microsoft.com/project/2007" xmlns:xsd="http://www.w3.org/2001/XMLSchema" targetNamespace="http://schemas.microsoft.com/project/2007" elementFormDefault="qualified">
  <xsd:annotation>
    <xsd:documentation>The full project schema definition from the project level down, starting with data type definitions.</xsd:documentation>
    <xsd:appinfo>The Microsoft Project Data Interchange Schema for Microsoft Office Project 2007.</xsd:appinfo>
  </xsd:annotation>

  <!-- data type definitions: - @TimephasedData schema -->
  <xsd:complexType name="TimephasedDataType"> . . . </xsd:complexType>

  <!-- @Project schema -->
  <xsd:element name="Project">
    <xsd:annotation>
      <xsd:documentation>The project is the top-level element of the document.</xsd:documentation>
    </xsd:annotation>
    <xsd:complexType>
      <xsd:sequence>
        <!-- #New Project 2007 element definition -->
        <xsd:element name="SaveVersion" type="xsd:integer">
          <xsd:annotation>
            <xsd:documentation>The version of Microsoft Office Project from which the project was saved. Values are: 12=Project 2007.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <!-- #End new Project 2007 element definition -->
        <xsd:element name="UID" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The unique ID of the project.</xsd:documentation>
          </xsd:annotation>
          <xsd:simpleType>
            <xsd:restriction base="xsd:string">
              <xsd:maxLength value="16" />
            </xsd:restriction>
          </xsd:simpleType>
        </xsd:element>
        <xsd:element name="Name" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The name of the project.</xsd:documentation>
          </xsd:annotation>
          <xsd:simpleType>
            <xsd:restriction base="xsd:string">
              <xsd:maxLength value="255" />
            </xsd:restriction>
          </xsd:simpleType>
        </xsd:element>
        <xsd:element name="Title" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The title of the project.</xsd:documentation>
          </xsd:annotation>
          <xsd:simpleType>
            <xsd:restriction base="xsd:string">
              <xsd:maxLength value="512" />
            </xsd:restriction>
          </xsd:simpleType>
        </xsd:element>
        <xsd:element name="Subject" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The subject of the project.</xsd:documentation>
          </xsd:annotation>
          <xsd:simpleType>
            <xsd:restriction base="xsd:string">
              <xsd:maxLength value="512" />
            </xsd:restriction>
          </xsd:simpleType>
        </xsd:element>
        <xsd:element name="Category" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The category of the project.</xsd:documentation>
          </xsd:annotation>
          <xsd:simpleType>
            <xsd:restriction base="xsd:string">
              <xsd:maxLength value="512" />
            </xsd:restriction>
          </xsd:simpleType>
        </xsd:element>
        <xsd:element name="Company" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The company that owns the project.</xsd:documentation>
          </xsd:annotation>
          <xsd:simpleType>
            <xsd:restriction base="xsd:string">
              <xsd:maxLength value="512" />
            </xsd:restriction>
          </xsd:simpleType>
        </xsd:element>
        <xsd:element name="Manager" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The manager of the project.</xsd:documentation>
          </xsd:annotation>
          <xsd:simpleType>
            <xsd:restriction base="xsd:string">
              <xsd:maxLength value="512" />
            </xsd:restriction>
          </xsd:simpleType>
        </xsd:element>
        <xsd:element name="Author" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The author of the project.</xsd:documentation>
          </xsd:annotation>
          <xsd:simpleType>
            <xsd:restriction base="xsd:string">
              <xsd:maxLength value="512" />
            </xsd:restriction>
          </xsd:simpleType>
        </xsd:element>
        <xsd:element name="CreationDate" type="xsd:dateTime" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The date that the project was created.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="Revision" type="xsd:integer" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The number of times a project has been saved.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="LastSaved" type="xsd:dateTime" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The date that the project was last saved.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="ScheduleFromStart" type="xsd:boolean" default="true" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Whether the project is schduled from the start date or finish date.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="StartDate" type="xsd:dateTime" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The start date of the project. Required if ScheduleFromStart is true.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="FinishDate" type="xsd:dateTime" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The finish date of the project. Required if ScheduleFromStart is false.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="FYStartDate" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Fiscal Year starting month. Values are: 1=January, 2=February, 3=March, 4=April, 5=May, 6=June, 7=July, 8=August, 9=September, 10=October, 11=November, 12=December.</xsd:documentation>
          </xsd:annotation>
          <xsd:simpleType>
            <xsd:restriction base="xsd:integer">
              <xsd:enumeration value="1" />
              <xsd:enumeration value="2" />
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
            </xsd:restriction>
          </xsd:simpleType>
        </xsd:element>
        <xsd:element name="CriticalSlackLimit" type="xsd:integer" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The number of days past its end date that a task can go before Microsoft Office Project marks that task as a critical task.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="CurrencyDigits" type="xsd:integer" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The number of digits after the decimal symbol.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="CurrencySymbol" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The currency symbol used in the project.</xsd:documentation>
          </xsd:annotation>
          <xsd:simpleType>
            <xsd:restriction base="xsd:string">
              <xsd:maxLength value="20" />
            </xsd:restriction>
          </xsd:simpleType>
        </xsd:element>
        <!-- #New Project 2007 element definition -->
        <xsd:element name="CurrencyCode">
          <xsd:annotation>
            <xsd:documentation>The three-letter currency character code as defined in ISO 4217. Valid values is: USD.</xsd:documentation>
          </xsd:annotation>
          <xsd:simpleType>
            <xsd:restriction base="xsd:string">
              <xsd:maxLength value="3" />
            </xsd:restriction>
          </xsd:simpleType>
        </xsd:element>
        <!-- #End new Project 2007 element definition -->
        <xsd:element name="CurrencySymbolPosition" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The position of the currency symbol.  Values are: 0=Before, 1=After, 2=Before With Space, 3=After with space.</xsd:documentation>
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
        <xsd:element name="CalendarUID" type="xsd:integer" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The project calendar.  Refers to a valid UID in the Calendars element of the Microsoft Office Project 2007 XML Schema.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="DefaultStartTime" type="xsd:time" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The default start time of new tasks.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="DefaultFinishTime" type="xsd:time" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The default finish time of new tasks.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="MinutesPerDay" type="xsd:integer" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The number of minutes per day.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="MinutesPerWeek" type="xsd:integer" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The number of minutes per week.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="DaysPerMonth" type="xsd:integer" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The number of days per month.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="DefaultTaskType" default="1" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The default type of new tasks. Values are: 0=Fixed Units, 1=Fixed Duration, 2=Fixed Work.</xsd:documentation>
          </xsd:annotation>
          <xsd:simpleType>
            <xsd:restriction base="xsd:integer">
              <xsd:enumeration value="0" />
              <xsd:enumeration value="1" />
              <xsd:enumeration value="2" />
            </xsd:restriction>
          </xsd:simpleType>
        </xsd:element>
        <xsd:element name="DefaultFixedCostAccrual" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The default from where fixed costs are accrued.  Values are: 1=Start, 2=Prorated, 3=End.</xsd:documentation>
          </xsd:annotation>
          <xsd:simpleType>
            <xsd:restriction base="xsd:integer">
              <xsd:enumeration value="1" />
              <xsd:enumeration value="2" />
              <xsd:enumeration value="3" />
            </xsd:restriction>
          </xsd:simpleType>
        </xsd:element>
        <xsd:element name="DefaultStandardRate" type="xsd:float" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The default standard rate for new resources.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="DefaultOvertimeRate" type="xsd:float" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The default overtime rate for new resources.</xsd:documentation>
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
        <xsd:element name="WorkFormat" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The default work unit format. Values are: 1=m, 2=h, 3=d, 4=w, 5=mo.</xsd:documentation>
          </xsd:annotation>
          <xsd:simpleType>
            <xsd:restriction base="xsd:integer">
              <xsd:enumeration value="1" />
              <xsd:enumeration value="2" />
              <xsd:enumeration value="3" />
              <xsd:enumeration value="4" />
              <xsd:enumeration value="5" />
            </xsd:restriction>
          </xsd:simpleType>
        </xsd:element>
        <xsd:element name="EditableActualCosts" type="xsd:boolean" default="false" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Whether or not actual costs are editable.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="HonorConstraints" type="xsd:boolean" default="true" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Whether tasks honour their constraint dates.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="EarnedValueMethod" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The default method for calculating earned value. Values are: 0=Percent Complete, 1=Physical Percent Complete.</xsd:documentation>
          </xsd:annotation>
          <xsd:simpleType>
            <xsd:restriction base="xsd:integer">
              <xsd:enumeration value="0" />
              <xsd:enumeration value="1" />
            </xsd:restriction>
          </xsd:simpleType>
        </xsd:element>
        <xsd:element name="InsertedProjectsLikeSummary" type="xsd:boolean" default="true" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Whether to calculate subtasks as summary tasks.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="MultipleCriticalPaths" type="xsd:boolean" default="false" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Whether multiple critical paths are calculated.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="NewTasksEffortDriven" type="xsd:boolean" default="true" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Whether new tasks are effort driven.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="NewTasksEstimated" type="xsd:boolean" default="true" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Whether to show the estimated duration by default.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="SplitsInProgressTasks" type="xsd:boolean" default="true" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Whether in-progress tasks can be split.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="SpreadActualCost" type="xsd:boolean" default="true" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Whether actual costs are spread to the status date.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="SpreadPercentComplete" type="xsd:boolean" default="false" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Whether percent complete is spread to the status date.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="TaskUpdatesResource" type="xsd:boolean" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Whether updates to tasks update resources.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="FiscalYearStart" type="xsd:boolean" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Specifies whether to use fiscal year numbering.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="WeekStartDay" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Start day of the week. Values are: 0=Sunday, 1=Monday, 2=Tuesday, 3=Wednesday, 4=Thursday, 5=Friday, 6=Saturday.</xsd:documentation>
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
            </xsd:restriction>
          </xsd:simpleType>
        </xsd:element>
        <xsd:element name="MoveCompletedEndsBack" type="xsd:boolean" default="false" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Specifies whether the end of completed portions of tasks scheduled to begin after the status date but begun early should be moved back to the status date.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="MoveRemainingStartsBack" type="xsd:boolean" default="false" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Specifies whether the beginning of remaining portions of tasks scheduled to begin after the status date but begun early should be moved back to the status date.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="MoveRemainingStartsForward" type="xsd:boolean" default="false" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Specifies whether the beginning of remaining portions of tasks scheduled to have begun late should be moved up to the status date.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="MoveCompletedEndsForward" type="xsd:boolean" default="false" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Specifies whether the end of completed portions of tasks scheduled to have been completed before the status date but begun late should be moved up to the status date.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="BaselineForEarnedValue" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The specific baseline used to calculate Variance values.  Values are: 0=Baseline, 1=Baseline 1, 2=Baseline 2, 3=Baseline 3, 4=Baseline 4, 5=Baseline 5, 6=Baseline 6, 7=Baseline 7, 8=Baseline 8, 9=Baseline 9, 10=Baseline 10.</xsd:documentation>
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
              <xsd:enumeration value="9" />
              <xsd:enumeration value="10" />
            </xsd:restriction>
          </xsd:simpleType>
        </xsd:element>
        <xsd:element name="AutoAddNewResourcesAndTasks" type="xsd:boolean" default="true" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Whether to automatically add new resources to the resource pool.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="StatusDate" type="xsd:dateTime" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Date used for calculation and reporting.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="CurrentDate" type="xsd:dateTime" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The system date that the XML was generated.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="MicrosoftProjectServerURL" type="xsd:boolean" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Whether the project was created by a Project Server user as opposed to an NT user.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="Autolink" type="xsd:boolean" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Whether to autolink inserted or moved tasks.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="NewTaskStartDate" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The default start date for new tasks.  Values are: 0=Project Start Date, 1=Current Date.</xsd:documentation>
          </xsd:annotation>
          <xsd:simpleType>
            <xsd:restriction base="xsd:integer">
              <xsd:enumeration value="0" />
              <xsd:enumeration value="1" />
            </xsd:restriction>
          </xsd:simpleType>
        </xsd:element>
        <xsd:element name="DefaultTaskEVMethod" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>The default earned value method for tasks.  Values are: 0=Percent Complete, 1=Physical Percent Complete.</xsd:documentation>
          </xsd:annotation>
          <xsd:simpleType>
            <xsd:restriction base="xsd:integer">
              <xsd:enumeration value="0" />
              <xsd:enumeration value="1" />
            </xsd:restriction>
          </xsd:simpleType>
        </xsd:element>
        <xsd:element name="ProjectExternallyEdited" type="xsd:boolean" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Whether the project XML was edited.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="ExtendedCreationDate" type="xsd:dateTime" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Date used for calculation and reporting.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="ActualsInSync" type="xsd:boolean" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Whether all actual work has been synchronized with the project.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="RemoveFileProperties" type="xsd:boolean" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Whether to remove all file properties on save.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="AdminProject" type="xsd:boolean" minOccurs="0">
          <xsd:annotation>
            <xsd:documentation>Whether the project is an administrative project.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>

        <!-- @OutlineCode Schema -->
        <xsd:element name="OutlineCodes" minOccurs="0"> . . . </xsd:element>

        <!-- @WBSMask Schema -->
        <xsd:element name="WBSMasks" minOccurs="0"> . . . </xsd:element>

        <!-- @ExtendedAttribute Schema -->
        <xsd:element name="ExtendedAttributes" minOccurs="0"> . . . </xsd:element>

        <!-- @Calendar Schema -->
        <xsd:element name="Calendars" minOccurs="0"> . . . </xsd:element>

        <!-- @Task Schema -->
        <xsd:element name="Tasks" minOccurs="0"> . . . </xsd:element>

        <!-- @Resource Schema -->
        <xsd:element name="Resources" minOccurs="0"> . . . </xsd:element>

        <!-- @Assignment Schema -->
        <xsd:element name="Assignments" minOccurs="0"> . . . </xsd:element>

      </xsd:sequence>
    </xsd:complexType>
  </xsd:element>
```

## See Also

#### Concepts

[Project Elements and XML Structure](bb968439\(v=office.12\).md)

[XML Schema for the OutlineCodes Element](bb968584\(v=office.12\).md)

[XML Schema for the WBSMasks Element](bb968565\(v=office.12\).md)

[XML Schema for the ExtendedAttributes Element](bb968705\(v=office.12\).md)

[XML Schema for the Calendars Element](bb968557\(v=office.12\).md)

[XML Schema for the Tasks Element](bb968415\(v=office.12\).md)

[XML Schema for the Resources Element](bb968511\(v=office.12\).md)

[XML Schema for the Assignments Element](bb968414\(v=office.12\).md)

