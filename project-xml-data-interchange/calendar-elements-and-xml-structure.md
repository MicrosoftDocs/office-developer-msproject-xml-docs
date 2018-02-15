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

Calendars is a child of the Project element. For more information, see [Project Elements and XML Structure](project-elements-and-xml-structure.md).

## XML Structure of Calendar Elements

The following shows the XML structure of the elements defined by the Calendar schema section of mspdi\_pj12.xsd. The data type is indicated for those elements that require a text value. You can find more detailed information about valid text values for each element in the documentation annotations that are embedded in the [XML Schema for the Calendars Element](xml-schema-for-the-calendars-element.md).

For more information about the data types used in the Project 2007 XML Data Interchange Schema, see [Introduction to Project XML Data](introduction-to-project-xml-data.md).

\<[Calendars](calendars-element.md)\>

    \<[Calendar](calendar-element.md)\>

        \<[UID](uid-element.md)\>integer\</UID\>

        \<[Name](name-element.md)\>string\</Name\>

        \<[IsBaseCalendar](isbasecalendar-element.md)\>boolean\</IsBaseCalendar\>

        \<[BaseCalendarUID](basecalendaruid-element.md)\>integer\</BaseCalendarUID\>

        \<[WeekDays](weekdays-element.md)\>

            \<[WeekDay](weekday-element.md)\>

                \<[DayType](daytype-element.md)\>integer\</DayType\>

                \<[DayWorking](dayworking-element-calendar.md)\>boolean\</DayWorking\>

                \<[TimePeriod](timeperiod-element-calendar.md)\>

                    \<[FromDate](fromdate-element-calendar.md)\>dateTime\</FromDate\>

                    \<[ToDate](todate-element-calendar.md)\>dateTime\</ToDate\>

                \</TimePeriod\>

                \<[WorkingTimes](workingtimes-element-calendar.md)\>

                    \<[WorkingTime](workingtime-element-calendar.md)\>

                        \<[FromTime](fromtime-element-calendar.md)\>time\</FromTime\>

                        \<[ToTime](totime-element-calendar.md)\>time\</Time\>

                    \</WorkingTime\>

                \</WorkingTimes\>

            \</WeekDay\>

        \</WeekDays\>

        \<[Exceptions](exceptions-element.md)\>

            \<[Exception](exception-element.md)\>

                \<[EnteredByOccurrences](enteredbyoccurrences-element.md)\>boolean\</EnteredByOccurrences\>

                \<[TimePeriod](timeperiod-element-calendar.md)\>

                    \<[FromDate](fromdate-element-calendar.md)\>dateTime\</FromDate\>

                    \<[ToDate](todate-element-calendar.md)\>dateTime\</ToDate\>

                \</TimePeriod\>

                \<[Occurrences](occurrences-element.md)\>integer\</Occurrences\>

                \<[Name](name-element.md)\>string\</Name\>

                \<[Type](type-element-multiple-parents.md)\>integer\</Type\>

                \<[Period](period-element.md)\>integer\</Period\>

                \<[DaysOfWeek](daysofweek-element.md)\>integer\</DaysOfWeek\>

                \<[MonthItem](monthitem-element.md)\>integer\</MonthItem\>

                \<[MonthPosition](monthposition-element.md)\>integer\</MonthPosition\>

                \<[Month](month-element.md)\>integer\</Month\>

                \<[MonthDay](monthday-element.md)\>integer\</MonthDay\>

                \<[DayWorking](dayworking-element-calendar.md)\>boolean\</DayWorking\>

                \<[WorkingTimes](workingtimes-element-calendar.md)\>

                    \<[WorkingTime](workingtime-element-calendar.md)\>

                        \<[FromTime](fromtime-element-calendar.md)\>time\</FromTime\>

                        \<[ToTime](totime-element-calendar.md)\>time\</ToTime\>

                    \</WorkingTime\>

                \</WorkingTimes\>

            \</Exception\>

        \</Exceptions\>

        \<[WorkWeeks](workweeks-element.md)\>   \<\!-- See note in the WorkWeeks and WorkWeek topics --\>

            \<[WorkWeek](workweek-element.md)\>

                \<[TimePeriod](timeperiod-element-calendar.md)\>

                    \<[FromDate](fromdate-element-calendar.md)\>dateTime\</FromDate\>

                    \<[ToDate](todate-element-calendar.md)\>dateTime\</ToDate\>

                \</TimePeriod\>

                \<[Name](name-element.md)\>string\</Name\>

                \<[WeekDay](weekday-element.md)\>

                    \<[DayType](daytype-element.md)\>integer\</DayType\>

                    \<[DayWorking](dayworking-element-calendar.md)\>boolean\</DayWorking\>

                \</WeekDay\>

            \</WorkWeek\>

        \</WorkWeeks\>

    \</Calendar\>

\</Calendars\>

## See Also

#### Concepts

[Introduction to Project XML Data](introduction-to-project-xml-data.md)

[XML Schema for the Calendars Element](xml-schema-for-the-calendars-element.md)

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

