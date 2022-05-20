---
title: Task Elements and XML Structure
TOCTitle: Task Elements and XML Structure
ms:assetid: 3fa5904f-841c-421b-bfdd-cb9531c8bdf7
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968475(v=office.12)
ms:contentKeyID: 13188167
ms.date: 03/14/2018
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
ms.localizationpriority: medium
---

# Task Elements and XML Structure




This section contains information about children of the Tasks element defined in the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd). The elements represent task data when you save a project in the XML format.

Tasks is a child of the Project element. For more information, see [Project Elements and XML Structure](project-elements-and-xml-structure.md).

## XML Structure of Task Elements

The following shows the XML structure of the elements defined by the Task schema section of mspdi\_pj12.xsd. The data type is indicated for those elements that require a text value. You can find more detailed information about valid text values for each element in the documentation annotations that are embedded in the [Task Schema](xml-schema-for-the-tasks-element.md).

For more information about the data types used in the Project 2007 XML Data Interchange Schema, see [Introduction to Project XML Data](introduction-to-project-xml-data.md).

Many of the Task elements represent data fields in Microsoft Office Project. For more information about fields in Project Professional 2007 and Project Standard 2007, see [Fields Reference](https://support.microsoft.com/office/available-fields-reference-615a4563-1cc3-40f4-b66f-1b17e793a460#ID0EBBD=Office_2007).


> [!NOTE]
> Detailed information about the structure of the TimephasedData element is shown in <A href="https://msdn.microsoft.com/en-us/library/317823-7111-4dfd-ae38-50a06c6cb70f(v=office.12)">TimephasedDataType Elements and XML Structure</A> in this schema reference.


\<[Tasks](tasks-element.md)\>

    \<[Task](task-element.md)\>

        \<[UID](uid-element.md)\>integer\</UID\>

        \<[ID](id-element.md)\>integer\</ID\>

        \<[Name](name-element.md)\>string\</Name\>

        \<[Type](type-element-multiple-parents.md)\>integer\</Type\>

        \<[IsNull](isnull-element.md)\>boolean\<IsNull\>

        \<[CreateDate](createdate-element.md)\>dateTime\</CreateDate\>

        \<[Contact](contact-element.md)\>string\</Contact\>

        \<[WBS](wbs-element.md)\>string\</WBS\>

        \<[WBSLevel](wbslevel-element.md)\>string\<WBSLevel\>

        \<[OutlineNumber](outlinenumber-element.md)\>string\</OutlineNumber\>

        \<[OutlineLevel](outlinelevel-element.md)\>integer\</OutlineLevel\>

        \<[Priority](priority-element.md)\>integer\</Priority\>

        \<[Start](start-element.md)\>dateTime\</Start\>

        \<[Finish](finish-element.md)\>dateTime\</Finish\>

        \<[Duration](duration-element.md)\>duration\</Duration\>

        \<[DurationFormat](durationformat-element.md)\>integer\</DurationFormat\>

        \<[Work](work-element.md)\>duration\</Work\>

        \<[Stop](stop-element.md)\>dateTime\</Stop\>

        \<[Resume](resume-element.md)\>dateTime\</Resume\>

        \<[ResumeValid](resumevalid-element.md)\>boolean\</ResumeValid\>

        \<[EffortDriven](effortdriven-element.md)\>boolean\</EffortDriven\>

        \<[Recurring](recurring-element.md)\>boolean\</Recurring\>

        \<[OverAllocated](overallocated-element.md)\>boolean\</OverAllocated\>

        \<[Estimated](estimated-element.md)\>boolean\</Estimated\>

        \<[Milestone](milestone-element.md)\>boolean\</Milestone\>

        \<[Summary](summary-element.md)\>boolean\</Summary\>

        \<[Critical](critical-element.md)\>boolean\</Critical\>

        \<[IsSubproject](issubproject-element.md)\>boolean\</IsSubproject\>

        \<[IsSubprojectReadOnly](issubprojectreadonly-element.md)\>boolean\</IsSubprojectReadOnly\>

        \<[SubprojectName](subprojectname-element.md)\>string\</SubprojectName\>

        \<[ExternalTask](externaltask-element.md)\>boolean\</ExternalTask\>

        \<[ExternalTaskProject](externaltaskproject-element.md)\>string\</ExternalTaskProject\>

        \<[EarlyStart](earlystart-element.md)\>dateTime\</EarlyStart\>

        \<[EarlyFinish](earlyfinish-element.md)\>dateTime\</EarlyFinish\>

        \<[LateStart](latestart-element.md)\>dateTime\</LateStart\>

        \<[LateFinish](latefinish-element.md)\>dateTime\</LateFinish\>

        \<[StartVariance](startvariance-element.md)\>integer\</StartVariance\>

        \<[FinishVariance](finishvariance-element.md)\>integer\</FinishVariance\>

        \<[WorkVariance](workvariance-element.md)\>float\</WorkVariance\>

        \<[FreeSlack](freeslack-element.md)\>integer\</FreeSlack\>

        \<[TotalSlack](totalslack-element.md)\>integer\</TotalSlack\>

        \<[FixedCost](fixedcost-element-baseline.md)\>float\</FixedCost\>

        \<[FixedCostAccrual](fixedcostaccrual-element.md)\>string\</FixedCostAccrual\>

        \<[PercentComplete](percentcomplete-element.md)\>integer\</PercentComplete\>

        \<[PercentWorkComplete](percentworkcomplete-element.md)\>integer\</PercentWorkComplete\>

        \<[Cost](cost-element.md)\>decimal\</Cost\>

        \<[OvertimeCost](overtimecost-element.md)\>decimal\</OvertimeCost\>

        \<[OvertimeWork](overtimework-element.md)\>duration\</OvertimeWork\>

        \<[ActualStart](actualstart-element.md)\>dateTime\<ActualStart\>

        \<[ActualFinish](actualfinish-element.md)\>dateTime\</ActualFinish\>

        \<[ActualDuration](actualduration-element.md)\>duration\</ActualDuration\>

        \<[ActualCost](actualcost-element.md)\>decimal\</ActualCost\>

        \<[ActualOvertimeCost](actualovertimecost-element.md)\>decimal\</ActualOvertimeCost\>

        \<[ActualWork](actualwork-element.md)\>duration\</ActualWork\>

        \<[ActualOvertimeWork](actualovertimework-element.md)\>duration\</ActualOvertimeWork\>

        \<[RegularWork](regularwork-element.md)\>duration\</RegularWork\>

        \<[RemainingDuration](remainingduration-element.md)\>duration\</RemainingDuration\>

        \<[RemainingCost](remainingcost-element.md)\>decimal\</RemainingCost\>

        \<[RemainingWork](remainingwork-element.md)\>duration\</RemainingWork\>

        \<[RemainingOvertimeCost](remainingovertimecost-element.md)\>decimal\</RemainingOvertimeCost\>

        \<[RemainingOvertimeWork](remainingovertimework-element.md)\>duration\</RemainingOvertimeWork\>

        \<[ACWP](acwp-element.md)\>float\</ACWP\>

        \<[CV](cv-element.md)\>float\</CV\>

        \<[ConstraintType](constrainttype-element.md)\>integer\</ConstraintType\>

        \<[CalendarUID](calendaruid-element.md)\>integer\</CalendarUID\>

        \<[ConstraintDate](constraintdate-element.md)\>dateTime\</ConstraintDate\>

        \<[Deadline](deadline-element.md)\>dateTime\</Deadline\>

        \<[LevelAssignments](levelassignments-element.md)\>boolean\</LevelAssignments\>

        \<[LevelingCanSplit](levelingcansplit-element.md)\>boolean\</LevelingCanSplit\>

        \<[LevelingDelay](levelingdelay-element.md)\>integer\</LevelingDelay\>

        \<[LevelingDelayFormat](levelingdelayformat-element.md)\>integer\</LevelingDelayFormat\>

        \<[PreLeveledStart](preleveledstart-element.md)\>dateTime\</PreLeveledStart\>

        \<[PreLeveledFinish](preleveledfinish-element.md)\>dateTime\</PreLeveledFinish\>

        \<[Hyperlink](hyperlink-element.md)\>string\</Hyperlink\>

        \<[HyperlinkAddress](hyperlinkaddress-element.md)\>string\</HyperlinkAddress\>

        \<[HyperlinkSubAddress](hyperlinksubaddress-element.md)\>string\</HyperlinkSubAddress\>

        \<[IgnoreResourceCalendar](ignoreresourcecalendar-element.md)\>boolean\</IgnoreResourceCalendar\>

        \<[Notes](notes-element.md)\>string\</Notes\>

        \<[HideBar](hidebar-element.md)\>boolean\</HideBar\>

        \<[Rollup](rollup-element.md)\>boolean\</Rollup\>

        \<[BCWS](bcws-element.md)\>float\</BCWS\>

        \<[BCWP](bcwp-element.md)\>float\</BCWP\>

        \<[PhysicalPercentComplete](physicalpercentcomplete-element.md)\>integer\</PhysicalPercentComplete\>

        \<[EarnedValueMethod](earnedvaluemethod-element.md)\>integer\</EarnedValueMethod\>

        \<[PredecessorLink](predecessorlink-element.md)\>

            \<[PredecessorUID](predecessoruid-element.md)\>integer\</PredecessorUID\>

            \<[Type](type-element-multiple-parents.md)\>integer\</Type\>

            \<[CrossProject](crossproject-element.md)\>boolean\</CrossProject\>

            \<[CrossProjectName](crossprojectname-element.md)\>string\</CrossProjectName\>

            \<[LinkLag](linklag-element.md)\>integer\</LinkLag\>

            \<[LagFormat](lagformat-element.md)\>integer\</LagFormat\>

        \</PredecessorLink\>

        \<[ActualWorkProtected](actualworkprotected-element.md)\>duration\</ActualWorkProtected\>

        \<[ActualOvertimeWorkProtected](actualovertimeworkprotected-element.md)\>duration\</ActualOvertimeWorkProtected\>

        \<[ExtendedAttribute](extendedattribute-element.md)\>

            \<[UID](uid-element.md)\>integer\</UID\>

            \<[FieldID](fieldid-element.md)\>string\</FieldID\>

            \<[Value](value-element.md)\>string\</Value\>

            \<[ValueID](valueid-element.md)\>integer\</ValueID\>

            \<[DurationFormat](durationformat-element.md)\>integer\</DurationFormat\>

        \</ExtendedAttribute\>

        \<[Baseline](baseline-element.md)\>

            [\<TimephasedData\>](timephaseddatatype-elements-and-xml-structure.md)…\</TimephasedData\>

            \<[Number](number-element.md)\>integer\</Number\>

            \<[Interim](interim-element.md)\>boolean\</Interim\>

            \<[Start](start-element.md)\>dateTime\</Start\>

            \<[Finish](finish-element.md)\>dateTime\</Finish\>

            \<[Duration](duration-element.md)\>duration\</Duration\>

            \<[DurationFormat](durationformat-element.md)\>integer\</DurationFormat\>

            \<[EstimatedDuration](estimatedduration-element.md)\>boolean\</EstimatedDuration\>

            \<[Work](work-element.md)\>duration\</Work\>

            \<[Cost](cost-element.md)\>decimal\</Cost\>

            \<[BCWS](bcws-element.md)\>float\</BCWS\>

            \<[BCWP](bcwp-element.md)\>float\</BCWP\>

            \<[FixedCost](fixedcost-element-baseline.md)\>float\</FixedCost\>

        \</Baseline\>

        \<[IsPublished](ispublished-element.md)\>boolean\</IsPublished\>

        \<[StatusManager](statusmanager-element.md)\>string\</StatusManager\>

        \<[CommitmentStart](commitmentstart-element.md)\>dateTime\</CommitmentStart\>

        \<[CommitmentFinish](commitmentfinish-element.md)\>dateTime\</CommitmentFinish\>

        \<[CommitmentType](commitmenttype-element.md)\>integer\</CommitmentType\>

        \<[b408000 – b417fff](b408000-b417fff-elements.md)\>

                \<\!-- \#\#New Project 2007 enterprise task custom field data.

                        See [Custom Field Data in XML](custom-field-data-in-xml.md) for more information. --\>

        \</b408000 – b417fff\>

        \<[b608000 – b617fff](b608000-b617fff-elements.md)\>

                \<\!-- \#\#New Project 2007 enterprise project custom field data. --\>

        \</b608000 – b617fff\>

        \<[ExtendedAttribute](extendedattribute-element.md)\>

            \<[FieldID](fieldid-element.md)\>string\</FieldID\>

            \<[Value](value-element.md)\>string\</ValueID\>

            \<[ValueGUID](valueguid-element.md)\>string\</UID\>

            \<[DurationFormat](durationformat-element.md)\>integer\</ValueID\>

        \</ExtendedAttribute\>

        \<[OutlineCode](outlinecode-element.md)\>

            \<[FieldID](fieldid-element.md)\>string\</FieldID\>

            \<[ValueID](valueid-element.md)\>integer\</ValueID\>

            \<[ValueGUID](valueguid-element.md)\>string\</UID\>

        \</OutlineCode\>

        \<[TimephasedData](timephaseddata-element.md)\>. . .\</TimephasedData\>

    \</Task\>

\</Tasks\>

## See Also

#### Reference

[TimephasedDataType Elements and XML Structure](https://msdn.microsoft.com/en-us/library/317823-7111-4dfd-ae38-50a06c6cb70f\(v=office.12\))

#### Concepts

[Introduction to Project XML Data](introduction-to-project-xml-data.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

[Custom Field Data in XML](custom-field-data-in-xml.md)

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

#### Other Resources

[Fields Reference](http://office.microsoft.com/en-us/project/ch100788901033.aspx)

