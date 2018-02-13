---
title: Task Elements and XML Structure
TOCTitle: Task Elements and XML Structure
ms:assetid: 3fa5904f-841c-421b-bfdd-cb9531c8bdf7
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968475(v=office.12)
ms:contentKeyID: 13188167
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

# Task Elements and XML Structure

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

This section contains information about children of the Tasks element defined in the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd). The elements represent task data when you save a project in the XML format.

Tasks is a child of the Project element. For more information, see [Project Elements and XML Structure](bb968439\(v=office.12\).md).

## XML Structure of Task Elements

The following shows the XML structure of the elements defined by the Task schema section of mspdi\_pj12.xsd. The data type is indicated for those elements that require a text value. You can find more detailed information about valid text values for each element in the documentation annotations that are embedded in the [Task Schema](bb968415\(v=office.12\).md).

For more information about the data types used in the Project 2007 XML Data Interchange Schema, see [Introduction to Project XML Data](bb968652\(v=office.12\).md).

Many of the Task elements represent data fields in Microsoft Office Project. For more information about fields in Project Professional 2007 and Project Standard 2007, see [Fields Reference](http://office.microsoft.com/en-us/project/ch100788901033.aspx).


> [!NOTE]
> Detailed information about the structure of the TimephasedData element is shown in <A href="https://msdn.microsoft.com/en-us/library/317823-7111-4dfd-ae38-50a06c6cb70f(v=office.12)">TimephasedDataType Elements and XML Structure</A> in this schema reference.


\<[Tasks](bb968617\(v=office.12\).md)\>

    \<[Task](bb968487\(v=office.12\).md)\>

        \<[UID](bb968590\(v=office.12\).md)\>integer\</UID\>

        \<[ID](bb968437\(v=office.12\).md)\>integer\</ID\>

        \<[Name](bb968600\(v=office.12\).md)\>string\</Name\>

        \<[Type](bb968434\(v=office.12\).md)\>integer\</Type\>

        \<[IsNull](bb968682\(v=office.12\).md)\>boolean\<IsNull\>

        \<[CreateDate](bb968422\(v=office.12\).md)\>dateTime\</CreateDate\>

        \<[Contact](bb968485\(v=office.12\).md)\>string\</Contact\>

        \<[WBS](bb968566\(v=office.12\).md)\>string\</WBS\>

        \<[WBSLevel](bb968653\(v=office.12\).md)\>string\<WBSLevel\>

        \<[OutlineNumber](bb968651\(v=office.12\).md)\>string\</OutlineNumber\>

        \<[OutlineLevel](bb968465\(v=office.12\).md)\>integer\</OutlineLevel\>

        \<[Priority](bb968643\(v=office.12\).md)\>integer\</Priority\>

        \<[Start](bb968645\(v=office.12\).md)\>dateTime\</Start\>

        \<[Finish](bb968534\(v=office.12\).md)\>dateTime\</Finish\>

        \<[Duration](bb968640\(v=office.12\).md)\>duration\</Duration\>

        \<[DurationFormat](bb968637\(v=office.12\).md)\>integer\</DurationFormat\>

        \<[Work](bb968571\(v=office.12\).md)\>duration\</Work\>

        \<[Stop](bb968470\(v=office.12\).md)\>dateTime\</Stop\>

        \<[Resume](bb968423\(v=office.12\).md)\>dateTime\</Resume\>

        \<[ResumeValid](bb968677\(v=office.12\).md)\>boolean\</ResumeValid\>

        \<[EffortDriven](bb968574\(v=office.12\).md)\>boolean\</EffortDriven\>

        \<[Recurring](bb968731\(v=office.12\).md)\>boolean\</Recurring\>

        \<[OverAllocated](bb968615\(v=office.12\).md)\>boolean\</OverAllocated\>

        \<[Estimated](bb968711\(v=office.12\).md)\>boolean\</Estimated\>

        \<[Milestone](bb968520\(v=office.12\).md)\>boolean\</Milestone\>

        \<[Summary](bb968468\(v=office.12\).md)\>boolean\</Summary\>

        \<[Critical](bb968692\(v=office.12\).md)\>boolean\</Critical\>

        \<[IsSubproject](bb968630\(v=office.12\).md)\>boolean\</IsSubproject\>

        \<[IsSubprojectReadOnly](bb968461\(v=office.12\).md)\>boolean\</IsSubprojectReadOnly\>

        \<[SubprojectName](bb968656\(v=office.12\).md)\>string\</SubprojectName\>

        \<[ExternalTask](bb968595\(v=office.12\).md)\>boolean\</ExternalTask\>

        \<[ExternalTaskProject](bb968537\(v=office.12\).md)\>string\</ExternalTaskProject\>

        \<[EarlyStart](bb968432\(v=office.12\).md)\>dateTime\</EarlyStart\>

        \<[EarlyFinish](bb968483\(v=office.12\).md)\>dateTime\</EarlyFinish\>

        \<[LateStart](bb968576\(v=office.12\).md)\>dateTime\</LateStart\>

        \<[LateFinish](bb968671\(v=office.12\).md)\>dateTime\</LateFinish\>

        \<[StartVariance](bb968588\(v=office.12\).md)\>integer\</StartVariance\>

        \<[FinishVariance](bb968724\(v=office.12\).md)\>integer\</FinishVariance\>

        \<[WorkVariance](bb968689\(v=office.12\).md)\>float\</WorkVariance\>

        \<[FreeSlack](bb968623\(v=office.12\).md)\>integer\</FreeSlack\>

        \<[TotalSlack](bb968632\(v=office.12\).md)\>integer\</TotalSlack\>

        \<[FixedCost](bb968494\(v=office.12\).md)\>float\</FixedCost\>

        \<[FixedCostAccrual](bb968493\(v=office.12\).md)\>string\</FixedCostAccrual\>

        \<[PercentComplete](bb968546\(v=office.12\).md)\>integer\</PercentComplete\>

        \<[PercentWorkComplete](bb968608\(v=office.12\).md)\>integer\</PercentWorkComplete\>

        \<[Cost](bb968522\(v=office.12\).md)\>decimal\</Cost\>

        \<[OvertimeCost](bb968407\(v=office.12\).md)\>decimal\</OvertimeCost\>

        \<[OvertimeWork](bb968609\(v=office.12\).md)\>duration\</OvertimeWork\>

        \<[ActualStart](bb968713\(v=office.12\).md)\>dateTime\<ActualStart\>

        \<[ActualFinish](bb968472\(v=office.12\).md)\>dateTime\</ActualFinish\>

        \<[ActualDuration](bb968446\(v=office.12\).md)\>duration\</ActualDuration\>

        \<[ActualCost](bb968591\(v=office.12\).md)\>decimal\</ActualCost\>

        \<[ActualOvertimeCost](bb968431\(v=office.12\).md)\>decimal\</ActualOvertimeCost\>

        \<[ActualWork](bb968429\(v=office.12\).md)\>duration\</ActualWork\>

        \<[ActualOvertimeWork](bb968413\(v=office.12\).md)\>duration\</ActualOvertimeWork\>

        \<[RegularWork](bb968582\(v=office.12\).md)\>duration\</RegularWork\>

        \<[RemainingDuration](bb968613\(v=office.12\).md)\>duration\</RemainingDuration\>

        \<[RemainingCost](bb968728\(v=office.12\).md)\>decimal\</RemainingCost\>

        \<[RemainingWork](bb968720\(v=office.12\).md)\>duration\</RemainingWork\>

        \<[RemainingOvertimeCost](bb968690\(v=office.12\).md)\>decimal\</RemainingOvertimeCost\>

        \<[RemainingOvertimeWork](bb968473\(v=office.12\).md)\>duration\</RemainingOvertimeWork\>

        \<[ACWP](bb968717\(v=office.12\).md)\>float\</ACWP\>

        \<[CV](bb968685\(v=office.12\).md)\>float\</CV\>

        \<[ConstraintType](bb968703\(v=office.12\).md)\>integer\</ConstraintType\>

        \<[CalendarUID](bb968514\(v=office.12\).md)\>integer\</CalendarUID\>

        \<[ConstraintDate](bb968552\(v=office.12\).md)\>dateTime\</ConstraintDate\>

        \<[Deadline](bb968639\(v=office.12\).md)\>dateTime\</Deadline\>

        \<[LevelAssignments](bb968452\(v=office.12\).md)\>boolean\</LevelAssignments\>

        \<[LevelingCanSplit](bb968467\(v=office.12\).md)\>boolean\</LevelingCanSplit\>

        \<[LevelingDelay](bb968397\(v=office.12\).md)\>integer\</LevelingDelay\>

        \<[LevelingDelayFormat](bb968448\(v=office.12\).md)\>integer\</LevelingDelayFormat\>

        \<[PreLeveledStart](bb968725\(v=office.12\).md)\>dateTime\</PreLeveledStart\>

        \<[PreLeveledFinish](bb968501\(v=office.12\).md)\>dateTime\</PreLeveledFinish\>

        \<[Hyperlink](bb968729\(v=office.12\).md)\>string\</Hyperlink\>

        \<[HyperlinkAddress](bb968561\(v=office.12\).md)\>string\</HyperlinkAddress\>

        \<[HyperlinkSubAddress](bb968602\(v=office.12\).md)\>string\</HyperlinkSubAddress\>

        \<[IgnoreResourceCalendar](bb968540\(v=office.12\).md)\>boolean\</IgnoreResourceCalendar\>

        \<[Notes](bb968616\(v=office.12\).md)\>string\</Notes\>

        \<[HideBar](bb968691\(v=office.12\).md)\>boolean\</HideBar\>

        \<[Rollup](bb968489\(v=office.12\).md)\>boolean\</Rollup\>

        \<[BCWS](bb968411\(v=office.12\).md)\>float\</BCWS\>

        \<[BCWP](bb968714\(v=office.12\).md)\>float\</BCWP\>

        \<[PhysicalPercentComplete](bb968424\(v=office.12\).md)\>integer\</PhysicalPercentComplete\>

        \<[EarnedValueMethod](bb968620\(v=office.12\).md)\>integer\</EarnedValueMethod\>

        \<[PredecessorLink](bb968712\(v=office.12\).md)\>

            \<[PredecessorUID](bb968447\(v=office.12\).md)\>integer\</PredecessorUID\>

            \<[Type](bb968434\(v=office.12\).md)\>integer\</Type\>

            \<[CrossProject](bb968586\(v=office.12\).md)\>boolean\</CrossProject\>

            \<[CrossProjectName](bb968597\(v=office.12\).md)\>string\</CrossProjectName\>

            \<[LinkLag](bb968558\(v=office.12\).md)\>integer\</LinkLag\>

            \<[LagFormat](bb968698\(v=office.12\).md)\>integer\</LagFormat\>

        \</PredecessorLink\>

        \<[ActualWorkProtected](bb968400\(v=office.12\).md)\>duration\</ActualWorkProtected\>

        \<[ActualOvertimeWorkProtected](bb968676\(v=office.12\).md)\>duration\</ActualOvertimeWorkProtected\>

        \<[ExtendedAttribute](bb968669\(v=office.12\).md)\>

            \<[UID](bb968590\(v=office.12\).md)\>integer\</UID\>

            \<[FieldID](bb968474\(v=office.12\).md)\>string\</FieldID\>

            \<[Value](bb968696\(v=office.12\).md)\>string\</Value\>

            \<[ValueID](bb968406\(v=office.12\).md)\>integer\</ValueID\>

            \<[DurationFormat](bb968637\(v=office.12\).md)\>integer\</DurationFormat\>

        \</ExtendedAttribute\>

        \<[Baseline](bb968599\(v=office.12\).md)\>

            [\<TimephasedData\>](bb968722\(v=office.12\).md)…\</TimephasedData\>

            \<[Number](bb968680\(v=office.12\).md)\>integer\</Number\>

            \<[Interim](bb968438\(v=office.12\).md)\>boolean\</Interim\>

            \<[Start](bb968645\(v=office.12\).md)\>dateTime\</Start\>

            \<[Finish](bb968534\(v=office.12\).md)\>dateTime\</Finish\>

            \<[Duration](bb968640\(v=office.12\).md)\>duration\</Duration\>

            \<[DurationFormat](bb968637\(v=office.12\).md)\>integer\</DurationFormat\>

            \<[EstimatedDuration](bb968697\(v=office.12\).md)\>boolean\</EstimatedDuration\>

            \<[Work](bb968571\(v=office.12\).md)\>duration\</Work\>

            \<[Cost](bb968522\(v=office.12\).md)\>decimal\</Cost\>

            \<[BCWS](bb968411\(v=office.12\).md)\>float\</BCWS\>

            \<[BCWP](bb968714\(v=office.12\).md)\>float\</BCWP\>

            \<[FixedCost](bb968494\(v=office.12\).md)\>float\</FixedCost\>

        \</Baseline\>

        \<[IsPublished](bb968507\(v=office.12\).md)\>boolean\</IsPublished\>

        \<[StatusManager](bb968633\(v=office.12\).md)\>string\</StatusManager\>

        \<[CommitmentStart](bb968530\(v=office.12\).md)\>dateTime\</CommitmentStart\>

        \<[CommitmentFinish](bb968464\(v=office.12\).md)\>dateTime\</CommitmentFinish\>

        \<[CommitmentType](bb968709\(v=office.12\).md)\>integer\</CommitmentType\>

        \<[b408000 – b417fff](bb968719\(v=office.12\).md)\>

                \<\!-- \#\#New Project 2007 enterprise task custom field data.

                        See [Custom Field Data in XML](bb968687\(v=office.12\).md) for more information. --\>

        \</b408000 – b417fff\>

        \<[b608000 – b617fff](bb968536\(v=office.12\).md)\>

                \<\!-- \#\#New Project 2007 enterprise project custom field data. --\>

        \</b608000 – b617fff\>

        \<[ExtendedAttribute](bb968669\(v=office.12\).md)\>

            \<[FieldID](bb968474\(v=office.12\).md)\>string\</FieldID\>

            \<[Value](bb968696\(v=office.12\).md)\>string\</ValueID\>

            \<[ValueGUID](bb968572\(v=office.12\).md)\>string\</UID\>

            \<[DurationFormat](bb968637\(v=office.12\).md)\>integer\</ValueID\>

        \</ExtendedAttribute\>

        \<[OutlineCode](bb968410\(v=office.12\).md)\>

            \<[FieldID](bb968474\(v=office.12\).md)\>string\</FieldID\>

            \<[ValueID](bb968406\(v=office.12\).md)\>integer\</ValueID\>

            \<[ValueGUID](bb968572\(v=office.12\).md)\>string\</UID\>

        \</OutlineCode\>

        \<[TimephasedData](bb968479\(v=office.12\).md)\>. . .\</TimephasedData\>

    \</Task\>

\</Tasks\>

## See Also

#### Reference

[TimephasedDataType Elements and XML Structure](https://msdn.microsoft.com/en-us/library/317823-7111-4dfd-ae38-50a06c6cb70f\(v=office.12\))

#### Concepts

[Introduction to Project XML Data](bb968652\(v=office.12\).md)

[XML Schema for the Tasks Element](bb968415\(v=office.12\).md)

[Custom Field Data in XML](bb968687\(v=office.12\).md)

[Project Elements and XML Structure](bb968439\(v=office.12\).md)

#### Other Resources

[Fields Reference](http://office.microsoft.com/en-us/project/ch100788901033.aspx)

