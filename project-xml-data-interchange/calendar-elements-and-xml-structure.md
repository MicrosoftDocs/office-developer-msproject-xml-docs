---
title: Calendar Elements and XML Structure
TOCTitle: Calendar Elements and XML Structure
ms:assetid: 8147b68c-654d-405e-9878-73548c661689
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968563(v=office.12)
ms:contentKeyID: 13188254
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

# Calendar Elements and XML Structure




This section contains information about children of the Calendars element defined in the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd). The elements represent calendar data when you save a project in the XML format.

Calendars is a child of the Project element. For more information, see [Project Elements and XML Structure](bb968439\(v=office.12\).md).

## XML Structure of Calendar Elements

The following shows the XML structure of the elements defined by the Calendar schema section of mspdi\_pj12.xsd. The data type is indicated for those elements that require a text value. You can find more detailed information about valid text values for each element in the documentation annotations that are embedded in the [XML Schema for the Calendars Element](bb968557\(v=office.12\).md).

For more information about the data types used in the Project 2007 XML Data Interchange Schema, see [Introduction to Project XML Data](bb968652\(v=office.12\).md).

\<[Calendars](bb968499\(v=office.12\).md)\>

    \<[Calendar](bb968481\(v=office.12\).md)\>

        \<[UID](bb968590\(v=office.12\).md)\>integer\</UID\>

        \<[Name](bb968600\(v=office.12\).md)\>string\</Name\>

        \<[IsBaseCalendar](bb968610\(v=office.12\).md)\>boolean\</IsBaseCalendar\>

        \<[BaseCalendarUID](bb968744\(v=office.12\).md)\>integer\</BaseCalendarUID\>

        \<[WeekDays](bb968420\(v=office.12\).md)\>

            \<[WeekDay](bb968433\(v=office.12\).md)\>

                \<[DayType](bb968462\(v=office.12\).md)\>integer\</DayType\>

                \<[DayWorking](bb968665\(v=office.12\).md)\>boolean\</DayWorking\>

                \<[TimePeriod](bb968661\(v=office.12\).md)\>

                    \<[FromDate](bb968583\(v=office.12\).md)\>dateTime\</FromDate\>

                    \<[ToDate](bb968399\(v=office.12\).md)\>dateTime\</ToDate\>

                \</TimePeriod\>

                \<[WorkingTimes](bb968403\(v=office.12\).md)\>

                    \<[WorkingTime](bb968585\(v=office.12\).md)\>

                        \<[FromTime](bb968425\(v=office.12\).md)\>time\</FromTime\>

                        \<[ToTime](bb968466\(v=office.12\).md)\>time\</Time\>

                    \</WorkingTime\>

                \</WorkingTimes\>

            \</WeekDay\>

        \</WeekDays\>

        \<[Exceptions](bb968618\(v=office.12\).md)\>

            \<[Exception](bb968492\(v=office.12\).md)\>

                \<[EnteredByOccurrences](bb968564\(v=office.12\).md)\>boolean\</EnteredByOccurrences\>

                \<[TimePeriod](bb968661\(v=office.12\).md)\>

                    \<[FromDate](bb968583\(v=office.12\).md)\>dateTime\</FromDate\>

                    \<[ToDate](bb968399\(v=office.12\).md)\>dateTime\</ToDate\>

                \</TimePeriod\>

                \<[Occurrences](bb968710\(v=office.12\).md)\>integer\</Occurrences\>

                \<[Name](bb968600\(v=office.12\).md)\>string\</Name\>

                \<[Type](bb968434\(v=office.12\).md)\>integer\</Type\>

                \<[Period](bb968554\(v=office.12\).md)\>integer\</Period\>

                \<[DaysOfWeek](bb968569\(v=office.12\).md)\>integer\</DaysOfWeek\>

                \<[MonthItem](bb968560\(v=office.12\).md)\>integer\</MonthItem\>

                \<[MonthPosition](bb968624\(v=office.12\).md)\>integer\</MonthPosition\>

                \<[Month](bb968450\(v=office.12\).md)\>integer\</Month\>

                \<[MonthDay](bb968700\(v=office.12\).md)\>integer\</MonthDay\>

                \<[DayWorking](bb968665\(v=office.12\).md)\>boolean\</DayWorking\>

                \<[WorkingTimes](bb968403\(v=office.12\).md)\>

                    \<[WorkingTime](bb968585\(v=office.12\).md)\>

                        \<[FromTime](bb968425\(v=office.12\).md)\>time\</FromTime\>

                        \<[ToTime](bb968466\(v=office.12\).md)\>time\</ToTime\>

                    \</WorkingTime\>

                \</WorkingTimes\>

            \</Exception\>

        \</Exceptions\>

        \<[WorkWeeks](bb968496\(v=office.12\).md)\>   \<\!-- See note in the WorkWeeks and WorkWeek topics --\>

            \<[WorkWeek](bb968525\(v=office.12\).md)\>

                \<[TimePeriod](bb968661\(v=office.12\).md)\>

                    \<[FromDate](bb968583\(v=office.12\).md)\>dateTime\</FromDate\>

                    \<[ToDate](bb968399\(v=office.12\).md)\>dateTime\</ToDate\>

                \</TimePeriod\>

                \<[Name](bb968600\(v=office.12\).md)\>string\</Name\>

                \<[WeekDay](bb968433\(v=office.12\).md)\>

                    \<[DayType](bb968462\(v=office.12\).md)\>integer\</DayType\>

                    \<[DayWorking](bb968665\(v=office.12\).md)\>boolean\</DayWorking\>

                \</WeekDay\>

            \</WorkWeek\>

        \</WorkWeeks\>

    \</Calendar\>

\</Calendars\>

## See Also

#### Concepts

[Introduction to Project XML Data](bb968652\(v=office.12\).md)

[XML Schema for the Calendars Element](bb968557\(v=office.12\).md)

[Project Elements and XML Structure](bb968439\(v=office.12\).md)

