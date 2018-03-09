---
title: Resource Element
ms.date: 03/08/2018
monikerRange: '>= project-client-2010 || project-client-odc'
---

# Resource Element




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
<td><p><a href="resources-element.md">Resources</a></p></td>
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
<tr class="even">
<td><p><a href="uid-element.md">UID Element</a></p></td>
<td><p>Required</p></td>
<td><p>The unique ID for the resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="guid-element-multiple-parents.md">GUID</a></p></td>
<td><p>Optional</p></td>
<td><p>The GUID for the resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="id-element.md">ID Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The position identifier of the resource within the list of resources.</p></td>
</tr>
<tr class="odd">
<td><p><a href="name-element.md">Name Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The name of the resource; must be unique within the enterprise, whether or not the resource is active.</p></td>
</tr>
<tr class="even">
<td><p><a href="type-element-multiple-parents.md">Type Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The resource type (work or material).</p></td>
</tr>
<tr class="odd">
<td><p><a href="isnull-element.md">IsNull Element</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the resource is a null resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="initials-element.md">Initials Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The initials of a resource name.</p></td>
</tr>
<tr class="odd">
<td><p><a href="phonetics-element.md">Phonetics Element</a></p></td>
<td><p>Optional</p></td>
<td><p>Contains phonetic information in either Hiragana or Katakana for resource names; used only in the Japanese version of Microsoft Office Project.</p></td>
</tr>
<tr class="even">
<td><p><a href="ntaccount-element.md">NTAccount Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The Microsoft Windows NT Account name for a resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="materiallabel-element.md">MaterialLabel Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The unit of measurement entered for a material resource, for example, tons, boxes, or cubic yards.</p></td>
</tr>
<tr class="even">
<td><p><a href="code-element.md">Code Element</a></p></td>
<td><p>Optional</p></td>
<td><p>A code, abbreviation, or number entered as part of a resource's information.</p></td>
</tr>
<tr class="odd">
<td><p><a href="group-element.md">Group Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The name of the group the resource belongs to.</p></td>
</tr>
<tr class="even">
<td><p><a href="workgroup-element.md">WorkGroup Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The messaging method used to communicate with a project team.</p></td>
</tr>
<tr class="odd">
<td><p><a href="emailaddress-element.md">EmailAddress Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The e-mail address of a resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="hyperlink-element.md">Hyperlink Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The title or explanatory text for a hyperlink associated with a resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="hyperlinkaddress-element.md">HyperlinkAddress Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The address for a hyperlink associated with a resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="hyperlinksubaddress-element.md">HyperlinkSubAddress Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The specific location in a document within a hyperlink associated with a resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="maxunits-element.md">MaxUnits Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The maximum percentage, or number of units, that represents the maximum amount that a resource is available to accomplish any tasks during the current time period.</p></td>
</tr>
<tr class="even">
<td><p><a href="peakunits-element.md">PeakUnits Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The maximum percentage, or number of units, that a resource is assigned at any one time for all tasks assigned to that resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="overallocated-element.md">OverAllocated Element</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether a resource is assigned to do more work on all assigned tasks than can be done within the resource's normal work capacity.</p></td>
</tr>
<tr class="even">
<td><p><a href="availablefrom-element.md">AvailableFrom Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The starting date that a resource is available for work at the units specified for the current time period.</p></td>
</tr>
<tr class="odd">
<td><p><a href="availableto-element.md">AvailableTo Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The ending date that a resource will be available for work at the units specified for the current time period.</p></td>
</tr>
<tr class="even">
<td><p><a href="start-element.md">Start Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The date and time that a resource is scheduled to start work on all assigned tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="finish-element.md">Finish Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The date and time that a resource is scheduled to complete work on all assigned tasks.</p></td>
</tr>
<tr class="even">
<td><p><a href="canlevel-element.md">CanLevel Element</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether resource leveling can be performed with a resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="accrueat-element.md">AccrueAt Element</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates how and when resource standard and overtime costs are to be charged, or accrued, to the cost of a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="work-element.md">Work Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The total amount of work scheduled to be performed by a resource on all assigned tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="regularwork-element.md">RegularWork Element</a></p></td>
<td><p>Optional</p></td>
<td><p>The total amount of non-overtime work scheduled to be performed for all assignments assigned to a resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="overtimework-element.md">OvertimeWork</a></p></td>
<td><p>Optional</p></td>
<td><p>The amount of overtime to be performed for all tasks assigned to a resource and charged at the resource's overtime rate.</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualwork-element.md">ActualWork</a></p></td>
<td><p>Optional</p></td>
<td><p>The actual amount of work that has already been done for all assignments assigned to a resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="remainingwork-element.md">RemainingWork</a></p></td>
<td><p>Optional</p></td>
<td><p>The amount of time, or person-hours, still required by a resource to complete all assigned tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualovertimework-element.md">ActualOvertimeWork</a></p></td>
<td><p>Optional</p></td>
<td><p>The actual amount of overtime work already performed for all assignments assigned to a resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="remainingovertimework-element.md">RemainingOvertimeWork</a></p></td>
<td><p>Optional</p></td>
<td><p>The remaining amount of overtime required by a resource to complete all tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="percentworkcomplete-element.md">PercentWorkComplete</a></p></td>
<td><p>Optional</p></td>
<td><p>The current status of all tasks assigned to a resource, expressed as the total percentage of the resource's work that has been completed.</p></td>
</tr>
<tr class="even">
<td><p><a href="standardrate-element.md">StandardRate</a></p></td>
<td><p>Optional</p></td>
<td><p>The rate of pay for regular, non-overtime work performed by a resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="standardrateformat-element.md">StandardRateFormat</a></p></td>
<td><p>Optional</p></td>
<td><p>The units used to display the standard rate.</p></td>
</tr>
<tr class="even">
<td><p><a href="cost-element.md">Cost</a></p></td>
<td><p>Optional</p></td>
<td><p>The total scheduled cost for a resource for all assigned tasks, based on costs already incurred for work performed by the resource on all assigned tasks in addition to the costs planned for all remaining work.</p></td>
</tr>
<tr class="odd">
<td><p><a href="overtimerate-element.md">OvertimeRate</a></p></td>
<td><p>Optional</p></td>
<td><p>The rate of pay for overtime work performed by a resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="overtimerateformat-element.md">OvertimeRateFormat</a></p></td>
<td><p>Optional</p></td>
<td><p>The units used to display the overtime rate.</p></td>
</tr>
<tr class="odd">
<td><p><a href="overtimecost-element.md">OvertimeCost</a></p></td>
<td><p>Optional</p></td>
<td><p>The total overtime cost for a resource on all assigned tasks.</p></td>
</tr>
<tr class="even">
<td><p><a href="costperuse-element.md">CostPerUse</a></p></td>
<td><p>Optional</p></td>
<td><p>The cost that accrues each time a resource is used.</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualcost-element.md">ActualCost</a></p></td>
<td><p>Optional</p></td>
<td><p>The sum of costs incurred for the work already performed by a resource for all assigned tasks.</p></td>
</tr>
<tr class="even">
<td><p><a href="actualovertimecost-element.md">ActualOvertimeCost</a></p></td>
<td><p>Optional</p></td>
<td><p>The cost incurred for overtime work already performed by a resource for all assigned tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="remainingcost-element.md">RemainingCost</a></p></td>
<td><p>Optional</p></td>
<td><p>The remaining scheduled expense that will be incurred in completing the remaining work assigned to a resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="remainingovertimecost-element.md">RemainingOvertimeCost</a></p></td>
<td><p>Optional</p></td>
<td><p>The remaining scheduled overtime expense of a resource that will be incurred in completing the remaining planned overtime work by a resource on all assigned tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="workvariance-element.md">WorkVariance</a></p></td>
<td><p>Optional</p></td>
<td><p>The difference between a resource's total baseline work and the currently scheduled work.</p></td>
</tr>
<tr class="even">
<td><p><a href="costvariance-element.md">CostVariance</a></p></td>
<td><p>Optional</p></td>
<td><p>The difference between the baseline cost and total cost for a resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="sv-element.md">SV</a></p></td>
<td><p>Optional</p></td>
<td><p>The difference in cost between the current progress and the baseline plan of all the resource's assigned tasks up to the status date or today's date; also called earned value schedule variance.</p></td>
</tr>
<tr class="even">
<td><p><a href="cv-element.md">CV</a></p></td>
<td><p>Optional</p></td>
<td><p>The difference between how much it should have cost for the resource to achieve the current level of completion, and how much it has actually cost to achieve the current level of completion, up to the status date or today's date.</p></td>
</tr>
<tr class="odd">
<td><p><a href="acwp-element.md">ACWP</a></p></td>
<td><p>Optional</p></td>
<td><p>The sum of actual cost of work performed (ACWP) values for all of a resource's assignments, up to the status date or today's date.</p></td>
</tr>
<tr class="even">
<td><p><a href="calendaruid-element.md">CalendarUID</a></p></td>
<td><p>Optional</p></td>
<td><p>The unique ID for the calendar associated with this resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="notes-element.md">Notes</a></p></td>
<td><p>Optional</p></td>
<td><p>Notes about a resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="bcws-element.md">BCWS</a></p></td>
<td><p>Optional</p></td>
<td><p>The rolled-up summary of a resource's BCWS values for all assigned tasks; also called budgeted cost of work scheduled.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bcwp-element.md">BCWP</a></p></td>
<td><p>Optional</p></td>
<td><p>The rolled-up summary of a resource's BCWP values for all assigned tasks, calculated up to the status date or today's date; also called budgeted cost of work performed.</p></td>
</tr>
<tr class="even">
<td><p><a href="isgeneric-element.md">IsGeneric</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the resource is an enterprise-level generic resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="isinactive-element.md">IsInactive</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the resource is an active (enabled) or inactive user.</p></td>
</tr>
<tr class="even">
<td><p><a href="isenterprise-element.md">IsEnterprise</a></p></td>
<td><p>Optional</p></td>
<td><p>Specifies whether the resource is an enterprise resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bookingtype-element.md">BookingType</a></p></td>
<td><p>Optional</p></td>
<td><p>Specifies the booking type of the resource (committed or proposed).</p></td>
</tr>
<tr class="even">
<td><p><a href="actualworkprotected-element.md">ActualWorkProtected</a></p></td>
<td><p>Optional</p></td>
<td><p>Specifies the duration through which actual work is protected.</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualovertimeworkprotected-element.md">ActualOvertimeWorkProtected</a></p></td>
<td><p>Optional</p></td>
<td><p>Specifies the duration through which actual overtime work is protected.</p></td>
</tr>
<tr class="even">
<td><p><a href="activedirectoryguid-element.md">ActiveDirectoryGUID</a></p></td>
<td><p>Optional</p></td>
<td><p>The Active Directory GUID for the resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="creationdate-element.md">CreationDate</a></p></td>
<td><p>Optional</p></td>
<td><p>The date that the project, resource, or assignment was created.</p></td>
</tr>
<tr class="even">
<td><p><a href="extendedattribute-element.md">ExtendedAttribute</a></p></td>
<td><p>Optional</p></td>
<td><p>A custom field definition associated with a resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="baseline-element.md">Baseline</a></p></td>
<td><p>Optional</p></td>
<td><p>A set of project estimates used for tracking purposes.</p></td>
</tr>
<tr class="even">
<td><p><a href="outlinecode-element.md">OutlineCode</a></p></td>
<td><p>Optional</p></td>
<td><p>A custom tag defined for a resource that enables an alternate project structure.</p></td>
</tr>
<tr class="odd">
<td><p><a href="iscostresource-element.md">IsCostResource</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Indicates whether the resource is a cost resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="assnowner-element.md">AssnOwner</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Name of the assignment owner.</p></td>
</tr>
<tr class="odd">
<td><p><a href="assnownerguid-element.md">AssnOwnerGuid</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. The GUID of the assignment owner.</p></td>
</tr>
<tr class="even">
<td><p><a href="isbudget-element.md">IsBudget</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Indicates whether the resource is a budget resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="availabilityperiods-element.md">AvailabilityPeriods</a></p></td>
<td><p>Optional</p></td>
<td><p>The collection of dates the resource is available.</p></td>
</tr>
<tr class="even">
<td><p><a href="rates-element.md">Rates</a></p></td>
<td><p>Optional</p></td>
<td><p>The collection of pay rates for the resource.</p></td>
</tr>
<tr class="odd">
<td><p><a href="c408000-c417fff-elements.md">c408000 – c417fff</a></p></td>
<td><p>Optional</p></td>
<td><p>Enterprise resource custom field data.</p></td>
</tr>
<tr class="even">
<td><p><a href="extendedattribute-element.md">ExtendedAttribute</a></p></td>
<td><p>Optional</p></td>
<td><p>Local resource custom field data.</p></td>
</tr>
<tr class="odd">
<td><p><a href="timephaseddata-element.md">TimephasedData</a></p></td>
<td><p>Optional</p></td>
<td><p>The timephased data block associated with the resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="notecontainsobjects-element.md">NoteContainsObjects</a></p></td>
<td><p>Optional</p></td>
<td><p>This value is true if the note for a resource contains an object.</p></td>
</tr>
<tr class="odd">
<td><p><a href="enterpriseextendedattribute-element.md">
EnterpriseExtendedAttribute</a></p></td>
<td><p>Optional</p></td>
<td><p>Collection of Enterprise Custom Fields with lookup table values.</p></td>
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

[Resource Elements and XML Structure](resource-elements-and-xml-structure.md)

[XML Schema for the Resources Element](xml-schema-for-the-resources-element.md)

