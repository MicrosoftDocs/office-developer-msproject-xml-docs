---
title: Assignment Elements and XML Structure
TOCTitle: Assignment Elements and XML Structure
ms:assetid: f74cca91-ea2a-478d-b935-528b25dddaa8
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968738(v=office.12)
ms:contentKeyID: 13188428
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
---

# Assignment Elements and XML Structure

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

This section contains information about children of the Assignments element defined in the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd). The elements represent assignment data when you save a project in the XML format.

Assignments is a child of the Project element. For more information, see [Project Elements and XML Structure](bb968439\(v=office.12\).md).

## XML Structure of Assignment Elements

The following shows the XML structure of the elements defined by the Assignment schema section of mspdi\_pj12.xsd. The data type is indicated for those elements that require a text value. You can find more detailed information about valid text values for each element in the documentation annotations that are embedded in the [XML Schema for the Assignments Element](bb968414\(v=office.12\).md).

For more information about the data types used in the Project 2007 XML Data Interchange Schema, see [Introduction to Project XML Data](bb968652\(v=office.12\).md).

Many of the Assignment elements represent data fields in Microsoft Office Project Professional 2007. For more information about fields in Project Professional 2007 and Project Standard 2007, see [Fields Reference](http://office.microsoft.com/en-us/project/ch100788901033.aspx).


> [!NOTE]
>    Detailed information about the structure of the TimephasedData element is shown in <A href="https://msdn.microsoft.com/en-us/library/317823-7111-4dfd-ae38-50a06c6cb70f(v=office.12)">TimephasedDataType Elements and XML Structure</A> in this schema reference.


\<[Assignments](bb968684\(v=office.12\).md)\>

    \<[Assignment](bb968611\(v=office.12\).md)\>

        \<[UID](bb968590\(v=office.12\).md)\>integer\</UID\>

        \<[TaskUID](bb968646\(v=office.12\).md)\>integer\</TaskUID\>

        \<[ResourceUID](bb968535\(v=office.12\).md)\>integer\</ResourceUID\>

        \<[PercentWorkComplete](bb968608\(v=office.12\).md)\>integer\</PercentWorkComplete\>

        \<[ActualCost](bb968591\(v=office.12\).md)\>decimal\</ActualCost\>

        \<[ActualFinish](bb968472\(v=office.12\).md)\>dateTime\</ActualFinish\>

        \<[ActualOvertimeCost](bb968431\(v=office.12\).md)\>decimal\</ActualOvertimeCost\>

        \<[ActualOvertimeWork](bb968413\(v=office.12\).md)\>duration\</ActualOvertimeWork\>

        \<[ActualStart](bb968713\(v=office.12\).md)\>dateTime\</ActualStart\>

        \<[ActualWork](bb968429\(v=office.12\).md)\>duration\</ActualWork\>

        \<[ACWP](bb968717\(v=office.12\).md)\>float\</ACWP\>

        \<[Confirmed](bb968559\(v=office.12\).md)\>boolean\</Confirmed\>

        \<[Cost](bb968522\(v=office.12\).md)\>decimal\</Cost\>

        \<[CostRateTable](bb968541\(v=office.12\).md)\>integer\</CostRateTable\>

        \<[CostVariance](bb968683\(v=office.12\).md)\>float\</CostVariance\>

        \<[CV](bb968685\(v=office.12\).md)\>float\</CV\>

        \<[Delay](bb968678\(v=office.12\).md)\>integer\</Delay\>

        \<[Finish](bb968534\(v=office.12\).md)\>dateTime\</Finish\>

        \<[FinishVariance](bb968724\(v=office.12\).md)\>integer\</FinishVariance\>

        \<[Hyperlink](bb968729\(v=office.12\).md)\>string\</Hyperlink\>

        \<[HyperlinkAddress](bb968561\(v=office.12\).md)\>string\</HyperlinkAddress\>

        \<[HyperlinkSubAddress](bb968602\(v=office.12\).md)\>string\</HyperlinkSubAddress\>

        \<[WorkVariance](bb968689\(v=office.12\).md)\>float\</WorkVariance\>

        \<[HasFixedRateUnits](bb968547\(v=office.12\).md)\>boolean\</HasFixedRateUnits\>

        \<[FixedMaterial](bb968521\(v=office.12\).md)\>boolean\</FixedMaterial\>

        \<[LevelingDelay](bb968397\(v=office.12\).md)\>integer\</LevelingDelay\>

        \<[LevelingDelayFormat](bb968448\(v=office.12\).md)\>integer\</LevelingDelayFormat\>

        \<[LinkedFields](bb968484\(v=office.12\).md)\>boolean\</LinkedFields\>

        \<[Milestone](bb968520\(v=office.12\).md)\>boolean\</Milestone\>

        \<[Notes](bb968616\(v=office.12\).md)\>string\</Notes\>

        \<[OverAllocated](bb968615\(v=office.12\).md)\>boolean\</Overallocated\>

        \<[OvertimeCost](bb968407\(v=office.12\).md)\>decimal\</OvertimeCost\>

        \<[OvertimeWork](bb968609\(v=office.12\).md)\>duration\</OvertimeWork\>

        \<[PeakUnits](bb968404\(v=office.12\).md)\>float\</PeakUnits\>

        \<[RegularWork](bb968582\(v=office.12\).md)\>duration\</RegularWork\>

        \<[RemainingCost](bb968728\(v=office.12\).md)\>decimal\</RemainingCost\>

        \<[RemainingOvertimeCost](bb968690\(v=office.12\).md)\>decimal\</RemainingOvertimeCost\>

        \<[RemainingOvertimeWork](bb968473\(v=office.12\).md)\>duration\</RemainingOvertimeWork\>

        \<[RemainingWork](bb968720\(v=office.12\).md)\>duration\</RemainingWork\>

        \<[ResponsePending](bb968477\(v=office.12\).md)\>boolean\</ResponsePending\>

        \<[Start](bb968645\(v=office.12\).md)\>dateTime\</Start\>

        \<[Stop](bb968470\(v=office.12\).md)\>dateTime\</Stop\>

        \<[Resume](bb968423\(v=office.12\).md)\>dateTime\</Resume\>

        \<[StartVariance](bb968588\(v=office.12\).md)\>integer\</StartVariance\>

        \<[Summary](bb968468\(v=office.12\).md)\>boolean\</Summary\>

        \<[SV](bb968647\(v=office.12\).md)\>float\</SV\>

        \<[Units](bb968642\(v=office.12\).md)\>float\</Units\>

        \<[UpdateNeeded](bb968735\(v=office.12\).md)\>boolean\</UpdateNeeded\>

        \<[VAC](bb968455\(v=office.12\).md)\>float\</VAC\>

        \<[Work](bb968571\(v=office.12\).md)\>duration\</Work\>

        \<[WorkContour](bb968726\(v=office.12\).md)\>integer\</WorkContour\>

        \<[BCWS](bb968411\(v=office.12\).md)\>float\</BCWS\>

        \<[BCWP](bb968714\(v=office.12\).md)\>float\</BCWP\>

        \<[BookingType](bb968505\(v=office.12\).md)\>integer\</BookingType\>

        \<[ActualWorkProtected](bb968400\(v=office.12\).md)\>duration\</ActualWorkProtected\>

        \<[ActualOvertimeWorkProtected](bb968676\(v=office.12\).md)\>duration\</ActualOvertimeWorkProtected\>

        \<[CreationDate](bb968396\(v=office.12\).md)\>dateTime\</CreationDate\>

        \<[AssnOwner](bb968408\(v=office.12\).md)\>string\</AssnOwner\>

        \<[AssnOwnerGuid](bb968551\(v=office.12\).md)\>string\</AssnOwnerGuid\>

        \<[BudgetCost](bb968532\(v=office.12\).md)\>decimal\</BudgetCost\>

        \<[BudgetWork](bb968506\(v=office.12\).md)\>duration\</BudgetWork\>

        \<[ExtendedAttribute](bb968669\(v=office.12\).md)\>

            \<[FieldID](bb968474\(v=office.12\).md)\>string\</FieldID\>

            \<[Value](bb968696\(v=office.12\).md)\>string\</ValueID\>

            \<[ValueGUID](bb968572\(v=office.12\).md)\>string\</UID\>

            \<[DurationFormat](bb968637\(v=office.12\).md)\>integer\</ValueID\>

        \</ExtendedAttribute\>

        \<[Baseline](bb968599\(v=office.12\).md)\>

            [\<TimephasedData\>](bb968722\(v=office.12\).md)…\</TimephasedData\>        

            \<[Number](bb968680\(v=office.12\).md)\>string\</Number\>

            \<[Start](bb968645\(v=office.12\).md)\>string\</Start\>

            \<[Finish](bb968534\(v=office.12\).md)\>string\</Finish\>

            \<[Work](bb968571\(v=office.12\).md)\>duration\</Work\>

            \<[Cost](bb968522\(v=office.12\).md)\>string\</Cost\>

            \<[BCWS](bb968411\(v=office.12\).md)\>float\</BCWS\>

            \<[BCWP](bb968714\(v=office.12\).md)\>float\</BCWP\>

        \</Baseline\>    

        \<\!-- \#\#New Project 2007 assignment enterprise custom field elements are written here. See [Custom Field Data in XML](bb968687\(v=office.12\).md) for more information. --\>    

        \<f404000\>variable data type\</f404000\>        \<\!-- See [f404000 - f4040c8 Elements](bb968556\(v=office.12\).md) --\>

        . . .

        \<f4040c8\>variable data type\</f4040c8\>

        \<f408000\>variable data type\</f408000\>        \<\!-- See [f408000 - f417fff Elements](bb968688\(v=office.12\).md) --\>

        . . .

        \<f417fff\>variable data type\</f417fff\>

        \<[TimephasedData](bb968479\(v=office.12\).md)\>. . .\</TimephasedData\>

    \</Assignment\>

\</Assignments\>

## See Also

#### Reference

[TimephasedDataType Elements and XML Structure](https://msdn.microsoft.com/en-us/library/317823-7111-4dfd-ae38-50a06c6cb70f\(v=office.12\))

#### Concepts

[Introduction to Project XML Data](bb968652\(v=office.12\).md)

[XML Schema for the Assignments Element](bb968414\(v=office.12\).md)

[Custom Field Data in XML](bb968687\(v=office.12\).md)

[Project Elements and XML Structure](bb968439\(v=office.12\).md)

#### Other Resources

[Fields Reference](http://office.microsoft.com/en-us/project/ch100788901033.aspx)

