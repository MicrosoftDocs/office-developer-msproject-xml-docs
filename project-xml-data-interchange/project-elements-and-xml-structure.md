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

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

This section contains information about the Project element and the children of Project defined in the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd). The elements represent project data when you save a project in the XML format.

## XML Structure of Project Elements

The following shows the XML structure of the elements defined by the Project schema section of mspdi\_pj12.xsd. The data type is indicated for those elements that require a text value. You can find more detailed information about valid text values for each element in the documentation annotations that are embedded in the [XML Schema for the Project Element](bb968695\(v=office.12\).md).

For more information about the data types used in the Project 2007 XML Data Interchange Schema, see [Introduction to Project XML Data](bb968652\(v=office.12\).md).


> [!NOTE]
>   Detailed information about the structure of the OutlineCodes, WBSMasks, ExtendedAttributes, Calendars, Tasks, Resources, and Assignments elements are shown in separate topics in this schema reference.


\<[Project](bb968701\(v=office.12\).md)\>

    \<[SaveVersion](bb968654\(v=office.12\).md)\>integer\</SaveVersion\>

    \<[UID](bb968590\(v=office.12\).md) \>string\</UID\>

    \<[Name](bb968600\(v=office.12\).md)\>string\</Name\>

    \<[Title](bb968746\(v=office.12\).md)\>string\</Title\>

    \<[Subject](bb968657\(v=office.12\).md)\>string\</Subject\>

    \<[Category](bb968456\(v=office.12\).md)\>string\</Category\>

    \<[Company](bb968707\(v=office.12\).md)\>string\</Company\>

    \<[Manager](bb968670\(v=office.12\).md)\>string\</Manager\>

    \<[Author](bb968681\(v=office.12\).md)\>string\</Author\>

    \<[CreationDate](bb968396\(v=office.12\).md)\>dateTime\</CreationDate\>

    \<[Revision](bb968601\(v=office.12\).md)\>integer\</Revision\>

    \<[LastSaved](bb968736\(v=office.12\).md)\>dateTime\</LastSaved\>

    \<[ScheduleFromStart](bb968741\(v=office.12\).md)\>boolean\</ScheduleFromStart\>

    \<[StartDate](bb968562\(v=office.12\).md)\>dateTime\</StartDate\>

    \<[FinishDate](bb968517\(v=office.12\).md)\>dateTime\</FinishDate\>

    \<[FYStartDate](bb968568\(v=office.12\).md)\>integer\</FYStartDate\>

    \<[CriticalSlackLimit](bb968531\(v=office.12\).md)\>integer\</CriticalSlackLimit\>

    \<[CurrencyDigits](bb968638\(v=office.12\).md)\>integer\</CurrencyDigits\>

    \<[CurrencySymbol](bb968502\(v=office.12\).md)\>string\</CurrencySymbol\>

    \<[CurrencyCode](bb968575\(v=office.12\).md) \>string\</CurrencyCode\>

    \<[CurrencySymbolPosition](bb968631\(v=office.12\).md)\>integer\</CurrencySymbolPosition\>

    \<[CalendarUID](bb968514\(v=office.12\).md)\>integer\</CalendarUID\>

    \<[DefaultStartTime](bb968578\(v=office.12\).md)\>time\</DefaultStartTime\>

    \<[DefaultFinishTime](bb968593\(v=office.12\).md)\>time\</DefaultFinishTime\>

    \<[MinutesPerDay](bb968518\(v=office.12\).md)\>integer\</MinutesPerDay\>

    \<[MinutesPerWeek](bb968627\(v=office.12\).md)\>integer\</MinutesPerWeek\>

    \<[DaysPerMonth](bb968592\(v=office.12\).md)\>integer\</DaysPerMonth\>

    \<[DefaultTaskType](bb968603\(v=office.12\).md)\>integer\</DefaultTaskType\>

    \<[DefaultFixedCostAccrual](bb968743\(v=office.12\).md)\>integer\</DefaultFixedCostAccrual\>

    \<[DefaultStandardRate](bb968449\(v=office.12\).md)\>float\</DefaultStandardRate\>

    \<[DefaultOvertimeRate](bb968402\(v=office.12\).md)\>float\</DefaultOvertimeRate\>

    \<[DurationFormat](bb968637\(v=office.12\).md)\>integer\</DurationFormat\>

    \<[WorkFormat](bb968538\(v=office.12\).md)\>integer\</WorkFormat\>

    \<[EditableActualCosts](bb968544\(v=office.12\).md)\>boolean\</EditableActualCosts\>

    \<[HonorConstraints](bb968614\(v=office.12\).md)\>boolean\</HonorConstraints\>

    \<[EarnedValueMethod](bb968620\(v=office.12\).md)\>integer\</EarnedValueMethod\>

    \<[InsertedProjectsLikeSummary](bb968740\(v=office.12\).md)\>boolean\</InsertedProjectsLikeSummary\>

    \<[MultipleCriticalPaths](bb968750\(v=office.12\).md)\>boolean\</MultipleCriticalPaths\>

    \<[NewTasksEffortDriven](bb968412\(v=office.12\).md)\>boolean\</NewTasksEffortDriven\>

    \<[NewTasksEstimated](bb968708\(v=office.12\).md)\>boolean\</NewTasksEstimated\>

    \<[SplitsInProgressTasks](bb968513\(v=office.12\).md)\>boolean\</SplitsInProgressTasks\>

    \<[SpreadActualCost](bb968605\(v=office.12\).md)\>boolean\</SpreadActualCost\>

    \<[SpreadPercentComplete](bb968498\(v=office.12\).md)\>boolean\</SpreadPercentComplete\>

    \<[TaskUpdatesResource](bb968594\(v=office.12\).md)\>boolean\</TaskUpdatesResource\>

    \<[FiscalYearStart](bb968550\(v=office.12\).md)\>boolean\</FiscalYearStart\>

    \<[WeekStartDay](bb968442\(v=office.12\).md)\>integer\</WeekStartDay\>

    \<[MoveCompletedEndsBack](bb968457\(v=office.12\).md)\>boolean\</MoveCompletedEndsBack\>

    \<[MoveRemainingStartsBack](bb968650\(v=office.12\).md)\>boolean\</MoveRemainingStartsBack\>

    \<[MoveRemainingStartsForward](bb968418\(v=office.12\).md)\>boolean\</MoveRemainingStartsForward\>

    \<[MoveCompletedEndsForward](bb968463\(v=office.12\).md)\>boolean\</MoveCompletedEndsForward\>

    \<[BaselineForEarnedValue](bb968527\(v=office.12\).md)\>integer\</BaselineForEarnedValue\>

    \<[AutoAddNewResourcesAndTasks](bb968742\(v=office.12\).md)\>boolean\</AutoAddNewResourcesAndTasks\>

    \<[StatusDate](bb968628\(v=office.12\).md)\>dateTime\</StatusDate\>

    \<[CurrentDate](bb968629\(v=office.12\).md)\>dateTime\</CurrentDate\>

    \<[MicrosoftProjectServerURL](bb968553\(v=office.12\).md)\>boolean\</MicrosoftProjectServerURL\>

    \<[Autolink](bb968458\(v=office.12\).md)\>boolean\</Autolink\>

    \<[NewTaskStartDate](bb968699\(v=office.12\).md)\>integer\</NewTaskStartDate\>

    \<[DefaultTaskEVMethod](bb968440\(v=office.12\).md)\>integer\</DefaultTaskEVMethod\>

    \<[ProjectExternallyEdited](bb968674\(v=office.12\).md)\>boolean\</ProjectExternallyEdited\>

    \<[ExtendedCreationDate](bb968606\(v=office.12\).md)\>dateTime\</ExtendedCreationDate\>

    \<[ActualsInSync](bb968482\(v=office.12\).md)\>boolean\</ActualsInSync\>

    \<[RemoveFileProperties](bb968622\(v=office.12\).md)\>boolean\</RemoveFileProperties\>

    \<[AdminProject](bb968694\(v=office.12\).md)\>boolean\</AdminProject\>

    \<[OutlineCodes](bb968596\(v=office.12\).md)\> . . . \</OutlineCodes\>

    \<[WBSMasks](bb968416\(v=office.12\).md)\> . . . \</WBSMasks\>

    \<[ExtendedAttributes](bb968579\(v=office.12\).md)…\</ExtendedAttributes\>

    \<[Calendars](bb968563\(v=office.12\).md)\> . . . \</Calendars\>

    \<[Tasks](bb968475\(v=office.12\).md)\> . . . \</Tasks\>

    \<[Resources](bb968445\(v=office.12\).md)\> . . . \</Resources\>

    \<[Assignments](bb968738\(v=office.12\).md)\> . . . \</Assignments\>

\</Project\>

## See Also

#### Concepts

[Introduction to Project XML Data](bb968652\(v=office.12\).md)

[XML Schema for the Project Element](bb968695\(v=office.12\).md)

[OutlineCode Elements and XML Structure](bb968596\(v=office.12\).md)

[WBSMask Elements and XML Structure](bb968416\(v=office.12\).md)

[ExtendedAttribute Elements and XML Structure](bb968579\(v=office.12\).md)

[Calendar Elements and XML Structure](bb968563\(v=office.12\).md)

[Task Elements and XML Structure](bb968475\(v=office.12\).md)

[Resource Elements and XML Structure](bb968445\(v=office.12\).md)

[Assignment Elements and XML Structure](bb968738\(v=office.12\).md)

[TimephasedDataType Elements and XML Structure](bb968722\(v=office.12\).md)

