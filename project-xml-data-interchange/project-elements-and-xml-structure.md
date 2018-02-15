---
title: Project Elements and XML Structure
TOCTitle: Project Elements and XML Structure
ms:assetid: 23b2326a-66cf-4978-a982-48567ded715b
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968439(v=office.12)
ms:contentKeyID: 13188132
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

# Project Elements and XML Structure




This section contains information about the Project element and the children of Project defined in the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd). The elements represent project data when you save a project in the XML format.

## XML Structure of Project Elements

The following shows the XML structure of the elements defined by the Project schema section of mspdi\_pj12.xsd. The data type is indicated for those elements that require a text value. You can find more detailed information about valid text values for each element in the documentation annotations that are embedded in the [XML Schema for the Project Element](xml-schema-for-the-project-element.md).

For more information about the data types used in the Project 2007 XML Data Interchange Schema, see [Introduction to Project XML Data](introduction-to-project-xml-data.md).


> [!NOTE]
>   Detailed information about the structure of the OutlineCodes, WBSMasks, ExtendedAttributes, Calendars, Tasks, Resources, and Assignments elements are shown in separate topics in this schema reference.


\<[Project](project-element.md)\>

    \<[SaveVersion](saveversion-element.md)\>integer\</SaveVersion\>

    \<[UID](uid-element.md) \>string\</UID\>

    \<[Name](name-element.md)\>string\</Name\>

    \<[Title](title-element-project.md)\>string\</Title\>

    \<[Subject](subject-element.md)\>string\</Subject\>

    \<[Category](category-element.md)\>string\</Category\>

    \<[Company](company-element.md)\>string\</Company\>

    \<[Manager](manager-element.md)\>string\</Manager\>

    \<[Author](author-element.md)\>string\</Author\>

    \<[CreationDate](creationdate-element.md)\>dateTime\</CreationDate\>

    \<[Revision](revision-element.md)\>integer\</Revision\>

    \<[LastSaved](lastsaved-element.md)\>dateTime\</LastSaved\>

    \<[ScheduleFromStart](schedulefromstart-element.md)\>boolean\</ScheduleFromStart\>

    \<[StartDate](startdate-element.md)\>dateTime\</StartDate\>

    \<[FinishDate](finishdate-element.md)\>dateTime\</FinishDate\>

    \<[FYStartDate](fystartdate-element.md)\>integer\</FYStartDate\>

    \<[CriticalSlackLimit](criticalslacklimit-element.md)\>integer\</CriticalSlackLimit\>

    \<[CurrencyDigits](currencydigits-element.md)\>integer\</CurrencyDigits\>

    \<[CurrencySymbol](currencysymbol-element.md)\>string\</CurrencySymbol\>

    \<[CurrencyCode](currencycode-element.md) \>string\</CurrencyCode\>

    \<[CurrencySymbolPosition](currencysymbolposition-element.md)\>integer\</CurrencySymbolPosition\>

    \<[CalendarUID](calendaruid-element.md)\>integer\</CalendarUID\>

    \<[DefaultStartTime](defaultstarttime-element.md)\>time\</DefaultStartTime\>

    \<[DefaultFinishTime](defaultfinishtime-element.md)\>time\</DefaultFinishTime\>

    \<[MinutesPerDay](minutesperday-element.md)\>integer\</MinutesPerDay\>

    \<[MinutesPerWeek](minutesperweek-element.md)\>integer\</MinutesPerWeek\>

    \<[DaysPerMonth](dayspermonth-element.md)\>integer\</DaysPerMonth\>

    \<[DefaultTaskType](defaulttasktype-element.md)\>integer\</DefaultTaskType\>

    \<[DefaultFixedCostAccrual](defaultfixedcostaccrual-element.md)\>integer\</DefaultFixedCostAccrual\>

    \<[DefaultStandardRate](defaultstandardrate-element.md)\>float\</DefaultStandardRate\>

    \<[DefaultOvertimeRate](defaultovertimerate-element.md)\>float\</DefaultOvertimeRate\>

    \<[DurationFormat](durationformat-element.md)\>integer\</DurationFormat\>

    \<[WorkFormat](workformat-element.md)\>integer\</WorkFormat\>

    \<[EditableActualCosts](editableactualcosts-element.md)\>boolean\</EditableActualCosts\>

    \<[HonorConstraints](honorconstraints-element.md)\>boolean\</HonorConstraints\>

    \<[EarnedValueMethod](earnedvaluemethod-element.md)\>integer\</EarnedValueMethod\>

    \<[InsertedProjectsLikeSummary](insertedprojectslikesummary-element.md)\>boolean\</InsertedProjectsLikeSummary\>

    \<[MultipleCriticalPaths](multiplecriticalpaths-element.md)\>boolean\</MultipleCriticalPaths\>

    \<[NewTasksEffortDriven](newtaskseffortdriven-element.md)\>boolean\</NewTasksEffortDriven\>

    \<[NewTasksEstimated](newtasksestimated-element.md)\>boolean\</NewTasksEstimated\>

    \<[SplitsInProgressTasks](splitsinprogresstasks-element.md)\>boolean\</SplitsInProgressTasks\>

    \<[SpreadActualCost](spreadactualcost-element.md)\>boolean\</SpreadActualCost\>

    \<[SpreadPercentComplete](spreadpercentcomplete-element.md)\>boolean\</SpreadPercentComplete\>

    \<[TaskUpdatesResource](taskupdatesresource-element.md)\>boolean\</TaskUpdatesResource\>

    \<[FiscalYearStart](fiscalyearstart-element.md)\>boolean\</FiscalYearStart\>

    \<[WeekStartDay](weekstartday-element.md)\>integer\</WeekStartDay\>

    \<[MoveCompletedEndsBack](movecompletedendsback-element.md)\>boolean\</MoveCompletedEndsBack\>

    \<[MoveRemainingStartsBack](moveremainingstartsback-element.md)\>boolean\</MoveRemainingStartsBack\>

    \<[MoveRemainingStartsForward](moveremainingstartsforward-element.md)\>boolean\</MoveRemainingStartsForward\>

    \<[MoveCompletedEndsForward](movecompletedendsforward-element.md)\>boolean\</MoveCompletedEndsForward\>

    \<[BaselineForEarnedValue](baselineforearnedvalue-element.md)\>integer\</BaselineForEarnedValue\>

    \<[AutoAddNewResourcesAndTasks](autoaddnewresourcesandtasks-element.md)\>boolean\</AutoAddNewResourcesAndTasks\>

    \<[StatusDate](statusdate-element.md)\>dateTime\</StatusDate\>

    \<[CurrentDate](currentdate-element.md)\>dateTime\</CurrentDate\>

    \<[MicrosoftProjectServerURL](microsoftprojectserverurl-element.md)\>boolean\</MicrosoftProjectServerURL\>

    \<[Autolink](autolink-element.md)\>boolean\</Autolink\>

    \<[NewTaskStartDate](newtaskstartdate-element.md)\>integer\</NewTaskStartDate\>

    \<[DefaultTaskEVMethod](defaulttaskevmethod-element.md)\>integer\</DefaultTaskEVMethod\>

    \<[ProjectExternallyEdited](projectexternallyedited-element.md)\>boolean\</ProjectExternallyEdited\>

    \<[ExtendedCreationDate](extendedcreationdate-element.md)\>dateTime\</ExtendedCreationDate\>

    \<[ActualsInSync](actualsinsync-element.md)\>boolean\</ActualsInSync\>

    \<[RemoveFileProperties](removefileproperties-element.md)\>boolean\</RemoveFileProperties\>

    \<[AdminProject](adminproject-element.md)\>boolean\</AdminProject\>

    \<[OutlineCodes](outlinecode-elements-and-xml-structure.md)\> . . . \</OutlineCodes\>

    \<[WBSMasks](wbsmask-elements-and-xml-structure.md)\> . . . \</WBSMasks\>

    \<[ExtendedAttributes](extendedattribute-elements-and-xml-structure.md)…\</ExtendedAttributes\>

    \<[Calendars](calendar-elements-and-xml-structure.md)\> . . . \</Calendars\>

    \<[Tasks](task-elements-and-xml-structure.md)\> . . . \</Tasks\>

    \<[Resources](resource-elements-and-xml-structure.md)\> . . . \</Resources\>

    \<[Assignments](assignment-elements-and-xml-structure.md)\> . . . \</Assignments\>

\</Project\>

## See Also

#### Concepts

[Introduction to Project XML Data](introduction-to-project-xml-data.md)

[XML Schema for the Project Element](xml-schema-for-the-project-element.md)

[OutlineCode Elements and XML Structure](outlinecode-elements-and-xml-structure.md)

[WBSMask Elements and XML Structure](wbsmask-elements-and-xml-structure.md)

[ExtendedAttribute Elements and XML Structure](extendedattribute-elements-and-xml-structure.md)

[Calendar Elements and XML Structure](calendar-elements-and-xml-structure.md)

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[Resource Elements and XML Structure](resource-elements-and-xml-structure.md)

[Assignment Elements and XML Structure](assignment-elements-and-xml-structure.md)

[TimephasedDataType Elements and XML Structure](timephaseddatatype-elements-and-xml-structure.md)

