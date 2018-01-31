---
title: Resource Element
TOCTitle: Resource Element
ms:assetid: e67f9a03-2869-431d-8d48-353e3e15a896
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968715(v=office.12)
ms:contentKeyID: 13188405
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- Resource element
---

# Resource Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

A resource in the project. There must be at least one resource in each Resources collection.

    <Resource>
      ComplexTypeValue
    </Resource>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968730(v=office.12).md">Resources</a></p></td>
</tr>
</tbody>
</table>

## Child Elements

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Element</p></th>
<th><p>Required / Optional</p></th>
<th><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="bb968590(v=office.12).md">UID Element</a></p></td>
<td><p>Required</p></td>
<td><p>The unique ID for the resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968437(v=office.12).md">ID Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The position identifier of the resource within the list of resources.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968600(v=office.12).md">Name Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The name of the resource; must be unique within the enterprise, whether or not the resource is active.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968434(v=office.12).md">Type Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The resource type (work or material).</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968682(v=office.12).md">IsNull Element</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the resource is a null resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968658(v=office.12).md">Initials Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The initials of a resource name.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968636(v=office.12).md">Phonetics Element</a></p></td>
<td><p>Optional</p></td>
<td><p>Contains phonetic information in either Hiragana or Katakana for resource names; used only in the Japanese version of Microsoft Office Project.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968430(v=office.12).md">NTAccount Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The Microsoft Windows NT Account name for a resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968598(v=office.12).md">MaterialLabel Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The unit of measurement entered for a material resource, for example, tons, boxes, or cubic yards.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968539(v=office.12).md">Code Element</a></p></td>
<td><p>Optional</p></td>
<td><p>A code, abbreviation, or number entered as part of a resource's information.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968570(v=office.12).md">Group Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The name of the group the resource belongs to.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968721(v=office.12).md">WorkGroup Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The messaging method used to communicate with a project team.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968510(v=office.12).md">EmailAddress Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The e-mail address of a resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968729(v=office.12).md">Hyperlink Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The title or explanatory text for a hyperlink associated with a resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968561(v=office.12).md">HyperlinkAddress Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The address for a hyperlink associated with a resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968602(v=office.12).md">HyperlinkSubAddress Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The specific location in a document within a hyperlink associated with a resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968589(v=office.12).md">MaxUnits Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The maximum percentage, or number of units, that represents the maximum amount that a resource is available to accomplish any tasks during the current time period.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968404(v=office.12).md">PeakUnits Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The maximum percentage, or number of units, that a resource is assigned at any one time for all tasks assigned to that resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968615(v=office.12).md">OverAllocated Element</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether a resource is assigned to do more work on all assigned tasks than can be done within the resource's normal work capacity.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968686(v=office.12).md">AvailableFrom Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The starting date that a resource is available for work at the units specified for the current time period.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968648(v=office.12).md">AvailableTo Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The ending date that a resource will be available for work at the units specified for the current time period.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968645(v=office.12).md">Start Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The date and time that a resource is scheduled to start work on all assigned tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968534(v=office.12).md">Finish Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The date and time that a resource is scheduled to complete work on all assigned tasks.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968435(v=office.12).md">CanLevel Element</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether resource leveling can be performed with a resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968660(v=office.12).md">AccrueAt Element</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates how and when resource standard and overtime costs are to be charged, or accrued, to the cost of a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968571(v=office.12).md">Work Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The total amount of work scheduled to be performed by a resource on all assigned tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968582(v=office.12).md">RegularWork Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The total amount of non-overtime work scheduled to be performed for all assignments assigned to a resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968609(v=office.12).md">OvertimeWork</a></p></td>
<td><p>Optional</p></td>
<td><p>The amount of overtime to be performed for all tasks assigned to a resource and charged at the resource's overtime rate.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968429(v=office.12).md">ActualWork</a></p></td>
<td><p>Optional</p></td>
<td><p>The actual amount of work that has already been done for all assignments assigned to a resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968720(v=office.12).md">RemainingWork</a></p></td>
<td><p>Optional</p></td>
<td><p>The amount of time, or person-hours, still required by a resource to complete all assigned tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968413(v=office.12).md">ActualOvertimeWork</a></p></td>
<td><p>Optional</p></td>
<td><p>The actual amount of overtime work already performed for all assignments assigned to a resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968473(v=office.12).md">RemainingOvertimeWork</a></p></td>
<td><p>Optional</p></td>
<td><p>The remaining amount of overtime required by a resource to complete all tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968608(v=office.12).md">PercentWorkComplete</a></p></td>
<td><p>Optional</p></td>
<td><p>The current status of all tasks assigned to a resource, expressed as the total percentage of the resource's work that has been completed.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968453(v=office.12).md">StandardRate</a></p></td>
<td><p>Optional</p></td>
<td><p>The rate of pay for regular, non-overtime work performed by a resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968727(v=office.12).md">StandardRateFormat</a></p></td>
<td><p>Optional</p></td>
<td><p>The units used to display the standard rate.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968522(v=office.12).md">Cost</a></p></td>
<td><p>Optional</p></td>
<td><p>The total scheduled cost for a resource for all assigned tasks, based on costs already incurred for work performed by the resource on all assigned tasks in addition to the costs planned for all remaining work.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968679(v=office.12).md">OvertimeRate</a></p></td>
<td><p>Optional</p></td>
<td><p>The rate of pay for overtime work performed by a resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968737(v=office.12).md">OvertimeRateFormat</a></p></td>
<td><p>Optional</p></td>
<td><p>The units used to display the overtime rate.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968407(v=office.12).md">OvertimeCost</a></p></td>
<td><p>Optional</p></td>
<td><p>The total overtime cost for a resource on all assigned tasks.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968500(v=office.12).md">CostPerUse</a></p></td>
<td><p>Optional</p></td>
<td><p>The cost that accrues each time a resource is used.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968591(v=office.12).md">ActualCost</a></p></td>
<td><p>Optional</p></td>
<td><p>The sum of costs incurred for the work already performed by a resource for all assigned tasks.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968431(v=office.12).md">ActualOvertimeCost</a></p></td>
<td><p>Optional</p></td>
<td><p>The cost incurred for overtime work already performed by a resource for all assigned tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968728(v=office.12).md">RemainingCost</a></p></td>
<td><p>Optional</p></td>
<td><p>The remaining scheduled expense that will be incurred in completing the remaining work assigned to a resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968690(v=office.12).md">RemainingOvertimeCost</a></p></td>
<td><p>Optional</p></td>
<td><p>The remaining scheduled overtime expense of a resource that will be incurred in completing the remaining planned overtime work by a resource on all assigned tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968689(v=office.12).md">WorkVariance</a></p></td>
<td><p>Optional</p></td>
<td><p>The difference between a resource's total baseline work and the currently scheduled work.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968683(v=office.12).md">CostVariance</a></p></td>
<td><p>Optional</p></td>
<td><p>The difference between the baseline cost and total cost for a resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968647(v=office.12).md">SV</a></p></td>
<td><p>Optional</p></td>
<td><p>The difference in cost between the current progress and the baseline plan of all the resource's assigned tasks up to the status date or today's date; also called earned value schedule variance.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968685(v=office.12).md">CV</a></p></td>
<td><p>Optional</p></td>
<td><p>The difference between how much it should have cost for the resource to achieve the current level of completion, and how much it has actually cost to achieve the current level of completion, up to the status date or today's date.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968717(v=office.12).md">ACWP</a></p></td>
<td><p>Optional</p></td>
<td><p>The sum of actual cost of work performed (ACWP) values for all of a resource's assignments, up to the status date or today's date.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968514(v=office.12).md">CalendarUID</a></p></td>
<td><p>Optional</p></td>
<td><p>The unique ID for the calendar associated with this resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968616(v=office.12).md">Notes</a></p></td>
<td><p>Optional</p></td>
<td><p>Notes about a resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968411(v=office.12).md">BCWS</a></p></td>
<td><p>Optional</p></td>
<td><p>The rolled-up summary of a resource's BCWS values for all assigned tasks; also called budgeted cost of work scheduled.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968714(v=office.12).md">BCWP</a></p></td>
<td><p>Optional</p></td>
<td><p>The rolled-up summary of a resource's BCWP values for all assigned tasks, calculated up to the status date or today's date; also called budgeted cost of work performed.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968577(v=office.12).md">IsGeneric</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the resource is an enterprise-level generic resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968663(v=office.12).md">IsInactive</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the resource is an active (enabled) or inactive user.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968668(v=office.12).md">IsEnterprise</a></p></td>
<td><p>Optional</p></td>
<td><p>Specifies whether the resource is an enterprise resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968505(v=office.12).md">BookingType</a></p></td>
<td><p>Optional</p></td>
<td><p>Specifies the booking type of the resource (committed or proposed).</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968400(v=office.12).md">ActualWorkProtected</a></p></td>
<td><p>Optional</p></td>
<td><p>Specifies the duration through which actual work is protected.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968676(v=office.12).md">ActualOvertimeWorkProtected</a></p></td>
<td><p>Optional</p></td>
<td><p>Specifies the duration through which actual overtime work is protected.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968497(v=office.12).md">ActiveDirectoryGUID</a></p></td>
<td><p>Optional</p></td>
<td><p>The Active Directory GUID for the resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968396(v=office.12).md">CreationDate</a></p></td>
<td><p>Optional</p></td>
<td><p>The date that the project, resource, or assignment was created.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968669(v=office.12).md">ExtendedAttribute</a></p></td>
<td><p>Optional</p></td>
<td><p>A custom field definition associated with a resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968599(v=office.12).md">Baseline</a></p></td>
<td><p>Optional</p></td>
<td><p>A set of project estimates used for tracking purposes.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968410(v=office.12).md">OutlineCode</a></p></td>
<td><p>Optional</p></td>
<td><p>A custom tag defined for a resource that enables an alternate project structure.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968549(v=office.12).md">IsCostResource</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Indicates whether the resource is a cost resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968408(v=office.12).md">AssnOwner</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Name of the assignment owner.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968551(v=office.12).md">AssnOwnerGuid</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. The GUID of the assignment owner.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968612(v=office.12).md">IsBudget</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Indicates whether the resource is a budget resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968747(v=office.12).md">AvailabilityPeriods</a></p></td>
<td><p>Optional</p></td>
<td><p>The collection of dates the resource is available.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968693(v=office.12).md">Rates</a></p></td>
<td><p>Optional</p></td>
<td><p>The collection of pay rates for the resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968524(v=office.12).md">c408000 – c417fff</a></p></td>
<td><p>Optional</p></td>
<td><p>Enterprise resource custom field data.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968669(v=office.12).md">ExtendedAttribute</a></p></td>
<td><p>Optional</p></td>
<td><p>Local resource custom field data.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968479(v=office.12).md">TimephasedData</a></p></td>
<td><p>Optional</p></td>
<td><p>The timephased data block associated with the resource.</p></td>
</tr>
</tbody>
</table>

## Occurrences

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Minimum: 0</p>
<p>Maximum: Unbounded</p></td>
</tr>
</tbody>
</table>

## See Also

#### Concepts

[Resource Elements and XML Structure](bb968445\(v=office.12\).md)

[XML Schema for the Resources Element](bb968511\(v=office.12\).md)

