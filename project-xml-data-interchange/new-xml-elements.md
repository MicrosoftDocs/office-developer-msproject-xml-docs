---
title: New XML Elements
TOCTitle: New XML Elements
ms:assetid: 8c9c7788-53b1-460f-88b5-c8f4f4fdedf7
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968581(v=office.12)
ms:contentKeyID: 13188272
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- XML schema [Project 2007]
- Project XML schema
- Project 2007, XML
- Project XML schema changes
monikerRange: '>= project-client-2007 || project-client-odc'
---

# New XML Elements




The Microsoft Office Project 2007 XML Data Interchange Schema (mspdi\_pj12.xsd) includes new XML elements that support new and enhanced functionality in Office Project 2007.

## New XML Elements in Project 2007

The following sections briefly describe the new elements in the Project XML Data Interchange Schema in Project 2007. In addition, Project 2007 includes changes to the way that some custom field information is represented in XML. For more information, see [Custom Field Data in XML](custom-field-data-in-xml.md).

This article organizes the new elements alphabetically within the following sections, which parallel the organization of this schema reference. For detailed information about XML element structure, see [Project Data Interchange Elements](project-data-interchange-elements.md).

  - Table 1: New Project elements

  - Table 2: New OutlineCode elements

  - Table 3: New ExtendedAttribute elements

  - Table 4: New Calendar elements

  - Table 5: New Task elements

  - Table 6: New Resource elements

  - Table 7: New Assignment elements


### Table 1. New Project elements

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p><strong>Element Name</strong></p></th>
<th><p><strong>Description</strong></p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>CurrencyCode</p></td>
<td><p>Provides forward-compatibility for IOS 4217 currency code data.</p></td>
</tr>
<tr class="even">
<td><p>SaveVersion</p></td>
<td><p>The version of Project the XML file was saved from.</p></td>
</tr>
</tbody>
</table>

<br/>

### Table 2. New OutlineCode elements

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p><strong>Element Name</strong></p></th>
<th><p><strong>Description</strong></p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>FieldGUID</p></td>
<td><p>The globally unique identifier (GUID) of the outline code value.</p></td>
</tr>
<tr class="even">
<td><p>Guid</p></td>
<td><p>The GUID of the outline code.</p></td>
</tr>
<tr class="odd">
<td><p>Type</p></td>
<td><p>The outline code type.</p></td>
</tr>
</tbody>
</table>

<br/>

### Table 3. New ExtendedAttribute elements

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p><strong>Element Name</strong></p></th>
<th><p><strong>Description</strong></p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>AutoRollDown</p></td>
<td><p>Whether automatic rolldown to assignments is enabled.</p></td>
</tr>
<tr class="even">
<td><p>CFType</p></td>
<td><p>The custom field type.</p></td>
</tr>
<tr class="odd">
<td><p>ElemType</p></td>
<td><p>The custom field association.</p></td>
</tr>
<tr class="even">
<td><p>DefaultGuid</p></td>
<td><p>The GUID of the default custom field value.</p></td>
</tr>
<tr class="odd">
<td><p>Guid</p></td>
<td><p>The GUID of the custom field.</p></td>
</tr>
<tr class="even">
<td><p>Ltuid</p></td>
<td><p>The GUID of the lookup table associated with the custom field.</p></td>
</tr>
<tr class="odd">
<td><p>MaxMultiValues</p></td>
<td><p>The maximum number of items that can be selected from a picklist.</p></td>
</tr>
<tr class="even">
<td><p>Phonetic</p></td>
<td><p>Phonetic information for custom field names.</p></td>
</tr>
<tr class="odd">
<td><p>SecondaryPID</p></td>
<td><p>The secondary PID of the custom field.</p></td>
</tr>
<tr class="even">
<td><p>UserDef</p></td>
<td><p>Whether the custom field is user-defined.</p></td>
</tr>
</tbody>
</table>

<br/>

### Table 4. New Calendar elements

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p><strong>Element name</strong></p></th>
<th><p><strong>Description</strong></p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>DaysOfWeek</p></td>
<td><p>The days of the week the exception is valid for.</p></td>
</tr>
<tr class="even">
<td><p>EnteredByOccurrences</p></td>
<td><p>Whether the number of exception recurrences is defined by a number or by a finish date.</p></td>
</tr>
<tr class="odd">
<td><p>Exception</p></td>
<td><p>Contains the elements that define a calendar exception.</p></td>
</tr>
<tr class="even">
<td><p>Exceptions</p></td>
<td><p>Contains the collection of calendar exceptions.</p></td>
</tr>
<tr class="odd">
<td><p>Month</p></td>
<td><p>The month the exception recurrence is scheduled for.</p></td>
</tr>
<tr class="even">
<td><p>MonthDay</p></td>
<td><p>The day of the month the exception recurrence is scheduled for.</p></td>
</tr>
<tr class="odd">
<td><p>MonthItem</p></td>
<td><p>The month item the exception recurrence is scheduled for.</p></td>
</tr>
<tr class="even">
<td><p>MonthPosition</p></td>
<td><p>The position of a month item within a month.</p></td>
</tr>
<tr class="odd">
<td><p>Name (parent Exception)</p></td>
<td><p>The name of the exception.</p></td>
</tr>
<tr class="even">
<td><p>Name (parent WorkWeek)</p></td>
<td><p>The name of the effective work week.</p></td>
</tr>
<tr class="odd">
<td><p>Occurrences</p></td>
<td><p>The number of times the exception occurs.</p></td>
</tr>
<tr class="even">
<td><p>Period</p></td>
<td><p>The period of recurrence for the exception.</p></td>
</tr>
<tr class="odd">
<td><p>Type</p></td>
<td><p>The exception type.</p></td>
</tr>
<tr class="even">
<td><p>WorkWeek</p></td>
<td><p>Contains the elements that define an effective work week.</p></td>
</tr>
<tr class="odd">
<td><p>WorkWeeks</p></td>
<td><p>Contains the collection of effective work weeks associated with the calendar.</p></td>
</tr>
</tbody>
</table>

<br/>

### Table 5. New Task elements

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p><strong>Element name</strong></p></th>
<th><p><strong>Description</strong></p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>CommitmentFinish</p></td>
<td><p>The finish date of the deliverable.</p></td>
</tr>
<tr class="even">
<td><p>CommitmentStart</p></td>
<td><p>The start date of the deliverable.</p></td>
</tr>
<tr class="odd">
<td><p>CommitmentType</p></td>
<td><p>Whether the task has an associated deliverable or a dependency on an associated deliverable.</p></td>
</tr>
<tr class="even">
<td><p>FixedCost</p></td>
<td><p>The fixed cost of the task when the baseline was saved.</p></td>
</tr>
<tr class="odd">
<td><p>IsPublished</p></td>
<td><p>Whether the task is published.</p></td>
</tr>
<tr class="even">
<td><p>StatusManager</p></td>
<td><p>The name of the status manager for the task.</p></td>
</tr>
</tbody>
</table>

<br/>

### Table 6. New Resource elements

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p><strong>Element name</strong></p></th>
<th><p><strong>Description</strong></p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>AssnOwner</p></td>
<td><p>The name of the assignment owner.</p></td>
</tr>
<tr class="even">
<td><p>AssnOwnerGuid</p></td>
<td><p>The GUID of the assignment owner.</p></td>
</tr>
<tr class="odd">
<td><p>IsBudget</p></td>
<td><p>Whether the resource is a budget resource.</p></td>
</tr>
<tr class="even">
<td><p>IsCostResource</p></td>
<td><p>Whether the resource is a cost resource.</p></td>
</tr>
</tbody>
</table>

<br/>

### Table 7. New Assignment elements

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p><strong>Element name</strong></p></th>
<th><p><strong>Description</strong></p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>AssnOwner</p></td>
<td><p>The name of the assignment owner.</p></td>
</tr>
<tr class="even">
<td><p>AssnOwnerGuid</p></td>
<td><p>The GUID of the assignment owner.</p></td>
</tr>
<tr class="odd">
<td><p>BudgetCost</p></td>
<td><p>The budgeted amount for cost resources on this assignment.</p></td>
</tr>
<tr class="even">
<td><p>BudgetWork</p></td>
<td><p>The budgeted amount for work or material resources on this assignment.</p></td>
</tr>
<tr class="odd">
<td><p>PeakUnits</p></td>
<td><p>The maximum number of units a resource is assigned for a task.</p></td>
</tr>
<tr class="even">
<td><p>Summary</p></td>
<td><p>Whether the task is a summary task.</p></td>
</tr>
<tr class="odd">
<td><p>SV</p></td>
<td><p>The earned value schedule variance, through the project status date.</p></td>
</tr>
</tbody>
</table>

## See also

- [Custom Field Data in XML](custom-field-data-in-xml.md)

- [Introduction to Project XML Data](introduction-to-project-xml-data.md)

- [Project Data Interchange Elements](project-data-interchange-elements.md)

