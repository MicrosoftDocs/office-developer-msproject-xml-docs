---
title: Resource Elements and XML Structure
TOCTitle: Resource Elements and XML Structure
ms:assetid: 26f69c99-50e8-49c5-80cf-1c81c0abefbd
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968445(v=office.12)
ms:contentKeyID: 13188137
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

# Resource Elements and XML Structure




This section contains information about children of the Resources element defined in the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd). The XML elements represent resource data when you save a project in the XML format.

Resources is a child of the Project element. For more information, see [Project Elements and XML Structure](bb968439\(v=office.12\).md).

## XML Structure of Resource Elements

The following shows the XML structure of the elements defined in the Resource schema section of mspdi\_pj12.xsd. The data type is indicated for those elements that require a text value. You can find more detailed information about valid text values for each element in the documentation annotations that are embedded in the [Resource Schema](bb968511\(v=office.12\).md).

For more information about the data types used in the Project2007 XML Data Interchange Schema, see [Introduction to Project XML Data](bb968652\(v=office.12\).md).

Many of the Resource elements represent data fields in Microsoft Office Project. For more information about fields in Project Professional 2007 and Project Standard 2007, see [Fields Reference](http://office.microsoft.com/en-us/project/ch100788901033.aspx).


> [!NOTE]
> Detailed information about the structure of the TimephasedData element is shown in <A href="https://msdn.microsoft.com/en-us/library/317823-7111-4dfd-ae38-50a06c6cb70f(v=office.12)">TimephasedDataType Elements and XML Structure</A> in this schema reference.


\<[Resources](bb968730\(v=office.12\).md)\>

    \<[Resource](bb968715\(v=office.12\).md)\>

        \<[UID](bb968590\(v=office.12\).md)\>integer\</UID\>

        \<[ID](bb968437\(v=office.12\).md)\>integer\</ID\>

        \<[Name](bb968600\(v=office.12\).md)\>string\</Name\>

        \<[Type](bb968434\(v=office.12\).md)\>integer\</Type\>

        \<[IsNull](bb968682\(v=office.12\).md)\>boolean\</IsNull\>

        \<[Initials](bb968658\(v=office.12\).md)\>string\</Initials\>

        \<[Phonetics](bb968636\(v=office.12\).md)\>string\</Phonetics\>

        \<[NTAccount](bb968430\(v=office.12\).md)\>string\</NTAccount\>

        \<[MaterialLabel](bb968598\(v=office.12\).md)\>string\</MaterialLabel\>

        \<[Code](bb968539\(v=office.12\).md)\>string\</Code\>

        \<[Group](bb968570\(v=office.12\).md)\>string\</Group\>

        \<[WorkGroup](bb968721\(v=office.12\).md)\>integer\</WorkGroup\>

        \<[EmailAddress](bb968510\(v=office.12\).md)\>string\</EmailAddress\>

        \<[Hyperlink](bb968729\(v=office.12\).md)\>string\</Hyperlink\>

        \<[HyperlinkAddress](bb968561\(v=office.12\).md)\>string\</HyperlinkAddress\>

        \<[HyperlinkSubAddress](bb968602\(v=office.12\).md)\>string\</HyperlinkSubAddress\>

        \<[MaxUnits](bb968589\(v=office.12\).md)\>float\</MaxUnits\>

        \<[PeakUnits](bb968404\(v=office.12\).md)\>float\</PeakUnits\>

        \<[OverAllocated](bb968615\(v=office.12\).md)\>boolean\</OverAllocated\>

        \<[AvailableFrom](bb968686\(v=office.12\).md)\>dateTime\</AvailableFrom\>

        \<[AvailableTo](bb968648\(v=office.12\).md)\>dateTime\</AvailableTo\>

        \<[Start](bb968645\(v=office.12\).md)\>dateTime\</Start\>

        \<[Finish](bb968534\(v=office.12\).md)\>dateTime\</Finish\>

        \<[CanLevel](bb968435\(v=office.12\).md)\>boolean\</CanLevel\>

        \<[AccrueAt](bb968660\(v=office.12\).md)\>integer\</AccrueAt\>

        \<[Work](bb968571\(v=office.12\).md)\>duration\</Work\>

        \<[RegularWork](bb968582\(v=office.12\).md)\>duration\</RegularWork\>

        \<[OvertimeWork](bb968609\(v=office.12\).md)\>duration\</OvertimeWork\>

        \<[ActualWork](bb968429\(v=office.12\).md)\>duration\</ActualWork\>

        \<[RemainingWork](bb968720\(v=office.12\).md)\>duration\</RemainingWork\>

        \<[ActualOvertimeWork](bb968413\(v=office.12\).md)\>duration\</ActualOvertimeWork\>

        \<[RemainingOvertimeWork](bb968473\(v=office.12\).md)\>duration\</RemainingOvertimeWork\>

        \<[PercentWorkComplete](bb968608\(v=office.12\).md)\>integer\</PercentWorkComplete\>

        \<[StandardRate](bb968453\(v=office.12\).md)\>decimal\</StandardRate\>

        \<[StandardRateFormat](bb968727\(v=office.12\).md)\>integer\</StandardRateFormat\>

        \<[Cost](bb968522\(v=office.12\).md)\>decimal\</Cost\>

        \<[OvertimeRate](bb968679\(v=office.12\).md)\>decimal\</OvertimeRate\>

        \<[OvertimeRateFormat](bb968737\(v=office.12\).md)\>integer\</OvertimeRateFormat\>

        \<[OvertimeCost](bb968407\(v=office.12\).md)\>decimal\</OvertimeCost\>

        \<[CostPerUse](bb968500\(v=office.12\).md)\>decimal\</CostPerUse\>

        \<[ActualCost](bb968591\(v=office.12\).md)\>decimal\</ActualCost\>

        \<[ActualOvertimeCost](bb968431\(v=office.12\).md)\>decimal\</ActualOvertimeCost\>

        \<[RemainingCost](bb968728\(v=office.12\).md)\>decimal\</RemainingCost\>

        \<[RemainingOvertimeCost](bb968690\(v=office.12\).md)\>decimal\</RemainingOvertimeCost\>

        \<[WorkVariance](bb968689\(v=office.12\).md)\>float\</WorkVariance\>

        \<[CostVariance](bb968683\(v=office.12\).md)\>float\</CostVariance\>

        \<[SV](bb968647\(v=office.12\).md)\>float\</SV\>

        \<[CV](bb968685\(v=office.12\).md)\>float\</CV\>

        \<[ACWP](bb968717\(v=office.12\).md)\>float\</ACWP\>

        \<[CalendarUID](bb968514\(v=office.12\).md)\>integer\</CalendarUID\>

        \<[Notes](bb968616\(v=office.12\).md)\>string\</Notes\>

        \<[BCWS](bb968411\(v=office.12\).md)\>float\</BCWS\>

        \<[BCWP](bb968714\(v=office.12\).md)\>float\</BCWP\>

        \<[IsGeneric](bb968577\(v=office.12\).md)\>boolean\</IsGeneric\>

        \<[IsInactive](bb968663\(v=office.12\).md)\>boolean\</IsInactive\>

        \<[IsEnterprise](bb968668\(v=office.12\).md)\>boolean\</IsEnterprise\>

        \<[BookingType](bb968505\(v=office.12\).md)\>integer\</BookingType\>

        \<[ActualWorkProtected](bb968400\(v=office.12\).md)\>duration\</ActualWorkProtected\>

        \<[ActualOvertimeWorkProtected](bb968676\(v=office.12\).md)\>duration\</ActualOvertimeWorkProtected\>

        \<[ActiveDirectoryGUID](bb968497\(v=office.12\).md)\>string\</ActiveDirectoryGUID\>

        \<[CreationDate](bb968396\(v=office.12\).md)\>dateTime\</CreationDate\>

        \<[ExtendedAttribute](bb968669\(v=office.12\).md)\>

            \<[UID](bb968590\(v=office.12\).md)\>integer\</UID\>

            \<[FieldID](bb968474\(v=office.12\).md)\>string\</FieldID\>

            \<[Value](bb968696\(v=office.12\).md)\>string\</Value\>

            \<[ValueID](bb968406\(v=office.12\).md)\>integer\</ValueID\>

            \<[DurationFormat](bb968637\(v=office.12\).md)\>integer\</DurationFormat\>

        \</ExtendedAttribute\>

        \<[Baseline](bb968599\(v=office.12\).md)\>

            \<[Number](bb968680\(v=office.12\).md)\>integer\</Number\>

            \<[Work](bb968571\(v=office.12\).md)\>duration\</Work\>

            \<[Cost](bb968522\(v=office.12\).md)\>float\</Cost\>

            \<[BCWS](bb968411\(v=office.12\).md)\>float\</BCWS\>

            \<[BCWP](bb968714\(v=office.12\).md)\>float\</BCWP\>

        \</Baseline\>

        \<[OutlineCode](bb968410\(v=office.12\).md)\>

            \<[UID](bb968590\(v=office.12\).md)\>integer\</UID\>

            \<[FieldID](bb968474\(v=office.12\).md)\>string\</FieldID\>

            \<[ValueID](bb968406\(v=office.12\).md)\>integer\</ValueID\>

        \</OutlineCode\>

        \<[IsCostResource](bb968549\(v=office.12\).md)\>boolean\</IsCostResource\>

        \<[AssnOwner](bb968408\(v=office.12\).md)\>string\</AssnOwner\>

        \<[AssnOwnerGuid](bb968551\(v=office.12\).md)\>string\</AssnOwnerGuid\>

        \<[IsBudget](bb968612\(v=office.12\).md)\>boolean\</IsBudget\>

        \<[AvailabilityPeriods](bb968747\(v=office.12\).md)\>

            \<[AvailabilityPeriod](bb968625\(v=office.12\).md)\>

                \<[AvailableFrom](bb968686\(v=office.12\).md)\>dateTime\</AvailableFrom\>

                \<[AvailableTo](bb968648\(v=office.12\).md)\>dateTime\</AvailableTo\>

                \<[AvailableUnits](bb968515\(v=office.12\).md)\>float\</AvailableUnits\>

            \</AvailabilityPeriod\>

        \</AvailablilityPeriods\>

        \<[Rates](bb968693\(v=office.12\).md)\>

            \<[Rate](bb968716\(v=office.12\).md)\>

                \<[RatesFrom](bb968409\(v=office.12\).md)\>dateTime\</RatesFrom\>

                \<[RatesTo](bb968548\(v=office.12\).md)\>dateTime\</RatesTo\>

                \<[RateTable](bb968573\(v=office.12\).md)\>integer\</RateTable\>

                \<[StandardRate](bb968453\(v=office.12\).md)\>decimal\</StandardRate\>

                \<[StandardRateFormat](bb968727\(v=office.12\).md)\>integer\</StandardRateFormat\>

                \<[OvertimeRate](bb968679\(v=office.12\).md)\>decimal\</OvertimeRate\>

                \<[OvertimeRateFormat](bb968737\(v=office.12\).md)\>integer\</OvertimeRateFormat\>

                \<[CostPerUse](bb968500\(v=office.12\).md)\>decimal\</CostPerUse\>

            \</Rate\>

        \</Rates\>

        \<[c408000 – c417fff](bb968524\(v=office.12\).md)\>

                \<\!-- \#\#New Project 2007 enterprise resource custom field data.

                                See [Custom Field Data in XML](bb968687\(v=office.12\).md) for more information. --\>

        \</c408000 – c417fff\>

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

    \</Resource\>

\</Resources\>

## See Also

#### Reference

[TimephasedDataType Elements and XML Structure](https://msdn.microsoft.com/en-us/library/317823-7111-4dfd-ae38-50a06c6cb70f\(v=office.12\))

#### Concepts

[Introduction to Project XML Data](bb968652\(v=office.12\).md)

[XML Schema for the Resources Element](bb968511\(v=office.12\).md)

[Custom Field Data in XML](bb968687\(v=office.12\).md)

[Project Elements and XML Structure](bb968439\(v=office.12\).md)

#### Other Resources

[Fields Reference](http://office.microsoft.com/en-us/project/ch100788901033.aspx)

