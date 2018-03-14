---
title: Assignment Elements and XML Structure
TOCTitle: Assignment Elements and XML Structure
ms:assetid: f74cca91-ea2a-478d-b935-528b25dddaa8
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968738(v=office.12)
ms:contentKeyID: 13188428
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
---

# Assignment Elements and XML Structure




This section contains information about children of the Assignments element defined in the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd). The elements represent assignment data when you save a project in the XML format.

Assignments is a child of the Project element. For more information, see [Project Elements and XML Structure](project-elements-and-xml-structure.md).

## XML Structure of Assignment Elements

The following shows the XML structure of the elements defined by the Assignment schema section of mspdi\_pj12.xsd. The data type is indicated for those elements that require a text value. You can find more detailed information about valid text values for each element in the documentation annotations that are embedded in the [XML Schema for the Assignments Element](xml-schema-for-the-assignments-element.md).

For more information about the data types used in the Project 2007 XML Data Interchange Schema, see [Introduction to Project XML Data](introduction-to-project-xml-data.md).

Many of the Assignment elements represent data fields in Microsoft Office Project Professional 2007. For more information about fields in Project Professional 2007 and Project Standard 2007, see [Fields Reference](http://office.microsoft.com/en-us/project/ch100788901033.aspx).


> [!NOTE]
>    Detailed information about the structure of the TimephasedData element is shown in <A href="https://msdn.microsoft.com/en-us/library/317823-7111-4dfd-ae38-50a06c6cb70f(v=office.12)">TimephasedDataType Elements and XML Structure</A> in this schema reference.


\<[Assignments](assignments-element.md)\>

    \<[Assignment](assignment-element.md)\>

        \<[UID](uid-element.md)\>integer\</UID\>

        \<[TaskUID](taskuid-element.md)\>integer\</TaskUID\>

        \<[ResourceUID](resourceuid-element.md)\>integer\</ResourceUID\>

        \<[PercentWorkComplete](percentworkcomplete-element.md)\>integer\</PercentWorkComplete\>

        \<[ActualCost](actualcost-element.md)\>decimal\</ActualCost\>

        \<[ActualFinish](actualfinish-element.md)\>dateTime\</ActualFinish\>

        \<[ActualOvertimeCost](actualovertimecost-element.md)\>decimal\</ActualOvertimeCost\>

        \<[ActualOvertimeWork](actualovertimework-element.md)\>duration\</ActualOvertimeWork\>

        \<[ActualStart](actualstart-element.md)\>dateTime\</ActualStart\>

        \<[ActualWork](actualwork-element.md)\>duration\</ActualWork\>

        \<[ACWP](acwp-element.md)\>float\</ACWP\>

        \<[Confirmed](confirmed-element.md)\>boolean\</Confirmed\>

        \<[Cost](cost-element.md)\>decimal\</Cost\>

        \<[CostRateTable](costratetable-element.md)\>integer\</CostRateTable\>

        \<[CostVariance](costvariance-element.md)\>float\</CostVariance\>

        \<[CV](cv-element.md)\>float\</CV\>

        \<[Delay](delay-element.md)\>integer\</Delay\>

        \<[Finish](finish-element.md)\>dateTime\</Finish\>

        \<[FinishVariance](finishvariance-element.md)\>integer\</FinishVariance\>

        \<[Hyperlink](hyperlink-element.md)\>string\</Hyperlink\>

        \<[HyperlinkAddress](hyperlinkaddress-element.md)\>string\</HyperlinkAddress\>

        \<[HyperlinkSubAddress](hyperlinksubaddress-element.md)\>string\</HyperlinkSubAddress\>

        \<[WorkVariance](workvariance-element.md)\>float\</WorkVariance\>

        \<[HasFixedRateUnits](hasfixedrateunits-element.md)\>boolean\</HasFixedRateUnits\>

        \<[FixedMaterial](fixedmaterial-element.md)\>boolean\</FixedMaterial\>

        \<[LevelingDelay](levelingdelay-element.md)\>integer\</LevelingDelay\>

        \<[LevelingDelayFormat](levelingdelayformat-element.md)\>integer\</LevelingDelayFormat\>

        \<[LinkedFields](linkedfields-element.md)\>boolean\</LinkedFields\>

        \<[Milestone](milestone-element.md)\>boolean\</Milestone\>

        \<[Notes](notes-element.md)\>string\</Notes\>

        \<[OverAllocated](overallocated-element.md)\>boolean\</Overallocated\>

        \<[OvertimeCost](overtimecost-element.md)\>decimal\</OvertimeCost\>

        \<[OvertimeWork](overtimework-element.md)\>duration\</OvertimeWork\>

        \<[PeakUnits](peakunits-element.md)\>float\</PeakUnits\>

        \<[RegularWork](regularwork-element.md)\>duration\</RegularWork\>

        \<[RemainingCost](remainingcost-element.md)\>decimal\</RemainingCost\>

        \<[RemainingOvertimeCost](remainingovertimecost-element.md)\>decimal\</RemainingOvertimeCost\>

        \<[RemainingOvertimeWork](remainingovertimework-element.md)\>duration\</RemainingOvertimeWork\>

        \<[RemainingWork](remainingwork-element.md)\>duration\</RemainingWork\>

        \<[ResponsePending](responsepending-element.md)\>boolean\</ResponsePending\>

        \<[Start](start-element.md)\>dateTime\</Start\>

        \<[Stop](stop-element.md)\>dateTime\</Stop\>

        \<[Resume](resume-element.md)\>dateTime\</Resume\>

        \<[StartVariance](startvariance-element.md)\>integer\</StartVariance\>

        \<[Summary](summary-element.md)\>boolean\</Summary\>

        \<[SV](sv-element.md)\>float\</SV\>

        \<[Units](units-element.md)\>float\</Units\>

        \<[UpdateNeeded](updateneeded-element.md)\>boolean\</UpdateNeeded\>

        \<[VAC](vac-element.md)\>float\</VAC\>

        \<[Work](work-element.md)\>duration\</Work\>

        \<[WorkContour](workcontour-element.md)\>integer\</WorkContour\>

        \<[BCWS](bcws-element.md)\>float\</BCWS\>

        \<[BCWP](bcwp-element.md)\>float\</BCWP\>

        \<[BookingType](bookingtype-element.md)\>integer\</BookingType\>

        \<[ActualWorkProtected](actualworkprotected-element.md)\>duration\</ActualWorkProtected\>

        \<[ActualOvertimeWorkProtected](actualovertimeworkprotected-element.md)\>duration\</ActualOvertimeWorkProtected\>

        \<[CreationDate](creationdate-element.md)\>dateTime\</CreationDate\>

        \<[AssnOwner](assnowner-element.md)\>string\</AssnOwner\>

        \<[AssnOwnerGuid](assnownerguid-element.md)\>string\</AssnOwnerGuid\>

        \<[BudgetCost](budgetcost-element.md)\>decimal\</BudgetCost\>

        \<[BudgetWork](budgetwork-element.md)\>duration\</BudgetWork\>

        \<[ExtendedAttribute](extendedattribute-element.md)\>

            \<[FieldID](fieldid-element.md)\>string\</FieldID\>

            \<[Value](value-element.md)\>string\</ValueID\>

            \<[ValueGUID](valueguid-element.md)\>string\</UID\>

            \<[DurationFormat](durationformat-element.md)\>integer\</ValueID\>

        \</ExtendedAttribute\>

        \<[Baseline](baseline-element.md)\>

            [\<TimephasedData\>](timephaseddatatype-elements-and-xml-structure.md)…\</TimephasedData\>        

            \<[Number](number-element.md)\>string\</Number\>

            \<[Start](start-element.md)\>string\</Start\>

            \<[Finish](finish-element.md)\>string\</Finish\>

            \<[Work](work-element.md)\>duration\</Work\>

            \<[Cost](cost-element.md)\>string\</Cost\>

            \<[BCWS](bcws-element.md)\>float\</BCWS\>

            \<[BCWP](bcwp-element.md)\>float\</BCWP\>

        \</Baseline\>    

        \<\!-- \#\#New Project 2007 assignment enterprise custom field elements are written here. See [Custom Field Data in XML](custom-field-data-in-xml.md) for more information. --\>    

        \<f404000\>variable data type\</f404000\>        \<\!-- See [f404000 - f4040c8 Elements](f404000-f4040c8-elements.md) --\>

        . . .

        \<f4040c8\>variable data type\</f4040c8\>

        \<f408000\>variable data type\</f408000\>        \<\!-- See [f408000 - f417fff Elements](f408000-f417fff-elements.md) --\>

        . . .

        \<f417fff\>variable data type\</f417fff\>

        \<[TimephasedData](timephaseddata-element.md)\>. . .\</TimephasedData\>

    \</Assignment\>

\</Assignments\>

## See Also

#### Reference

[TimephasedDataType Elements and XML Structure](https://msdn.microsoft.com/en-us/library/317823-7111-4dfd-ae38-50a06c6cb70f\(v=office.12\))

#### Concepts

[Introduction to Project XML Data](introduction-to-project-xml-data.md)

[XML Schema for the Assignments Element](xml-schema-for-the-assignments-element.md)

[Custom Field Data in XML](custom-field-data-in-xml.md)

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

#### Other Resources

[Fields Reference](http://office.microsoft.com/en-us/project/ch100788901033.aspx)

