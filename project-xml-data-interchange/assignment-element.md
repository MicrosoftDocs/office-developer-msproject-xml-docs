---
title: Assignment Element
ms.date: 03/14/2018
monikerRange: '>= project-client-2010 || project-client-odc'
localization_priority: Normal
---

# Assignment Element




There must be at least one assignment in each Assignments collection.

    <Assignment>
      ComplexTypeValue
    </Assignment>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="assignments-element.md">Assignments</a></p></td>
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
<td><p><a href="uid-element.md">UID</a></p></td>
<td><p>Required</p></td>
<td><p>The unique ID for the assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="guid-element-multiple-parents.md">GUID</a></p></td>
<td><p>Optional</p></td>
<td><p>The GUID for the assignment.</p></td>
</tr>
<tr class="even">
<td><p><a href="taskuid-element.md">TaskUID</a></p></td>
<td><p>Optional</p></td>
<td><p>The unique ID for the task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="resourceuid-element.md">ResourceUID</a></p></td>
<td><p>Optional</p></td>
<td><p>The unique ID for the resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="percentworkcomplete-element.md">PercentWorkComplete</a></p></td>
<td><p>Optional</p></td>
<td><p>The current status of an assignment, expressed as the percentage of the assignment's work that has been completed.</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualcost-element.md">ActualCost</a></p></td>
<td><p>Optional</p></td>
<td><p>The cost incurred for work already performed by a resource on a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="actualfinish-element.md">ActualFinish</a></p></td>
<td><p>Optional</p></td>
<td><p>The date and time when an assignment was actually completed.</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualovertimecost-element.md">ActualOvertimeCost</a></p></td>
<td><p>Optional</p></td>
<td><p>The cost incurred for overtime work already performed by a resource on a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="actualovertimework-element.md">ActualOvertimeWork</a></p></td>
<td><p>Optional</p></td>
<td><p>The actual amount of overtime work already performed by a resource on an assigned task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualstart-element.md">ActualStart</a></p></td>
<td><p>Optional</p></td>
<td><p>The date and time that an assignment actually began.</p></td>
</tr>
<tr class="even">
<td><p><a href="actualwork-element.md">ActualWork</a></p></td>
<td><p>Optional</p></td>
<td><p>The amount of work that has already been done by a resource on a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="acwp-element.md">ACWP</a></p></td>
<td><p>Optional</p></td>
<td><p>The costs incurred for work already performed by a resource on a task up to the project status date or today's date; also called actual cost of work performed.</p></td>
</tr>
<tr class="even">
<td><p><a href="confirmed-element.md">Confirmed</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether a resource assigned to a task has accepted or rejected the task assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="cost-element.md">Cost</a></p></td>
<td><p>Optional</p></td>
<td><p>The total scheduled (or projected) cost for an assignment.</p></td>
</tr>
<tr class="even">
<td><p><a href="costratetable-element.md">CostRateTable</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates which cost rate table to use for a resource on an assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="costvariance-element.md">CostVariance</a></p></td>
<td><p>Optional</p></td>
<td><p>The difference between the baseline cost and total cost for an assignment.</p></td>
</tr>
<tr class="even">
<td><p><a href="cv-element.md">CV</a></p></td>
<td><p>Optional</p></td>
<td><p>The difference between how much it should have cost to achieve the current level of completion on the assignment and how much it has actually cost.</p></td>
</tr>
<tr class="odd">
<td><p><a href="delay-element.md">Delay</a></p></td>
<td><p>Optional</p></td>
<td><p>The amount of time a resource is to wait after the task start date before starting work on an assignment.</p></td>
</tr>
<tr class="even">
<td><p><a href="finish-element.md">Finish</a></p></td>
<td><p>Optional</p></td>
<td><p>The date and time that an assigned resource is scheduled to complete work on a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="finishvariance-element.md">FinishVariance</a></p></td>
<td><p>Optional</p></td>
<td><p>The difference between an assignment's baseline finish date and its scheduled finish date.</p></td>
</tr>
<tr class="even">
<td><p><a href="hyperlink-element.md">Hyperlink</a></p></td>
<td><p>Optional</p></td>
<td><p>The title or explanatory text for a hyperlink associated with an assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="hyperlinkaddress-element.md">HyperlinkAddress</a></p></td>
<td><p>Optional</p></td>
<td><p>The address for a hyperlink associated with an assignment.</p></td>
</tr>
<tr class="even">
<td><p><a href="hyperlinksubaddress-element.md">HyperlinkSubAddress</a></p></td>
<td><p>Optional</p></td>
<td><p>The specific location in a document within a hyperlink associated with an assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="workvariance-element.md">WorkVariance</a></p></td>
<td><p>Optional</p></td>
<td><p>The difference between an assignment's baseline work and the currently scheduled work.</p></td>
</tr>
<tr class="even">
<td><p><a href="hasfixedrateunits-element.md">HasFixedRateUnits</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether an assignment has fixed rate units.</p></td>
</tr>
<tr class="odd">
<td><p><a href="fixedmaterial-element.md">FixedMaterial</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the consumption of the assigned material resource occurs in a single, fixed amount.</p></td>
</tr>
<tr class="even">
<td><p><a href="levelingdelay-element.md">LevelingDelay</a></p></td>
<td><p>Optional</p></td>
<td><p>The amount of time that an assignment is to be delayed from the scheduled start date as a result of resource leveling.</p></td>
</tr>
<tr class="odd">
<td><p><a href="levelingdelayformat-element.md">LevelingDelayFormat</a></p></td>
<td><p>Optional</p></td>
<td><p>The format for expressing the duration of the delay.</p></td>
</tr>
<tr class="even">
<td><p><a href="linkedfields-element.md">LinkedFields</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether there are OLE links to the assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="milestone-element.md">Milestone</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the assignment task is a milestone.</p></td>
</tr>
<tr class="even">
<td><p><a href="notes-element.md">Notes</a></p></td>
<td><p>Optional</p></td>
<td><p>Notes about an assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="overallocated-element.md">OverAllocated</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether a resource is assigned to more work on a specific task than can be done within the resource's normal working capacity.</p></td>
</tr>
<tr class="even">
<td><p><a href="overtimecost-element.md">OvertimeCost</a></p></td>
<td><p>Optional</p></td>
<td><p>The total overtime cost for a resource assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="overtimework-element.md">OvertimeWork</a></p></td>
<td><p>Optional</p></td>
<td><p>The amount of overtime to be performed by a resource on a task; charged at the resource's overtime rate.</p></td>
</tr>
<tr class="even">
<td><p><a href="regularwork-element.md">RegularWork</a></p></td>
<td><p>Optional</p></td>
<td><p>The total amount of non-overtime work scheduled to be performed by a resource assigned to a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="remainingcost-element.md">RemainingCost</a></p></td>
<td><p>Optional</p></td>
<td><p>The costs associated with completing all remaining scheduled work by any resources on a specific task.</p></td>
</tr>
<tr class="even">
<td><p><a href="remainingovertimecost-element.md">RemainingOvertimeCost</a></p></td>
<td><p>Optional</p></td>
<td><p>The remaining scheduled overtime expense for an assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="remainingovertimework-element.md">RemainingOvertimeWork</a></p></td>
<td><p>Optional</p></td>
<td><p>The amount of overtime work that remains on an assignment.</p></td>
</tr>
<tr class="even">
<td><p><a href="remainingwork-element.md">RemainingWork</a></p></td>
<td><p>Optional</p></td>
<td><p>The amount of time required by a resource assigned to a task to complete an assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="responsepending-element.md">ResponsePending</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether an answer has been received from a message sent to a resource assigned to a task notifying the resource of the assignment.</p></td>
</tr>
<tr class="even">
<td><p><a href="start-element.md">Start</a></p></td>
<td><p>Optional</p></td>
<td><p>The date and time that an assigned resource is scheduled to begin working on a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="https://msdn.microsoft.com/en-us/library/office%7cps12con%7c%7e%5chtml%5c3b4f7a6c-e08d-456e-85b4-186090f7791.htm(v=office.12)">Stop</a></p></td>
<td><p>Optional</p></td>
<td><p>The date the assignment was stopped.</p></td>
</tr>
<tr class="even">
<td><p><a href="resume-element.md">Resume</a></p></td>
<td><p>Optional</p></td>
<td><p>The date the assignment was resumed.</p></td>
</tr>
<tr class="odd">
<td><p><a href="startvariance-element.md">StartVariance</a></p></td>
<td><p>Optional</p></td>
<td><p>The difference between an assignment's baseline start date and its currently scheduled start date.</p></td>
</tr>
<tr class="even">
<td><p><a href="summary-element.md">Summary</a></p></td>
<td><p>Optional</p></td>
<td><p>New for Project 2007. Indicates whether an assignment is for a summary task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="sv-element.md">SV</a></p></td>
<td><p>Optional</p></td>
<td><p>The earned value schedule variance, through the project status date</p></td>
</tr>
<tr class="even">
<td><p><a href="units-element.md">Units</a></p></td>
<td><p>Optional</p></td>
<td><p>The number of units for which a resource is assigned to a task, expressed as a percentage.</p></td>
</tr>
<tr class="odd">
<td><p><a href="updateneeded-element.md">UpdateNeeded</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether a TeamUpdate message should be sent to the resource assigned to a task because of changes to the start date, finish date, or resource reassignments.</p></td>
</tr>
<tr class="even">
<td><p><a href="vac-element.md">VAC</a></p></td>
<td><p>Optional</p></td>
<td><p>The variance at completion (VAC) between the baseline cost and the total cost for an assignment on a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="work-element.md">Work</a></p></td>
<td><p>Optional</p></td>
<td><p>The total amount of work scheduled to be performed by a resource on a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="workcontour-element.md">WorkContour</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates how work for an assignment is to be distributed across the duration of the assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bcws-element.md">BCWS</a></p></td>
<td><p>Optional</p></td>
<td><p>The budgeted cost of work scheduled on the assignment.</p></td>
</tr>
<tr class="even">
<td><p><a href="bcwp-element.md">BCWP</a></p></td>
<td><p>Optional</p></td>
<td><p>The budgeted cost of the work performed on the assignment to-date.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bookingtype-element.md">BookingType</a></p></td>
<td><p>Optional</p></td>
<td><p>Specifies the booking type of the assignment (committed or proposed).</p></td>
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
<td><p><a href="creationdate-element.md">CreationDate</a></p></td>
<td><p>Optional</p></td>
<td><p>The date that the assignment was created.</p></td>
</tr>
<tr class="odd">
<td><p><a href="assnowner-element.md">AssnOwner</a></p></td>
<td><p>Optional</p></td>
<td><p>New for Project 2007. The name of the assignment owner.</p></td>
</tr>
<tr class="even">
<td><p><a href="assnownerguid-element.md">AssnOwnerGuid</a></p></td>
<td><p>Optional</p></td>
<td><p>New for Project 2007. The GUID of the assignment owner.</p></td>
</tr>
<tr class="odd">
<td><p><a href="budgetcost-element.md">BudgetCost</a></p></td>
<td><p>Optional</p></td>
<td><p>New for Project 2007. The budgeted amount for cost resources on this assignment.</p></td>
</tr>
<tr class="even">
<td><p><a href="budgetwork-element.md">BudgetWork</a></p></td>
<td><p>Optional</p></td>
<td><p>New for Project 2007. The budgeted work amount for work or material resources on this assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="extendedattribute-element.md">ExtendedAttribute</a></p></td>
<td><p>Optional</p></td>
<td><p>The value of an extended attribute (custom field).</p></td>
</tr>
<tr class="even">
<td><p><a href="baseline-element.md">Baseline</a></p></td>
<td><p>Optional</p></td>
<td><p>The collection of baseline values associated with the assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="f404000-f4040c8-elements.md">f404000 - f4040c8 Elements</a></p></td>
<td><p>Optional</p></td>
<td><p>New for Project 2007. An assignment-level local custom field value.</p></td>
</tr>
<tr class="even">
<td><p><a href="f408000-f417fff-elements.md">f408000 - f417fff Elements</a></p></td>
<td><p>Optional</p></td>
<td><p>New for Project 2007. An assignment-level enterprise custom field value.</p></td>
</tr>
<tr class="odd">
<td><p><a href="timephaseddata-element.md">TimephasedData</a></p></td>
<td><p>Optional</p></td>
<td><p>Information about the assignment that is distributed over time.</p></td>
</tr>
<tr class="even">
<td><p><a href="notecontainsobjects-element.md">NoteContainsObjects</a></p></td>
<td><p>Optional</p></td>
<td><p>This value is true if the note for an assignment contains an object.</p></td>
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

[Assignment Elements and XML Structure](assignment-elements-and-xml-structure.md)

[XML Schema for the Assignments Element](xml-schema-for-the-assignments-element.md)

[TimephasedDataType Elements and XML Structure](timephaseddatatype-elements-and-xml-structure.md)

