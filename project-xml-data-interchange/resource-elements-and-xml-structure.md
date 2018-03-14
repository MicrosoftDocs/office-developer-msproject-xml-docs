---
title: Resource Elements and XML Structure
TOCTitle: Resource Elements and XML Structure
ms:assetid: 26f69c99-50e8-49c5-80cf-1c81c0abefbd
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968445(v=office.12)
ms:contentKeyID: 13188137
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

# Resource Elements and XML Structure




This section contains information about children of the Resources element defined in the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd). The XML elements represent resource data when you save a project in the XML format.

Resources is a child of the Project element. For more information, see [Project Elements and XML Structure](project-elements-and-xml-structure.md).

## XML Structure of Resource Elements

The following shows the XML structure of the elements defined in the Resource schema section of mspdi\_pj12.xsd. The data type is indicated for those elements that require a text value. You can find more detailed information about valid text values for each element in the documentation annotations that are embedded in the [Resource Schema](xml-schema-for-the-resources-element.md).

For more information about the data types used in the Project2007 XML Data Interchange Schema, see [Introduction to Project XML Data](introduction-to-project-xml-data.md).

Many of the Resource elements represent data fields in Microsoft Office Project. For more information about fields in Project Professional 2007 and Project Standard 2007, see [Fields Reference](http://office.microsoft.com/en-us/project/ch100788901033.aspx).


> [!NOTE]
> Detailed information about the structure of the TimephasedData element is shown in <A href="https://msdn.microsoft.com/en-us/library/317823-7111-4dfd-ae38-50a06c6cb70f(v=office.12)">TimephasedDataType Elements and XML Structure</A> in this schema reference.


\<[Resources](resources-element.md)\>

    \<[Resource](resource-element.md)\>

        \<[UID](uid-element.md)\>integer\</UID\>

        \<[ID](id-element.md)\>integer\</ID\>

        \<[Name](name-element.md)\>string\</Name\>

        \<[Type](type-element-multiple-parents.md)\>integer\</Type\>

        \<[IsNull](isnull-element.md)\>boolean\</IsNull\>

        \<[Initials](initials-element.md)\>string\</Initials\>

        \<[Phonetics](phonetics-element.md)\>string\</Phonetics\>

        \<[NTAccount](ntaccount-element.md)\>string\</NTAccount\>

        \<[MaterialLabel](materiallabel-element.md)\>string\</MaterialLabel\>

        \<[Code](code-element.md)\>string\</Code\>

        \<[Group](group-element.md)\>string\</Group\>

        \<[WorkGroup](workgroup-element.md)\>integer\</WorkGroup\>

        \<[EmailAddress](emailaddress-element.md)\>string\</EmailAddress\>

        \<[Hyperlink](hyperlink-element.md)\>string\</Hyperlink\>

        \<[HyperlinkAddress](hyperlinkaddress-element.md)\>string\</HyperlinkAddress\>

        \<[HyperlinkSubAddress](hyperlinksubaddress-element.md)\>string\</HyperlinkSubAddress\>

        \<[MaxUnits](maxunits-element.md)\>float\</MaxUnits\>

        \<[PeakUnits](peakunits-element.md)\>float\</PeakUnits\>

        \<[OverAllocated](overallocated-element.md)\>boolean\</OverAllocated\>

        \<[AvailableFrom](availablefrom-element.md)\>dateTime\</AvailableFrom\>

        \<[AvailableTo](availableto-element.md)\>dateTime\</AvailableTo\>

        \<[Start](start-element.md)\>dateTime\</Start\>

        \<[Finish](finish-element.md)\>dateTime\</Finish\>

        \<[CanLevel](canlevel-element.md)\>boolean\</CanLevel\>

        \<[AccrueAt](accrueat-element.md)\>integer\</AccrueAt\>

        \<[Work](work-element.md)\>duration\</Work\>

        \<[RegularWork](regularwork-element.md)\>duration\</RegularWork\>

        \<[OvertimeWork](overtimework-element.md)\>duration\</OvertimeWork\>

        \<[ActualWork](actualwork-element.md)\>duration\</ActualWork\>

        \<[RemainingWork](remainingwork-element.md)\>duration\</RemainingWork\>

        \<[ActualOvertimeWork](actualovertimework-element.md)\>duration\</ActualOvertimeWork\>

        \<[RemainingOvertimeWork](remainingovertimework-element.md)\>duration\</RemainingOvertimeWork\>

        \<[PercentWorkComplete](percentworkcomplete-element.md)\>integer\</PercentWorkComplete\>

        \<[StandardRate](standardrate-element.md)\>decimal\</StandardRate\>

        \<[StandardRateFormat](standardrateformat-element.md)\>integer\</StandardRateFormat\>

        \<[Cost](cost-element.md)\>decimal\</Cost\>

        \<[OvertimeRate](overtimerate-element.md)\>decimal\</OvertimeRate\>

        \<[OvertimeRateFormat](overtimerateformat-element.md)\>integer\</OvertimeRateFormat\>

        \<[OvertimeCost](overtimecost-element.md)\>decimal\</OvertimeCost\>

        \<[CostPerUse](costperuse-element.md)\>decimal\</CostPerUse\>

        \<[ActualCost](actualcost-element.md)\>decimal\</ActualCost\>

        \<[ActualOvertimeCost](actualovertimecost-element.md)\>decimal\</ActualOvertimeCost\>

        \<[RemainingCost](remainingcost-element.md)\>decimal\</RemainingCost\>

        \<[RemainingOvertimeCost](remainingovertimecost-element.md)\>decimal\</RemainingOvertimeCost\>

        \<[WorkVariance](workvariance-element.md)\>float\</WorkVariance\>

        \<[CostVariance](costvariance-element.md)\>float\</CostVariance\>

        \<[SV](sv-element.md)\>float\</SV\>

        \<[CV](cv-element.md)\>float\</CV\>

        \<[ACWP](acwp-element.md)\>float\</ACWP\>

        \<[CalendarUID](calendaruid-element.md)\>integer\</CalendarUID\>

        \<[Notes](notes-element.md)\>string\</Notes\>

        \<[BCWS](bcws-element.md)\>float\</BCWS\>

        \<[BCWP](bcwp-element.md)\>float\</BCWP\>

        \<[IsGeneric](isgeneric-element.md)\>boolean\</IsGeneric\>

        \<[IsInactive](isinactive-element.md)\>boolean\</IsInactive\>

        \<[IsEnterprise](isenterprise-element.md)\>boolean\</IsEnterprise\>

        \<[BookingType](bookingtype-element.md)\>integer\</BookingType\>

        \<[ActualWorkProtected](actualworkprotected-element.md)\>duration\</ActualWorkProtected\>

        \<[ActualOvertimeWorkProtected](actualovertimeworkprotected-element.md)\>duration\</ActualOvertimeWorkProtected\>

        \<[ActiveDirectoryGUID](activedirectoryguid-element.md)\>string\</ActiveDirectoryGUID\>

        \<[CreationDate](creationdate-element.md)\>dateTime\</CreationDate\>

        \<[ExtendedAttribute](extendedattribute-element.md)\>

            \<[UID](uid-element.md)\>integer\</UID\>

            \<[FieldID](fieldid-element.md)\>string\</FieldID\>

            \<[Value](value-element.md)\>string\</Value\>

            \<[ValueID](valueid-element.md)\>integer\</ValueID\>

            \<[DurationFormat](durationformat-element.md)\>integer\</DurationFormat\>

        \</ExtendedAttribute\>

        \<[Baseline](baseline-element.md)\>

            \<[Number](number-element.md)\>integer\</Number\>

            \<[Work](work-element.md)\>duration\</Work\>

            \<[Cost](cost-element.md)\>float\</Cost\>

            \<[BCWS](bcws-element.md)\>float\</BCWS\>

            \<[BCWP](bcwp-element.md)\>float\</BCWP\>

        \</Baseline\>

        \<[OutlineCode](outlinecode-element.md)\>

            \<[UID](uid-element.md)\>integer\</UID\>

            \<[FieldID](fieldid-element.md)\>string\</FieldID\>

            \<[ValueID](valueid-element.md)\>integer\</ValueID\>

        \</OutlineCode\>

        \<[IsCostResource](iscostresource-element.md)\>boolean\</IsCostResource\>

        \<[AssnOwner](assnowner-element.md)\>string\</AssnOwner\>

        \<[AssnOwnerGuid](assnownerguid-element.md)\>string\</AssnOwnerGuid\>

        \<[IsBudget](isbudget-element.md)\>boolean\</IsBudget\>

        \<[AvailabilityPeriods](availabilityperiods-element.md)\>

            \<[AvailabilityPeriod](availabilityperiod-element.md)\>

                \<[AvailableFrom](availablefrom-element.md)\>dateTime\</AvailableFrom\>

                \<[AvailableTo](availableto-element.md)\>dateTime\</AvailableTo\>

                \<[AvailableUnits](availableunits-element.md)\>float\</AvailableUnits\>

            \</AvailabilityPeriod\>

        \</AvailablilityPeriods\>

        \<[Rates](rates-element.md)\>

            \<[Rate](rate-element.md)\>

                \<[RatesFrom](ratesfrom-element.md)\>dateTime\</RatesFrom\>

                \<[RatesTo](ratesto-element.md)\>dateTime\</RatesTo\>

                \<[RateTable](ratetable-element.md)\>integer\</RateTable\>

                \<[StandardRate](standardrate-element.md)\>decimal\</StandardRate\>

                \<[StandardRateFormat](standardrateformat-element.md)\>integer\</StandardRateFormat\>

                \<[OvertimeRate](overtimerate-element.md)\>decimal\</OvertimeRate\>

                \<[OvertimeRateFormat](overtimerateformat-element.md)\>integer\</OvertimeRateFormat\>

                \<[CostPerUse](costperuse-element.md)\>decimal\</CostPerUse\>

            \</Rate\>

        \</Rates\>

        \<[c408000 – c417fff](c408000-c417fff-elements.md)\>

                \<\!-- \#\#New Project 2007 enterprise resource custom field data.

                                See [Custom Field Data in XML](custom-field-data-in-xml.md) for more information. --\>

        \</c408000 – c417fff\>

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

    \</Resource\>

\</Resources\>

## See Also

#### Reference

[TimephasedDataType Elements and XML Structure](https://msdn.microsoft.com/en-us/library/317823-7111-4dfd-ae38-50a06c6cb70f\(v=office.12\))

#### Concepts

[Introduction to Project XML Data](introduction-to-project-xml-data.md)

[XML Schema for the Resources Element](xml-schema-for-the-resources-element.md)

[Custom Field Data in XML](custom-field-data-in-xml.md)

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

#### Other Resources

[Fields Reference](http://office.microsoft.com/en-us/project/ch100788901033.aspx)

