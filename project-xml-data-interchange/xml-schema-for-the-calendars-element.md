---
title: XML Schema for the Calendars Element
TOCTitle: XML Schema for the Calendars Element
ms:assetid: 7afbe811-c94e-4ff6-8968-5b9aede4393a
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968557(v=office.12)
ms:contentKeyID: 13188248
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- Schemas [Project 2007]
- XML and Project
- XML schema [Project 2007]
- Project schema
- Project XML schema
- XML in Project
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# XML Schema for the Calendars Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

The following shows the section of the Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd) that defines the Calendars element.

The complete Project 2007 XML Data Interchange Schema is included in the Project 2007 SDK download. For a link to the Project 2007 SDK download, see [Welcome to the Microsoft Office Project 2007 SDK](https://msdn.microsoft.com/en-us/library/ms512767).

## Calendars Schema

``` xml
<?xml version="1.0" encoding="utf-8"?>
. . .
<!-- @Calendar schema -->
<xsd:element name="Calendars" minOccurs="0">
  <xsd:annotation>
    <xsd:documentation>The collection of calendars that is associated with the project.</xsd:documentation>
  </xsd:annotation>
  <xsd:complexType>
    <xsd:sequence>
      <xsd:element name="Calendar" minOccurs="1" maxOccurs="unbounded">
        <xsd:annotation>
          <xsd:documentation>Calendars are used to define standard working and non-working times. Projects must have one base calendar. Tasks and resources can have their own non-base calendars that are based on a base calendar.</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="UID" type="xsd:integer">
              <xsd:annotation>
                <xsd:documentation>The unique identifier of the calendar.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="Name" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The name of the calendar.</xsd:documentation>
              </xsd:annotation>
              <xsd:simpleType>
                <xsd:restriction base="xsd:string">
                  <xsd:maxLength value="512" />
                </xsd:restriction>
              </xsd:simpleType>
            </xsd:element>
            <xsd:element name="IsBaseCalendar" type="xsd:boolean" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>Whether the calendar is a base calendar.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="BaseCalendarUID" type="xsd:integer" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The unique identifier of the base calendar on which this calendar depends. Only applicable if the calendar is not a base calendar.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="WeekDays" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The collection of weekdays that defines this calendar.</xsd:documentation>
              </xsd:annotation>
              <xsd:complexType>
                <xsd:sequence>
                  <xsd:element name="WeekDay" minOccurs="0" maxOccurs="unbounded">
                    <xsd:annotation>
                      <xsd:documentation>A weekday either defines regular days of the week or exception days in the calendar.</xsd:documentation>
                    </xsd:annotation>
                    <xsd:complexType>
                      <xsd:sequence>
                        <xsd:element name="DayType" minOccurs="1">
                          <xsd:annotation>
                            <xsd:documentation>The type of day. Values are: 0=Exception, 1=Sunday, 2=Monday, 3=Tuesday, 4=Wednesday, 5=Thursday, 6=Friday, 7=Saturday.</xsd:documentation>
                          </xsd:annotation>
                          <xsd:simpleType>
                            <xsd:restriction base="xsd:integer">
                              <xsd:enumeration value="0" />
                              <xsd:enumeration value="1" />
                              <xsd:enumeration value="2" />
                              <xsd:enumeration value="3" />
                              <xsd:enumeration value="4" />
                              <xsd:enumeration value="5" />
                              <xsd:enumeration value="6" />
                              <xsd:enumeration value="7" />
                            </xsd:restriction>
                          </xsd:simpleType>
                        </xsd:element>
                        <xsd:element name="DayWorking" type="xsd:boolean" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>Whether the specified date or day type is working.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <xsd:element name="TimePeriod" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>Defines a contiguous set of exception days.</xsd:documentation>
                          </xsd:annotation>
                          <xsd:complexType>
                            <xsd:sequence>
                              <xsd:element name="FromDate" type="xsd:dateTime" minOccurs="0">
                                <xsd:annotation>
                                  <xsd:documentation>The beginning of the exception time.</xsd:documentation>
                                </xsd:annotation>
                              </xsd:element>
                              <xsd:element name="ToDate" type="xsd:dateTime" minOccurs="0">
                                <xsd:annotation>
                                  <xsd:documentation>The end of the exception time.</xsd:documentation>
                                </xsd:annotation>
                              </xsd:element>
                            </xsd:sequence>
                          </xsd:complexType>
                        </xsd:element>
                        <xsd:element name="WorkingTimes" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The collection of working times that define the time worked on the weekday. One of these must be present, and there can be no more than five.</xsd:documentation>
                          </xsd:annotation>
                          <xsd:complexType>
                            <xsd:sequence>
                              <xsd:choice>
                                <xsd:element name="WorkingTime" minOccurs="0" maxOccurs="5">
                                  <xsd:annotation>
                                    <xsd:documentation>Defines the working time during the weekday.</xsd:documentation>
                                  </xsd:annotation>
                                  <xsd:complexType>
                                    <xsd:sequence>
                                      <xsd:element name="FromTime" type="xsd:time" minOccurs="0">
                                        <xsd:annotation>
                                          <xsd:documentation>The beginning of the working time.</xsd:documentation>
                                        </xsd:annotation>
                                      </xsd:element>
                                      <xsd:element name="ToTime" type="xsd:time" minOccurs="0">
                                        <xsd:annotation>
                                          <xsd:documentation>The end of the working time.</xsd:documentation>
                                        </xsd:annotation>
                                      </xsd:element>
                                    </xsd:sequence>
                                  </xsd:complexType>
                                </xsd:element>
                              </xsd:choice>
                            </xsd:sequence>
                          </xsd:complexType>
                        </xsd:element>
                      </xsd:sequence>
                    </xsd:complexType>
                  </xsd:element>
                </xsd:sequence>
              </xsd:complexType>
            </xsd:element>
            <!-- #New Project 2007 element definitions -->
            <xsd:element name="Exceptions" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The collection of exceptions that is associated with the calendar.</xsd:documentation>
              </xsd:annotation>
              <xsd:complexType>
                <xsd:sequence>
                  <xsd:element name="Exception" minOccurs="0" maxOccurs="unbounded">
                    <xsd:annotation>
                      <xsd:documentation>Exceptions are used to define an exception sub-calendar.</xsd:documentation>
                    </xsd:annotation>
                    <xsd:complexType>
                      <xsd:sequence>
                        <xsd:element name="EnteredByOccurrences" type="xsd:boolean" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>Whether the range of recurrence is defined by entering a number of occurrences. False specifies that the range of recurrence is defined by entering a finish date.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <xsd:element name="TimePeriod" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>Defines a contiguous set of exception days.</xsd:documentation>
                          </xsd:annotation>
                          <xsd:complexType>
                            <xsd:sequence>
                              <xsd:element name="FromDate" type="xsd:dateTime" minOccurs="0">
                                <xsd:annotation>
                                  <xsd:documentation>The beginning of the exception time.</xsd:documentation>
                                </xsd:annotation>
                              </xsd:element>
                              <xsd:element name="ToDate" type="xsd:dateTime" minOccurs="0">
                                <xsd:annotation>
                                  <xsd:documentation>The end of the exception time.</xsd:documentation>
                                </xsd:annotation>
                              </xsd:element>
                            </xsd:sequence>
                          </xsd:complexType>
                        </xsd:element>
                        <xsd:element name="Occurrences" type="xsd:integer" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The number of occurrences for which the calendar exception is valid.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <xsd:element name="Name" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The name of the exception.</xsd:documentation>
                          </xsd:annotation>
                          <xsd:simpleType>
                            <xsd:restriction base="xsd:string">
                              <xsd:maxLength value="512" />
                            </xsd:restriction>
                          </xsd:simpleType>
                        </xsd:element>
                        <xsd:element name="Type" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The exception type. Values are: 1=Daily, 2=Yearly by day of the month, 3=Yearly by position, 4=Monthly by day of the month, 5=Monthly by position, 6=Weekly, 7=By day count, 8=By weekday count, 9=No exception type.</xsd:documentation>
                          </xsd:annotation>
                          <xsd:simpleType>
                            <xsd:restriction base="xsd:integer">
                              <xsd:enumeration value="1" />
                              <xsd:enumeration value="2" />
                              <xsd:enumeration value="3" />
                              <xsd:enumeration value="4" />
                              <xsd:enumeration value="5" />
                              <xsd:enumeration value="6" />
                              <xsd:enumeration value="7" />
                              <xsd:enumeration value="8" />
                              <xsd:enumeration value="9" />
                            </xsd:restriction>
                          </xsd:simpleType>
                        </xsd:element>
                        <xsd:element name="Period" type="xsd:integer" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The period of recurrence for the exception.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <xsd:element name="DaysOfWeek" type="xsd:integer" minOccurs="0" maxOccurs="1">
                          <xsd:annotation>
                            <xsd:documentation>The days of the week on which the exception is valid. Values are: 1=Sunday, 2=Monday, 4=Tuesday, 8=Wednesday, 16=Thursday, 32=Friday, 64=Saturday.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <xsd:element name="MonthItem" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The month item for which an exception recurrence is scheduled. Values are: 0=Day, 1=Weekday, 2=WeekendDay, 3=Sunday, 4=Monday, 5=Tuesday, 6=Wednesday, 7=Thursday, 8=Friday, 9=Saturday.</xsd:documentation>
                          </xsd:annotation>
                          <xsd:simpleType>
                            <xsd:restriction base="xsd:integer">
                              <xsd:enumeration value="0" />
                              <xsd:enumeration value="1" />
                              <xsd:enumeration value="2" />
                              <xsd:enumeration value="3" />
                              <xsd:enumeration value="4" />
                              <xsd:enumeration value="5" />
                              <xsd:enumeration value="6" />
                              <xsd:enumeration value="7" />
                              <xsd:enumeration value="8" />
                              <xsd:enumeration value="9" />
                            </xsd:restriction>
                          </xsd:simpleType>
                        </xsd:element>
                        <xsd:element name="MonthPosition" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The position of a month item within a month. Values are: 0=First position, 1=Second position, 2=Third position, 3=Fourth position, 4=Last position.</xsd:documentation>
                          </xsd:annotation>
                          <xsd:simpleType>
                            <xsd:restriction base="xsd:integer">
                              <xsd:enumeration value="0" />
                              <xsd:enumeration value="1" />
                              <xsd:enumeration value="2" />
                              <xsd:enumeration value="3" />
                              <xsd:enumeration value="4" />
                            </xsd:restriction>
                          </xsd:simpleType>
                        </xsd:element>
                        <xsd:element name="Month" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The month for which an exception recurrence is scheduled. Values are: 0=January, 1=February, 2=March, 3=April, 4=May, 5=June, 6=July, 7=August, 8=September, 9=October, 10=November, 11=December.</xsd:documentation>
                          </xsd:annotation>
                          <xsd:simpleType>
                            <xsd:restriction base="xsd:integer">
                              <xsd:enumeration value="0" />
                              <xsd:enumeration value="1" />
                              <xsd:enumeration value="2" />
                              <xsd:enumeration value="3" />
                              <xsd:enumeration value="4" />
                              <xsd:enumeration value="5" />
                              <xsd:enumeration value="6" />
                              <xsd:enumeration value="7" />
                              <xsd:enumeration value="8" />
                              <xsd:enumeration value="9" />
                              <xsd:enumeration value="10" />
                              <xsd:enumeration value="11" />
                            </xsd:restriction>
                          </xsd:simpleType>
                        </xsd:element>
                        <xsd:element name="MonthDay" type="xsd:integer" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The day of the month on which an exception recurrence is scheduled.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <xsd:element name="DayWorking" type="xsd:boolean" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>Whether the specified date or day type is working.</xsd:documentation>
                          </xsd:annotation>
                        </xsd:element>
                        <xsd:element name="WorkingTimes" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The collection of working times that define the time worked on the weekday.  One of these must be present, and there can be no more than five.</xsd:documentation>
                          </xsd:annotation>
                          <xsd:complexType>
                            <xsd:sequence>
                              <xsd:choice>
                                <xsd:element name="WorkingTime" minOccurs="0" maxOccurs="5">
                                  <xsd:annotation>
                                    <xsd:documentation>Defines the working time during the weekday.</xsd:documentation>
                                  </xsd:annotation>
                                  <xsd:complexType>
                                    <xsd:sequence>
                                      <xsd:element name="FromTime" type="xsd:time" minOccurs="0">
                                        <xsd:annotation>
                                          <xsd:documentation>The beginning of the working time.</xsd:documentation>
                                        </xsd:annotation>
                                      </xsd:element>
                                      <xsd:element name="ToTime" type="xsd:time" minOccurs="0">
                                        <xsd:annotation>
                                          <xsd:documentation>The end of the working time.</xsd:documentation>
                                        </xsd:annotation>
                                      </xsd:element>
                                    </xsd:sequence>
                                  </xsd:complexType>
                                </xsd:element>
                              </xsd:choice>
                            </xsd:sequence>
                          </xsd:complexType>
                        </xsd:element>
                      </xsd:sequence>
                    </xsd:complexType>
                  </xsd:element>
                </xsd:sequence>
              </xsd:complexType>
            </xsd:element>
            <!-- Note: The WorkWeeks element is not correctly saved to XML. 
                 To create valid XML, you must replace the empty tag set (<> and </>) 
                 with the WorkWeeks tag set (<WorkWeeks> and </WorkWeeks>). 
            -->
            <xsd:element name="WorkWeeks" minOccurs="0">
              <xsd:annotation>
                <xsd:documentation>The collection of effective work weeks associated with the calendar.</xsd:documentation>
              </xsd:annotation>
              <xsd:complexType>
                <xsd:sequence>
                  <xsd:element name="WorkWeek" minOccurs="0" maxOccurs="unbounded">
                    <xsd:annotation>
                      <xsd:documentation>Defines an effective work week.</xsd:documentation>
                    </xsd:annotation>
                    <xsd:complexType>
                      <xsd:sequence>
                        <xsd:element name="TimePeriod" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>Defines a contiguous set of exception days.</xsd:documentation>
                          </xsd:annotation>
                          <xsd:complexType>
                            <xsd:sequence>
                              <xsd:element name="FromDate" type="xsd:dateTime" minOccurs="0">
                                <xsd:annotation>
                                  <xsd:documentation>The beginning of the exception time.</xsd:documentation>
                                </xsd:annotation>
                              </xsd:element>
                              <xsd:element name="ToDate" type="xsd:dateTime" minOccurs="0">
                                <xsd:annotation>
                                  <xsd:documentation>The end of the exception time.</xsd:documentation>
                                </xsd:annotation>
                              </xsd:element>
                            </xsd:sequence>
                          </xsd:complexType>
                        </xsd:element>
                        <xsd:element name="Name" minOccurs="0">
                          <xsd:annotation>
                            <xsd:documentation>The name of the effective week.</xsd:documentation>
                          </xsd:annotation>
                          <xsd:simpleType>
                            <xsd:restriction base="xsd:string">
                              <xsd:maxLength value="512" />
                            </xsd:restriction>
                          </xsd:simpleType>
                        </xsd:element>
                        <!-- Note: The WeekDay element is not correctly saved to XML. 
                             To create valid XML, you must manually insert a closing tag (</WeekDay>) 
                             for each opening tag (<WeekDay>) in the XML output.
                        -->
                        <xsd:element name="WeekDay" minOccurs="0" maxOccurs="unbounded">
                          <xsd:annotation>
                            <xsd:documentation>A weekday either defines regular days of the week or exception days in the calendar.</xsd:documentation>
                          </xsd:annotation>
                          <xsd:complexType>
                            <xsd:sequence>
                              <xsd:element name="DayType" minOccurs="1">
                                <xsd:annotation>
                                  <xsd:documentation>The type of day. Values are: 0=Exception, 1=Sunday, 2=Monday, 3=Tuesday, 4=Wednesday, 5=Thursday, 6=Friday, 7=Saturday.</xsd:documentation>
                                </xsd:annotation>
                                <xsd:simpleType>
                                  <xsd:restriction base="xsd:integer">
                                    <xsd:enumeration value="0" />
                                    <xsd:enumeration value="1" />
                                    <xsd:enumeration value="2" />
                                    <xsd:enumeration value="3" />
                                    <xsd:enumeration value="4" />
                                    <xsd:enumeration value="5" />
                                    <xsd:enumeration value="6" />
                                    <xsd:enumeration value="7" />
                                  </xsd:restriction>
                                </xsd:simpleType>
                              </xsd:element>
                              <xsd:element name="DayWorking" type="xsd:boolean" minOccurs="0">
                                <xsd:annotation>
                                  <xsd:documentation>Whether the specified date or day type is working.</xsd:documentation>
                                </xsd:annotation>
                              </xsd:element>
                            </xsd:sequence>
                          </xsd:complexType>
                        </xsd:element>
                      </xsd:sequence>
                    </xsd:complexType>
                  </xsd:element>
                </xsd:sequence>
              </xsd:complexType>
            </xsd:element>
            <!-- #End new Project 2007 element definitions -->
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
</xsd:element>
```

## See Also

#### Concepts

[Calendar Elements and XML Structure](bb968563\(v=office.12\).md)

